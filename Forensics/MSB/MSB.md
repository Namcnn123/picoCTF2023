# **MSB**

## **Overview:**
---
Category: Forensics 

Points: 200

## **Description**
---
This image passes LSB statistical analysis, but we can't help but think there must be something to the visual artifacts present in this image...
Download the image [here](https://artifacts.picoctf.net/c/304/Ninja-and-Prince-Genji-Ukiyoe-Utagawa-Kunisada.flag.png).

## **Hints**
What's causing the 'corruption' of the image?

## **Approach**
---
I searched about MSB encode and i found this definition. 
```
The most significant bit (MSB) is the bit in a multiple-bit binary number with the largest value. This is usually the bit farthest to the left, or the bit transmitted first in a sequence. For example, in the binary number 1000, the MSB is 1, and in the binary number 0111, the MSB is 0.
```
So i thought the first bit will be the key that contains the hidden message. But i can't find any possible ways to solve this until i got a hint from my friend to use stegsolve tool, you can easily install [it](https://github.com/zardus/ctf-tools/blob/master/stegsolve/install).

After installed, use this command to run.
> java -jar stegsolve.jar 

Open the [image](Ninja-and-Prince-Genji-Ukiyoe-Utagawa-Kunisada.flag.png) and analyse it by the [firstbit](stegsolve.png). 

Then i found the flag in the data extracted [file](flag.png).

## **Flag**
---
>**picoCTF{15_y0ur_que57_qu1x071c_0r_h3r01c_06326238}**









