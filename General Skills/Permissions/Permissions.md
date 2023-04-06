# **Permission**

## **Overview:**
---
Category: General Skills

Points: 100

## **Description**
---
Can you read files in the root file?
Additional details will be available after launching your challenge instance.

Note: This challenge launches an instance on demand.

## **Hints**
None.

## **Approach**

Connecting to the server and cd to \ I saw a directory named challenge, inside it there was a file which when cating it game the flag.

```
cd /
ls -la
cd challenge/
cat metadata.json
{"flag": "picoCTF{uS1ng_v1m_3dit0r_3dd6dcf4}", "username": "picoplayer", "password": "GhHrPQ2+zL"}
```


## **Flag**
---
>**picoCTF{uS1ng_v1m_3dit0r_3dd6dcf4}**









