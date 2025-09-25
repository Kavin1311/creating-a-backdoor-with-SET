# NAME: T.KAVINAJAI
# REGISTER NO: 212223100020
# creating-a-backdoor-with-SET
creating a backdoor with SET - Ethical Hacking Techniques course

# AIM:
To Create a backdoor with Social Engineering Toolkit (SET)

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode


### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

### Architecture Diagram

```
+----------------+        +------------------------+        +----------------------+
| Attacker's PC  | -----> | SET (Credential        | -----> | Fake Login Page      |
| (Kali Linux)   |        | Harvester via Apache)  |        | (Hosted by SET)      |
+----------------+        +------------------------+        +----------------------+
       |                                                             |
       |                                                             v
       |   1. Configure SET with phishing site (e.g., Gmail clone)   |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Victim's Browser     |
       | <------------------------------------------------| Clicks Phishing Link|
       |                                                 +----------------------+
       |                                                             |
       |                                                             v
       |     2. Victim Enters Credentials → Sent to SET/Attacker    |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Credentials Captured |
       |                                                 | in Apache log/SET DB |
       |                                                 +----------------------+

```

## EXECUTION STEPS AND ITS OUTPUT:
Social Engineering attacks are the various cons used by the hackers to trick people into providing sensitive data to the attackers.

**Steps to Use SET for Phishing (Credential Harvester Attack Method)**

**1. Open terminal:**
```bash
sudo setoolkit
```
<img width="678" height="632" alt="image" src="https://github.com/user-attachments/assets/abd6185c-527c-4a5c-9593-e30f9c3f1b40" />


**2. Navigate:**
```bash
1) Social-Engineering Attacks  
2) Website Attack Vectors  
3) Credential Harvester Attack Method  
```
**3. Enter your IP address as the attacker server.**
**4. Choose:**
```bash
2) Site Cloner

```
<img width="817" height="283" alt="image" src="https://github.com/user-attachments/assets/6c927c06-3d44-4bfa-b4dd-f23c65c9d291" />

**5. Enter the URL of the legitimate site ```(e.g., https://accounts.google.com)```**
<img width="891" height="93" alt="image" src="https://github.com/user-attachments/assets/e281695c-36c9-41b9-9be1-38e9beb381b4" />


**6. Send the generated link to the victim.**
<img width="1278" height="842" alt="image" src="https://github.com/user-attachments/assets/d106abe3-58c9-4642-921f-dc6e519f198c" />

**7. Once the victim logs in → their credentials are stored in:**
```bash
/var/www/html/
```
192.168.184.177
<img width="1148" height="308" alt="image" src="https://github.com/user-attachments/assets/923cfb42-f48a-4d2c-8fce-025c473f4c10" />


## RESULT:
The Social Engineering Toolkit (SET) is used to create backdoor is  examined successfully
