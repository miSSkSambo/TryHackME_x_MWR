# 🧪 MWR CyberSec Virtual Internship — Week 6 (DOM & DOM-Based XSS)

---
link to the room: https://tryhackme.com/room/MWR-CyberSec-Week-6-DOM-and-XSS

---
<p align="center">
  <img src="https://img.shields.io/badge/MWR-Week%206-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Focus-DOM%20%7C%20DOM%20XSS-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-Web%20Security-green?style=for-the-badge" />
</p>

---

## 📌 Overview

This assignment focuses on **client-side vulnerabilities in modern web applications**, specifically:

* Document Object Model (DOM)
* DOM-Based Attacks
* DOM-Based Cross-Site Scripting (XSS)
* Security issues in Single Page Applications (SPA)

---

## 🎯 Objectives

* Understand how the DOM works  
* Identify **sources and sinks**  
* Exploit DOM-based vulnerabilities  
* Analyse modern frontend frameworks (Vue)  
* Perform DOM-based XSS attacks  
* Weaponise XSS for real impact  

---

## 🧠 Key Concepts

* DOM (Document Object Model)  
* Source vs Sink  
* Taint Analysis  
* DOM-Based XSS  
* URL Fragments  
* SPA (Single Page Applications)  
* Client-side vs Server-side security  

---

# 🧪 WALKTHROUGH SUMMARY

---

## 🔹 DOM Basics

✔ The DOM is a **tree-like structure**  
✔ JavaScript modifies the DOM dynamically  
✔ Enables interactive web applications  

---

## 🔹 DOM Attack Concept

1. User input (**Source**)  
2. Flows through JavaScript  
3. Injected into DOM (**Sink**)  
4. No validation → vulnerability  

---

## 🔹 SPA (Single Page Applications)

✔ Load once, update dynamically  
✔ Built using:

* Angular  
* React  
* Vue  

✔ More efficient but introduces security risks  

---

# ✅ FULL QUESTIONS & ANSWERS

---

## 🔹 Task 1

**Q:** Introduction complete  
**A:** No answer needed  

---

## 🔹 Task 2 — The DOM Explained

**Q:** What does DOM stand for?  
**A:** Document Object Model  

**Q:** What JavaScript command creates new HTML elements?  
**A:** createElement  

**Q:** What JavaScript command retrieves cookie values?  
**A:** document.cookie  

**Q:** What API call adds a node to the DOM?  
**A:** appendChild()  

**Q:** What API call removes a node?  
**A:** removeChild()  

---

## 🔹 Task 3 — Modern Frontend Frameworks

**Q:** What does SPA stand for?  
**A:** Single Page Application  

**Q:** Should security be implemented client-side or server-side?  
**A:** Server-side  

**Q:** What control ensures bad user data is filtered?  
**A:** Input Validation  

**Q:** How can Angular apps become vulnerable to XSS?  
**A:** Trusting Safe Values  

---

## 🔹 Task 4 — DOM-Based Attacks

**Q:** What is the location where untrusted user input enters?  
**A:** Source  

**Q:** What is the function where input is used?  
**A:** Sink  

**Q:** What is tracking input flow called?  
**A:** Taint Analysis  

---

## 🔹 Task 5 — DOM-Based XSS

**Q:** Most common source?  
**A:** URL Fragments  

**Q:** What browser protection helps prevent this?  
**A:** URL Encoding  

**Q:** What is a dangerous JavaScript function?  
**A:** eval()  

---

## 🔹 Task 6 — XSS Weaponisation

**Q:** What flag prevents JavaScript from accessing cookies?  
**A:** HTTPOnly  

**Q:** What security control limits where content loads from?  
**A:** Content Security Policy  

**Q:** What CSP directive weakens security?  
**A:** unsafe-inline  

---

## 🔹 Task 7 — DOM-Based Attack Challenge

**Q:** What is the source field name?  
**A:** person  

**Q:** What is the sink Vue directive?  
**A:** v-html  

**Q:** What is the vulnerability category?  
**A:** HTML Injection  

---

### 🏁 Final Flag

MWR{We-Have-Learnt-DOM-XSS}

---

## 🔹 Task 8 — Juice Shop Challenge

**Q:** Who picks the oranges?  
**A:** Uncle Dittmeyer  

**Q:** Login bypass hash?  
**A:** 690fa3247a99d651e0b26f947baf0b79b4f404a9  

**Q:** What is the admin email?  
**A:** admin@juice-sh.op  

**Q:** What field should not be exposed?  
**A:** password  

**Q:** What hash function is used?  
**A:** MD5  

**Q:** What is the admin password?  
**A:** admin123  

**Q:** What port is exposed?  
**A:** 22  

---

### 🔐 Flags

Bypass Login → 690fa3247a99d651e0b26f947baf0b79b4f404a9  
DOM XSS → 4a31a4fe0954199566e360a873802bf64d0d0a84  
Reflected XSS → 305021787d3e9cd9cebc057a021c2504550bb3b6  
Scoreboard → 2614339936e8282e2f820f023d4d998a1f95e02a  

---

# 🚀 Exploitation Flow

1. Identify input fields  
2. Locate source and sink  
3. Inject payload  
4. Execute in browser  
5. Perform actions as the user  

---

## ⚠️ Key Takeaways

* DOM-based attacks happen entirely client-side  
* Server-side protection alone is not enough  
* Input validation is critical  
* SPAs increase attack surface  
* XSS can fully compromise users  

---

## 💡 Final Insight

DOM XSS is powerful because:

- Runs inside the browser  
- Bypasses traditional protections  
- Harder to detect  
- Can fully control user sessions  

---

## 📚 Reference

MWR CyberSec Week 6 Assignment  

---

## 🏁 Final Thought

Mastering DOM XSS = mastering advanced web exploitation
