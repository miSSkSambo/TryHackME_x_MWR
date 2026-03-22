# 🔐 Week 3 Assignment – Authentication & Brute Force Attacks - Q &  A notes

---
## 📌 Assignment Summary
This assignment focuses on understanding **authentication concepts** and how they are attacked in cybersecurity. It covers:

- The **IAAA model** (Identification, Authentication, Authorisation, Auditing)
- Types of **authentication factors** (something you know, have, are, or do)
- Common **login attacks** such as brute force and password spraying
- Using **Hydra**, a brute-force tool, to crack passwords
- Practical challenges involving **SSH and web authentication attacks**

The goal is to understand both **how authentication works** and **how attackers exploit weak security systems**. 

---
link for the room: https://tryhackme.com/jr/MWR-CyberSec-Week-3-Authentication-and-passwords 

## 🧩 Task 1 [Introduction]
**No answer needed**

---

## 🔑 Task 2 [Authentication]

**Q:** Match the IAAA: I can access the admin panel  
**A:** Authorisation  

**Q:** Match the IAAA: A picture of me accessing my profile page  
**A:** Auditing  

**Q:** Match the IAAA: Connecting from my home IP address  
**A:** Authentication  

**Q:** Match the IAAA: I am Tinus  
**A:** Identification  

---

**Q:** What authentication factor is: Answering a security questions  
**A:** Something you know  

**Q:** What authentication factor is: Interpretive Dance  
**A:** Something you do  

**Q:** What authentication factor is: A scan of my eyeball  
**A:** Something you are  

---

## ⚔️ Task 3 [Attacking Log In]

**Q:** What is the most well known password list  
**A:** rockyou.txt  

**Q:** What attack uses 1 password against many usernames  
**A:** password spray  

**Q:** What attack uses 1 username with many passwords  
**A:** brute force  

---

## 🛠️ Task 4 [Hydra Introduction]
**No answer needed**

---

## 💻 Task 5 [Using Hydra]

**Q:** Use Hydra to brute-force molly's web password. What is the value of flag 1?  
**A:** THM{2673a7dd116de68e85c48ec0b1f2612e}  

**Q:** Use Hydra to brute-force molly's SSH password. What is the value of flag 2?  
**A:** THM{c8eeb0468febbadea859baeb33b2541b}  

---

## 🚀 Task 6 [Start the next vm]
**No answer needed**

---

## 🧠 Task 7 [Challenge]

**Q:** What is the ssh password for the tommyboy1 user? This password is a URL encoded version of one of the passwords from the password list. So first encode the special characters in that list, then perform the attack with the encoded passwords  
**A:** 1qaz@WSX  

---

**Q:** When you ssh in, what is the name of the folder that you can see?  
**A:** DVWA-master  

---

**Q:** How do we differentiate between a failed and successful logins on the web application?  
**A:** Location Response Header  

---

**Q:** What is the password for the admin user on the web application? This attack can't use hydra because of the user_token, so you would need to use another tool that can request a new token each time.

You also need to use the unencoded version of the password list for this task

This is a difficult challenge, so if you do not complete this it is completely okay  
**A:** 1qaz@WSX  

---

## 🎯 Task 8 [More challenges]
**No answer needed**

---

## ✅ Conclusion
This assignment provided practical experience in:
- Understanding authentication systems
- Identifying weak password practices
- Performing brute-force attacks using tools like Hydra
- Analysing login responses in web applications

It highlights the importance of **strong passwords, secure authentication methods, and proper system configuration** to prevent attacks.

---

## 🧠 Key Takeaways
- Weak passwords are easily cracked using tools like Hydra  
- Authentication systems must implement protections (lockouts, MFA)  
- Understanding attacks helps improve defensive security  
- Real-world testing environments improve cybersecurity skills  

---
