# **VM0**

## **Overview:**
---
Category: Reverse Engineering

Points: 100

## **Description**
---
Can you crack this black box?
We grabbed this design doc from enemy servers: Download. We know that the rotation of the red axle is input and the rotation of the blue axle is output. The following input gives the flag as output: [Download](input.txt).


## **Hints**
Rotating the axle that number of times is obviously not feasible. Can you model the mathematical relationship between red and blue?

## **Approach**
I used the information about mathematical relationship between red and blue from a friend.

Opening the model in blender we get a lego construction with 2 wheels:

1. Blue - 8 teeth
2. Red - 40 teeth

We're told that the input is the number of times we turned the red wheel and the output is the number of times we turned the blue wheel.

Turing the red wheel once rotates the blue wheel 5 times so that's their relationship (idea from the hint), so if we just multiply the input by 5 we get the output which is a number that's supposed to be the flag.

So i wrote a python code to get the flag:
```
from Crypto.Util.number import inverse, long_to_bytes
print(long_to_bytes(39722847074734820757600524178581224432297292490103995916782275668358702105*5))

```

## **Flag**
---
>**picoCTF{g34r5_0f_m0r3_5ca97824}**









