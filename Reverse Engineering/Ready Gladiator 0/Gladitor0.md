# **Gladitor0**

## **Overview:**
---
Category: Reverse Engineering

Points: 100

## **Description**
---
Can you make a CoreWars warrior that always loses, no ties?
Additional details will be available after launching your challenge instance.


## **Hints**
None

## **Approach**
Ok so for this challenge I had to learn what CoreWars was, and its apparently its a game between two programs that are written in RedCode which is a pseudo-assembly language.

Our mission is to lose to the program provided 100 times.

I found a useful website about [this](http://moscova.inria.fr/~doligez/corewar/?fbclid=IwAR3JfmSrQrX5MjeIIXgKpHR9eBY40f-1UYtDVMI50PJYRMkqe0kaVdibj90) and it helped me a lot in the next 2 challenges. 

You can read more about CoreWars, but in this case, i simply changed the line
>mov 0,1 -> mov 0,2

## **Flag**
---
>**picoCTF{h3r0_t0_z3r0_4m1r1gh7_a220a377}**









