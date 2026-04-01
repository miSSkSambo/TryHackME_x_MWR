# 🧪 MWR CyberSec Virtual Internship — Week 5 (XSS, SOP & CORS)

---
Llink to the room: https://tryhackme.com/room/MWR-CyberSec-Week-5-XSS

---
<p align="center">
  <img src="https://img.shields.io/badge/MWR-Week%205-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Focus-XSS%20%7C%20SOP%20%7C%20CORS-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-Web%20Security-green?style=for-the-badge" />
</p>

---

## 📌 Overview

This assignment focuses on **client-side web security**, covering:

* Cross-Site Scripting (XSS)
* Same-Origin Policy (SOP)
* Cross-Origin Resource Sharing (CORS)

You learn how attackers exploit web applications and how browsers enforce security boundaries.

---

## 🎯 Objectives

* Understand XSS payloads and types
* Perform practical XSS exploitation
* Understand SOP restrictions
* Learn how CORS allows controlled bypassing of SOP
* Exploit real-world web vulnerabilities

---

## 🧠 Key Concepts

* XSS (Reflected, Stored, DOM)
* Payload crafting
* JavaScript injection
* SOP security model
* CORS headers
* Browser-based attacks

---

# 🧪 WALKTHROUGH SUMMARY

---

## 🔹 XSS Payload Types

| Type             | Purpose                     |
| ---------------- | --------------------------- |
| Proof of Concept | Alert popup                 |
| Session Stealing | Capture cookies             |
| Key Logger       | Capture keystrokes          |
| Business Logic   | Modify application behavior |

---

## 🔹 XSS Types

* **Reflected XSS** → input reflected immediately
* **Stored XSS** → payload saved in database
* **DOM XSS** → executed in browser (client-side)

---

## 🔹 SOP (Same-Origin Policy)

✔ Restricts interaction between:

* Different domains
* Different ports
* Different protocols

✔ Prevents:

* Data theft across sites

---

## 🔹 CORS

✔ Allows controlled cross-origin access via headers:

* `Access-Control-Allow-Origin`
* `Access-Control-Allow-Methods`
* `Access-Control-Allow-Headers`

---

# ✅ FULL QUESTIONS & ANSWERS

---

## 🔹 Task 1

**Q:** Ready to start
**A:** No answer needed

---

## 🔹 Task 2 — XSS Payloads

**Q:** Language used for XSS payloads?
**A:** Javascript

**Q:** Capturing keystrokes payload?
**A:** Key Logger

**Q:** Changing delivery address payload?
**A:** Business Logic

---

## 🔹 Task 3 — Reflected XSS

**Q:** Where to test in URL?
**A:** parameters

---

## 🔹 Task 4 — Stored XSS

**Q:** Where are payloads stored?
**A:** database

---

## 🔹 Task 5 — XSS Terminology

**Q:** XSS executed in browser (not saved)?
**A:** Reflected XSS

**Q:** XSS that stores payload?
**A:** Stored XSS

---

## 🔹 Task 6 — XSS Practical 1

✔ Levels solved using payloads:

* `<script>alert('THM');</script>`
* `"><script>alert('THM');</script>`
* `</textarea><script>alert('THM');</script>`
* `';alert('THM');//`
* `<sscriptcript>alert('THM');</sscriptcript>`
* `/images/cat.jpg" onload="alert('THM');`

---

**Q:** Final flag
**A:** MWR{XSS_IS_EASY}

<img width="1015" height="876" alt="Screenshot 2026-04-02 011525" src="https://github.com/user-attachments/assets/58fa824e-dc92-4a68-ac28-d4532aa8ef62" />

---

## 🔹 Task 7 — SOP

**Q:** Policy controlling browser interaction?
**A:** Same-origin Policy

---

## 🔹 Task 8 — CORS

**Q:** Header that allows domains?
**A:** Access-Control-Allow-Origin

---

## 🔹 Task 9 — ACAO

**Q:** Least secure configuration?
**A:** Wildcard Origin

---

## 🔹 Task 10 — XSS Practical 2

**Q:** Moderator flag
**A:** MWR{I.am.the.MOD}

**Q:** Admin flag
**A:** MWR{and.the.Admin.too!}

---

## 🔹 Task 11

**Q:** Completed week
**A:** No answer needed

---

# 🚀 Exploitation Flow

1. Identify input fields
2. Inject JavaScript payload
3. Bypass filters
4. Execute in victim browser
5. Capture data / escalate access

---

## ⚠️ Key Takeaways

* XSS is one of the most common web vulnerabilities
* JavaScript is the core attack vector
* Filters can be bypassed creatively
* SOP protects users but can be bypassed with XSS
* CORS must be configured securely

---

## 💡 Final Insight

XSS is powerful because:

➡️ It runs inside the victim’s browser
➡️ It bypasses SOP
➡️ It can fully compromise user accounts

---

## 📚 Reference

MWR CyberSec Week 5 Assignment 

---

## 🏁 Final Thought

Mastering XSS = mastering **web exploitation fundamentals**

---
