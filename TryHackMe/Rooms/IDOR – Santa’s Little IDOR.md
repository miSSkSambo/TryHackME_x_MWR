# 🎁 IDOR – Santa’s Little IDOR

---
link to the room: https://tryhackme.com/room/idor-aoc2025-zl6MywQid9

---
## 📌 Overview

This room introduces **IDOR (Insecure Direct Object Reference)**, a common web vulnerability caused by improper access control.

You investigate the **TryPresentMe** application and learn how attackers:
- Access other users’ data
- Exploit weak authorization checks
- Perform **horizontal privilege escalation**

---

## 🎯 Learning Objectives

- Understand **authentication vs authorization**
- Identify IDOR vulnerabilities in web apps
- Exploit IDOR through parameter manipulation
- Understand encoded and hashed references
- Learn how to prevent IDOR vulnerabilities

---

## 🧠 Key Concepts

- **IDOR (Insecure Direct Object Reference)**
- **Authentication vs Authorization**
- **Horizontal Privilege Escalation**
- **Base64 Encoding**
- **Hashing (MD5, SHA1)**
- **UUID Predictability**
- **Secure Design (SDOR)**

---

# ✅ Questions and Answers

## 🔹 Task 1: Introduction

**Q:** My target machine and AttackBox are ready  
**A:** No answer needed  

---

## 🔹 Task 2: IDOR on the Shelf

**Q:** What does IDOR stand for?  
**A:** Insecure Direct Object Reference  

**Q:** What type of privilege escalation are most IDOR cases?  
**A:** Horizontal  

**Q:** Exploiting the IDOR, what is the user_id of the parent with 10 children?  
**A:** 15

---

## 🎯 Bonus Tasks (Optional)

**Q:** Find child ID using base64 or MD5 endpoint  
**A:** No answer needed  

**Q:** Find voucher valid on 20 November 2025  
**A:** No answer needed  

---

## 🚀 Summary

This room demonstrates how **IDOR vulnerabilities occur when applications fail to enforce proper authorization checks**.

Key takeaways:
- Authentication verifies identity; authorization verifies access
- IDOR allows access to other users’ data
- Encoded or hashed IDs are **not secure**
- Predictable values (IDs, UUIDs) can be exploited

---

## ⚠️ Key Insight

IDOR is essentially an **authorization failure**:
- The system trusts user input (IDs)
- It does not verify ownership of data

---

## 🔐 Mitigation

- Always enforce **server-side authorization checks**
- Do not rely on hidden, encoded, or hashed IDs
- Use **random, non-sequential identifiers**
- Validate every request against user permissions
- Log and monitor suspicious access attempts

---

## 💡 Real-World Impact

IDOR vulnerabilities can lead to:
- Data breaches
- Account takeover
- Exposure of sensitive personal information

---
