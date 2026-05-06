# 🛡️ MWR CyberSec Virtual Internship – Week 10 (Injection Vulnerabilities)

🔗 **Room Link: https://tryhackme.com/room/MWR-CyberSec-Week-10-Injection-Attacks

---

## 📖 Overview

This room covers several common web application injection vulnerabilities and demonstrates how insecure input handling can lead to:

- Sensitive file disclosure
- Authentication bypass
- Remote compromise
- Server-side exploitation

Topics covered include:

- Path Traversal
- Local File Inclusion (LFI)
- NoSQL Injection
- XXE Injection
- LDAP Injection

---

## 🎯 Learning Objectives

- Understand common injection vulnerabilities
- Perform path traversal attacks
- Exploit Local File Inclusion vulnerabilities
- Understand MongoDB and NoSQL Injection
- Exploit XXE vulnerabilities
- Understand LDAP Injection authentication bypasses
- Learn secure mitigation techniques

---

## 🧠 Key Concepts

- Path Traversal
- Directory Traversal
- Local File Inclusion (LFI)
- NoSQL Injection
- XXE Injection
- LDAP Injection
- XML Entities
- Authentication Bypass
- SSRF
- Input Validation

---

# ✅ Questions and Answers

---

## 🔹 Task 1: Introduction

### Q: I've read up on the topics we covered this week and I'm ready to tackle my tenth assignment
**A:** No answer needed

---

# 🔹 Task 2: Path Traversal

### Q: Path Traversal allows you to access files outside of the ___ ____?
**A:** `Web Root`

---

### Q: Which special sequence is used to move up one directory level in a file path?
**A:** `../`

---

### Q: Image you are retrieving cat.png from C:\inetpub\wwwroot\images\, what payload would you need to read the \etc\hosts file on a Windows device.
**A:** `..\..\..\Windows\System32\drivers\etc\hosts`

---

# 🔹 Task 3: Local File Inclusion (LFI)

### Q: Give Lab #1 a try to read /etc/passwd. What would the request URI be?
**A:** `/lab1.php?file=/etc/passwd`

---

### Q: In Lab #2, what is the directory specified in the include function?
**A:** `includes`

---

### Q: Give Lab #3 a try to read /etc/passwd. What is the request look like?
**A:** `/lab3.php?file=../../../../etc/passwd`

---

### Q: Which function is causing the directory traversal in Lab #4?
**A:** `file_get_contents`

---

### Q: Try out Lab #6 and check what is the directory that has to be in the input field?
**A:** `THM-profile`

---

### Q: Try out Lab #6 and read /etc/os-release. What is the VERSION_ID value?
**A:** `12.04`

---

### Q: Go to http://MACHINE_IP/challenges/index.php and then capture Flag1 at /etc/flag1
**A:** 

---

### Q: Go to http://MACHINE_IP/challenges/index.php and then capture Flag2 at /etc/flag2
**A:** 

---

### Q: Go to http://MACHINE_IP/challenges/index.php and then capture Flag3 at /etc/flag3
**A:** 

---

# 🔹 Task 4: NoSQL Injection

### Q: What type of structure does MongoDB use instead of tables?
**A:** `documents`

---

### Q: What is a group of documents in MongoDB is known as?
**A:** `collection`

---

### Q: Using the MongoDB Operator Reference, what operator is used to filter data when a field isn't equal to a given value?
**A:** `$ne`

---

### Q: Following the example of the 3 documents given before, how many documents would be returned by the following filter:

```javascript
['gender' => ['$ne' => 'female'] , 'age' => ['$gt'=>'65'] ]
```

**A:** `0`

---

### Q: What type of NoSQL Injection is similar to normal SQL Injection?
**A:** `Syntax`

---

### Q: What type of NoSQL Injection allows you to modify the behaviour of the query, even if you can't escape the syntax?
**A:** `Operator`

---

### Q: What operator is used to find values less than a given number?
**A:** `$lt`

---

### Q: What are the two types of NoSQL Injection?
**A:** `Syntax Injection, Operator Injection`

---

# 🔹 Task 5: XXE Injection

### Q: What is the meaning of the acronym SGML?
**A:** `Standard Generalized Markup Language`

---

### Q: What is the meaning of the acronym DTD?
**A:** `Document Type Definition`

---

### Q: What XML parser builds the entire XML document into a memory-based tree structure, allowing random access to all parts of the document?
**A:** `DOM Parser`

---

### Q: What XXE vulnerability occurs when the server's response is immediately disclosed to the attacker without the use of external channels?
**A:** `In-Band XXE`

---

### Q: What is the content of the file 14232d6db2b5fd937aa92e8b3c48d958.txt in the /opt directory?

---

### Q: What kind of XXE vulnerability occurs when the response of the server is not visible to the attacker?
**A:** `Out-of-Band XXE`

---

### Q: What vulnerability can commonly be performed using XXE?
**A:** `SSRF`

---

# 🔹 Task 6: LDAP Injection

### Q: What is the flag?
**A:** 

---

### Q: What does LDAP Stand for?
**A:** `Lightweight Directory Access Protocol`

---

### Q: What port does Secured LDAP (LDAPS) communicate over
**A:** `636`

---

# 🔹 Task 7: More Challenges

### Q: I'm done week 10 YAY!!!!
**A:** No answer needed

---

# 🚀 Summary

This week demonstrated:

- Path Traversal attacks
- Local File Inclusion exploitation
- MongoDB NoSQL Injection
- XML External Entity attacks
- LDAP authentication bypasses
- Real-world injection exploitation techniques

---

# 🧠 Key Takeaway

> Improper input validation can lead to complete system compromise.

---

# 🏁 Skills Gained

- Web Exploitation
- Injection Attacks
- File Disclosure
- Authentication Bypass
- XML Exploitation
- LDAP Manipulation
- Secure Coding Awareness

---

# ⚠️ Disclaimer

This repository is for **educational purposes only**.  
All activities were performed in a **controlled TryHackMe lab environment**.
