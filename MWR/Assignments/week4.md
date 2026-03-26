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

# ✅ Questions and Answers

## 🔹 Task 1: Introduction

**Q:** Ready to start  
**A:** No answer needed  

---

## 🔹 Task 2: IAAA Model

**Q:** Access to read/send email  
**A:** Authorisation  

**Q:** Enforcing proper use of access  
**A:** Accountability  

**Q:** Enter username  
**A:** Identification  

---

## 🔹 Task 3: Identification

**Q:** Which cannot be used for identification?  
**A:** Street number  

---

## 🔹 Task 4: Authentication

**Q:** Swipe card + PIN  
**A:** 4 (2FA)  

---

## 🔹 Task 5: Authorisation & Access Control

**Q:** Policy for secretary sending emails  
**A:** 1  

**Q:** Hotel staff access decision  
**A:** 1  

**Q:** Prevent file modification  
**A:** 2  

---

## 🔹 Task 6: Accountability

**Q:** Ready for practical  
**A:** No answer needed  

---

## 🔹 Task 7: IDOR Example 1

**Q:** Flag  
**A:** THM{IDOR-VULN-FOUND}  

---

## 🔹 Task 8: IDOR Example 2

**Q:** Username (ID 1)  
**A:** adam84  

**Q:** Email (ID 3)  
**A:** j@fakemail.thm  

---

## 🔹 Task 9: Token-Based Authentication

**Q:** JWT header used  
**A:** Authorization: Bearer  

---

## 🔹 Task 10: JWT Basics

**Q:** HS256 type  
**A:** Symmetric  

**Q:** RS256 type  
**A:** Asymmetric  

**Q:** Encrypted JWT  
**A:** JWE  

---

## 🔹 Task 11: JWT Exploitation (Example 1)

**Q:** Flag  
**A:** THM{c64473e0-aca8-4827-8f50-1bb747da6257}  

---

## 🔹 Task 12: JWT Attacks

**Q:** Flag (Example 2)  
**A:** THM{251be376-e73e-4585-90c3-87fda5723782}  

**Q:** Flag (Example 3)  
**A:** THM{867ebbea-c3b9-4ef2-9d94-21127a54156f}  

**Q:** Flag (Example 4)  
**A:** THM{0db46b86-50d9-4dd7-ba32-223a8662056a}  

**Q:** Flag (Example 5)  
**A:** THM{721260b7-690b-46f5-bfa5-e77006a4ef95}  

---

## 🔹 Task 13: Completion

**Q:** Finished assignment  
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
