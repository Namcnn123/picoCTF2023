# **SafeOpener2**

## **Overview:**
---
Category: Reverse Engineering

Points: 100

## **Description**
---What can you do with this file?
I forgot the key to my safe but this [file](SafeOpener.class) is supposed to help me with retrieving the lost key. Can you help me unlock my safe?


## **Hints**
Download and try to decompile the file.

## **Approach**
Using an online java decompiler like [this](http://www.javadecompilers.com/) we get the following code:

And i found the line:
> final String encodedkey = "picoCTF{SAf3_0p3n3rr_y0u_solv3d_it_0e57c117}";


## **Flag**
---
>**picoCTF{SAf3_0p3n3rr_y0u_solv3d_it_0e57c117}**









