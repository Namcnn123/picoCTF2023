# **FindAndOpen**

## **Overview:**
---
Category: Forensics 

Points: 200

## **Description**
---
Someone might have hidden the password in the trace file.
Find the key to unlock this [file](https://artifacts.picoctf.net/c/493/flag.zip). [This tracefile](https://artifacts.picoctf.net/c/493/dump.pcap) might be good to analyze.

## **Hints**
1. Download the pcap and look for the password or flag.
2. Don't try to use a password cracking tool, there are easier ways here.

## **Approach**
---
After downloaded the .pcap file and the .zip file, i tried to read the .pcap with packet tracer.
I scrolled down to read all the packets. Look like the flag is not in here. But i found something interesting.
```
Flying on Ethernet secret: Is this the flag
iBwaWNvQ1RGe1Could the flag have been splitted?
AABBHHPJGTFRLKVGhpcyBpcyB0aGUgc2VjcmV0OiBwaWNvQ1RGe1IzNERJTkdfTE9LZF8=
PBwaWUvQ1RGesabababkjaASKBKSBACVVAVSDDSSSSDSKJBJS
PBwaWUvQ1RGe1Maybe try checking the other file
```
At first, i thought that the flag might be decoded by base64 in this string.
> AABBHHPJGTFRLKVGhpcyBpcyB0aGUgc2VjcmV0OiBwaWNvQ1RGe1IzNERJTkdfTE9LZF8=

But when i tried to decode it, nothing happended, so i decided to use only the data section.
> VGhpcyBpcyB0aGUgc2VjcmV0OiBwaWNvQ1RGe1IzNERJTkdfTE9LZF8=

Let's decode it by [Cyberchef](https://gchq.github.io/CyberChef/).
And i got it, but it seemed to be a part of the flag.
> This is the secret: picoCTF{R34DING_LOKd_

Then i used this as a password for the [zipfile](flag.zip). 


## **Flag**
---
>**picoCTF{R34DING_LOKd_fil56_succ3ss_419835ef}**









