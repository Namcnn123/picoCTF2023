# **ReadMyCert**

## **Overview:**
---
Category: General Skills

Points: 100

## **Description**
---
Flag format: picoCTF{Malwarename}
The first letter of the malware name should be capitalized and the rest lowercase.
Your friend just got hacked and has been asked to pay some bitcoins to 1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX. He doesn’t seem to understand what is going on and asks you for advice. Can you identify what malware he’s being a victim of?


## **Hints**
1. Some crypto-currencies abuse databases exist; check them out!
2. Maybe Google might help.

## **Approach**
Googling 1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX I got the [link](https://www.bitcoinabuse.com/reports/1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX) which had reports with descriptions and one of those descriptions points us to:

And i found this line:
> 	More information here: https://blog.avira.com/petya-strikes-back/

So i thought the flag is about petya!

## **Flag**
---
>**picoCTF{petya}**









