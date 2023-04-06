# **Gladitor0**

## **Overview:**
---
Category: Reverse Engineering

Points: 400

## **Description**
---
Can you make a CoreWars warrior that always loses, no ties?
Additional details will be available after launching your challenge instance.


## **Hints**
None

## **Approach**

Same as the first 2 challenge, this challenge is no exception. But this one take me a lot of effort to find the right source code :(.

```
;redcode-94nop
;name frenzy v6
;author Lukasz Grabun
;assert 1
                org     boot

step            equ     6000

start           add     #step+step,2
                mov     bomb,   @1
                mov     bomb,   @1
cl              jmp     -3,     >-8             ;hit to start clear
                mov     dbomb,  >start-4
                djn.f   -1,     >start-4
dbomb           dat.f   <5334,  dbomb-start+7
bomb            spl     #0,     #step

for 83
                dat     0,      0
rof

boot            mov     bomb,   2000
for 7
                mov     {boot,  <boot
rof
                jmp     @boot,  <-1000

end
```

## **Flag**
---
>**picoCTF{d3m0n_3xpung3r_47037b25}**









