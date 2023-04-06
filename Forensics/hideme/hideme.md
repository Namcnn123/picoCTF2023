# **hideme**

## **Overview:**
---
Category: Forensics 

Points: 100

## **Description**
---
Every file gets a flag.
The SOC analyst saw one image been sent back and forth between two people. They decided to investigate and found out that there was more than what meets the eye [here](picoFlag.png "picoFlag").

## **Hints**
---
None

## **Approach**
---
After downloaded the image, i tried to extract it.
```
binwalk -e flag.png  
unzip 9B3B.zip 
eog flag.png
```
Finally, we got an image which contains the flag.

![picoFlag](flag.png "flag")

## **Flag**
---
>**picoCTF{Hiddinng_An_imag3_within_@n_ima9e_568ea480}**









