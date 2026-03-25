# 💉 SQL Injection 

---
link to the room:https://tryhackme.com/room/sqlinjectionlm

---
## 📌 Overview

This room introduces **SQL Injection (SQLi)** — one of the most common and dangerous web application vulnerabilities.

It covers:
- Database fundamentals
- SQL query basics
- Detecting SQL Injection
- Exploiting SQLi vulnerabilities
- Preventing SQL Injection attacks

---

## 🎯 Learning Objectives

- Understand how databases work
- Learn basic SQL commands (SELECT, INSERT, UPDATE, DELETE)
- Identify SQL Injection vulnerabilities
- Exploit SQLi (In-band, Blind, Time-based, Out-of-band)
- Learn mitigation techniques

---

## 🧠 Key Concepts

- **SQL (Structured Query Language)**
- **DBMS (Database Management System)**
- **Tables, Rows, Columns**
- **In-Band SQLi**
- **Blind SQLi (Boolean & Time-based)**
- **Out-of-Band SQLi**
- **Authentication Bypass**
- **Prepared Statements**

---

# ✅ Questions and Answers

## 🔹 Task 1: Brief

**Q:** What does SQL stand for?  
**A:** Structured Query Language  

---

## 🔹 Task 2: What is a Database?

**Q:** What controls a database?  
**A:** DBMS  

**Q:** What is the grid-like structure called?  
**A:** table  

---

## 🔹 Task 3: What is SQL?

**Q:** Which statement retrieves data?  
**A:** SELECT  

**Q:** Which clause retrieves data from multiple tables?  
**A:** UNION  

**Q:** Which statement adds data?  
**A:** INSERT  

---

## 🔹 Task 4: What is SQL Injection?

**Q:** What character ends an SQL query?  
**A:** ;  

---

## 🔹 Task 5: In-Band SQLi

**Q:** What is the flag for level 1?  
**A:** THM{SQL_INJECTION_3840}  

---

## 🔹 Task 6: Blind SQLi – Authentication Bypass

**Q:** What is the flag for level 2?  
**A:** THM{SQL_INJECTION_9581}  

---

## 🔹 Task 7: Blind SQLi – Boolean Based

**Q:** What is the flag for level 3?  
**A:** THM{SQL_INJECTION_1093}  

---

## 🔹 Task 8: Blind SQLi – Time Based

**Q:** What is the final flag?  
**A:** THM{SQL_INJECTION_MASTER}  

---

## 🔹 Task 9: Out-of-Band SQLi

**Q:** Which protocol can be used to exfiltrate data?  
**A:** DNS  

---

## 🔹 Task 10: Remediation

**Q:** Name a method to prevent SQL Injection  
**A:** Prepared Statements 

---

## 🚀 Summary

This room demonstrates how SQL Injection can:

- Bypass authentication
- Extract sensitive data
- Modify or delete database content
- Fully compromise web applications

---

## ⚠️ Key Takeaways

- SQLi occurs when **user input is not validated**
- Attackers can manipulate SQL queries
- Blind SQLi relies on **true/false or time delays**
- UNION-based SQLi is used to extract large data sets

---

## 🔐 Mitigation

- Use **Prepared Statements (Parameterized Queries)**
- Validate and sanitize all user input
- Escape special characters
- Apply least privilege to database accounts
- Disable verbose error messages

---

## 💡 Key Insight

SQL Injection remains one of the **most critical vulnerabilities** in web security and is part of the **OWASP Top 10**.

---
