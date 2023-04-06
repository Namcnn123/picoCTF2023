# **who is it**

## **Overview:**
---
Category: Forensics 

Points: 100

## **Description**
---
Someone just sent you an email claiming to be Google's co-founder Larry Page but you suspect a scam.
Can you help us identify whose mail server the email actually originated from?
Download the email file [here](https://artifacts.picoctf.net/c/499/email-export.eml "email file"). Flag: picoCTF{FirstnameLastname}

## **Hints**
---
whois can be helpful on IP addresses also, not only domain names.

## **Approach**
---
With the hints, i found a web page that could be helpful to get information from an IP address: [whoislookup](https://whois.domaintools.com/). Then i read the email file to find any Ip addresses and there is only one that i found.
> 173.249.33.206

Use the web to search and we got the result.
```
person:         Wilhelm Zwalina
address:        Contabo GmbH
```
Let's follown the format: picoCTF{FirstnameLastname}


## **Flag**
---
>**picoCTF{WilhelmZwalina}**