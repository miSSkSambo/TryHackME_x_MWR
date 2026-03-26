# 🛡️ MWR CyberSec Virtual Internship Assignment — Week 4

---

link to the room: https://tryhackme.com/room/MWR-CyberSec-Week-4-Authorisation-Sessions

---
## 📌 Overview

This assignment focuses on **core web security concepts**:

- JWT (JSON Web Tokens)
- Authorisation & Access Control
- Privilege Escalation
- IAAA Model (Identification, Authentication, Authorisation, Accountability)

You will:
- Understand authentication models
- Exploit IDOR vulnerabilities
- Analyse and manipulate JWTs
- Perform privilege escalation via APIs

---

## 🎯 Learning Objectives

- Understand the IAAA security model
- Identify authentication vs authorisation
- Exploit access control vulnerabilities (IDOR)
- Work with JWT-based authentication systems
- Exploit JWT misconfigurations
- Understand secure implementation practices

---

## 🧠 Key Concepts

- **IAAA Model**
- **JWT (JSON Web Tokens)**
- **IDOR (Insecure Direct Object Reference)**
- **Access Control**
- **Privilege Escalation**
- **Token-Based Authentication**
- **Signature Validation**
- **API Security**

---

## 🔹 Task 1: Introduction

**Q:** I've read up on the topics we covered this week and I'm ready to tackle my fourth assignment  
**A:** No answer needed  

---

## 🔹 Task 2: IAAA Model

**Q:** You are granted access to read and send an email. What is the name of this process?  
**A:** Authorisation  

**Q:** Although you have write access, you should only make changes if necessary for the task. Which process is required to enforce this policy?  
**A:** Accountability  

**Q:** Which process would require you to enter your username?  
**A:** Identification  

---

## 🔹 Task 3: Identification

**Q:** Which of the following cannot be used for identification?  
- Landline phone number  
- Street number  
- Health insurance card number  
- Student ID number  

**A:** Street number  

---

## 🔹 Task 4: Authentication

**Q:** You need to swipe your card and enter a four-digit PIN to access the elevator. Under which group does this authentication fall?  

1. Something you know  
2. Something you have  
3. Something you are  
4. 2FA  

**A:** 4  

---

## 🔹 Task 5: Authorisation and Access Control

(Answer with 1 or 2)  
1 = Authorisation  
2 = Access Control  

**Q:** The new policy states that the secretary should be able to send an email on the manager’s behalf. What is this policy dictating?  
**A:** 1  

**Q:** The hotel management decided that the cleaning staff needed access to all the hotel rooms to do their work. What phase is this decision part of?  
**A:** 1  

**Q:** You shared a document with your colleague and gave them view permissions so they could read without making changes. What would ensure that your file won’t be modified?  
**A:** 2  

---

## 🔹 Task 6: Accountability

**Q:** I'm done reading the information above Captain Jonno and ready to explore the practical!  
**A:** No answer needed  

---

## 🔹 Task 7: Broken Authorisation Example 1

**Q:** What is the Flag from the authorisation bypass example website?  
**A:** THM{IDOR-VULN-FOUND}  

---

## 🔹 Task 8: Broken Authorisation Example 2

**Q:** What is the username for user id 1?  
**A:** adam84  

**Q:** What is the email address for user id 3?  
**A:** j@fakemail.thm  

---

## 🔹 Task 9: Token-Based Authentication

**Q:** What is the common header used to transport the JWT in a request?  
**A:** Authorization: Bearer  

---

## 🔹 Task 10: JSON Web Tokens

**Q:** HS256 is an example of what type of signing algorithm?  
**A:** Symmetric  

**Q:** RS256 is an example of what type of signing algorithm?  
**A:** Asymmetric  

**Q:** What is the name used for encrypted JWTs?  
**A:** JWE  

---

## 🔹 Task 11: JWT Sensitive Information Disclosure

**Q:** What is the flag for example 1?  
**A:** THM{c64473e0-aca8-4827-8f50-1bb747da6257}  

---

## 🔹 Task 12: JWT Signature Validation Mistakes

**Q:** What is the flag for example 2?  
**A:** THM{251be376-e73e-4585-90c3-87fda5723782}  

**Q:** What is the flag for example 3?  
**A:** THM{867ebbea-c3b9-4ef2-9d94-21127a54156f}  

**Q:** What is the flag for example 4?  
**A:** THM{0db46b86-50d9-4dd7-ba32-223a8662056a}  

**Q:** What is the flag for example 5?  
**A:** THM{721260b7-690b-46f5-bfa5-e77006a4ef95}  

---

## 🔹 Task 13: More Challenges

**Q:** I'm done week 4 YAY!!!!  
**A:** No answer needed  

---

# 🚀 Summary

This assignment demonstrated how weak implementations in authentication and authorisation can lead to serious vulnerabilities.

You performed:
- IDOR exploitation  
- JWT manipulation  
- Privilege escalation via API  
- Token forgery attacks  

---

## ⚠️ Key Takeaways

- Never trust user input (IDOR risk)
- Always validate JWT signatures
- Avoid weak secrets in symmetric encryption
- Do not allow algorithm downgrades (None attack)
- Separate authentication from authorisation checks

---

## 🔐 Common JWT Vulnerabilities

- ❌ No signature validation  
- ❌ `alg: none` bypass  
- ❌ Weak secret keys  
- ❌ Algorithm confusion (RS256 → HS256)  

---

## 🛡️ Mitigation

- Enforce strict access control checks  
- Validate JWT signatures properly  
- Use strong secrets  
- Restrict allowed algorithms  
- Implement proper logging & monitoring  

---

## 💡 Final Insight

Modern applications rely heavily on APIs and tokens.  
A single misconfiguration in JWT handling can lead to:

➡️ Full account takeover  
➡️ Privilege escalation  
➡️ Data exposure  

---

## 📚 Reference

Assignment based on MWR CyberSec Virtual Internship Week 4 
---
