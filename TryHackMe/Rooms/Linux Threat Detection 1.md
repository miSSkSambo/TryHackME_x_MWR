# 🐧 Linux Threat Detection 1 

<p align="center">
  <img src="https://img.shields.io/badge/TryHackMe-Linux%20Threat%20Detection-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Difficulty-Medium-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-Detection%20%26%20SOC-green?style=for-the-badge" />
</p>

---

link to the room: https://tryhackme.com/room/linuxthreatdetection1

---
## 📌 Overview

This room focuses on **detecting attacks on Linux systems**, especially how attackers gain **Initial Access** and how defenders can identify this using logs.

It covers:

* SSH attacks
* Service exploitation
* Log analysis
* Process tree analysis

---

## 🎯 Learning Objectives

* Understand SSH risks and attacks
* Detect brute-force and compromised logins
* Analyze Linux logs (`auth.log`, `nginx`, `auditd`)
* Use process tree analysis to trace attacks
* Identify real-world attack patterns

---

## 🧠 Key Concepts

* SSH brute-force attacks
* Log analysis (`/var/log/auth.log`)
* Web exploitation detection
* Command injection
* Process tree analysis (`auditd`)
* Initial Access techniques (MITRE)

---

# 🧪 Walkthrough Summary

## 🔹 1. SSH Detection

* Check logs:

```bash
cat /var/log/auth.log | grep "sshd"
```

✔ Identify:

* First login
* Authentication method (key/password)

---

## 🔹 2. Brute Force Detection

Look for:

* Multiple failed logins
* Sudden successful login
* External IPs

---

## 🔹 3. Web Attack Detection

Check:

```bash
cat /var/log/nginx/access.log
```

✔ Indicators:

* Commands inside URL parameters
* `;whoami`, `;ls` → command injection

---

## 🔹 4. Process Tree Analysis

Trace suspicious commands:

```bash
ausearch -i -x whoami
```

✔ Follow:

* PID → PPID → Parent process
* Identify origin of attack

---

## 🔹 5. Advanced Detection

* Supply chain attacks
* Malicious scripts
* Fake packages

---

# ✅ FULL QUESTIONS & ANSWERS

---

## 🔹 Task 1

**Q:** I'm ready to start!
**A:** No answer needed

---

## 🔹 Task 2

**Q:** When did ubuntu first log in via SSH?
**A:** 2024-10-22

**Q:** Did ubuntu use SSH keys?
**A:** Yea

---

## 🔹 Task 3

**Q:** When did brute force start?
**A:** 2025-08-21

**Q:** Which users were targeted?
**A:** root, roy, sol, user

**Q:** Which IP breached root?
**A:** 91.224.92.79

---

## 🔹 Task 4

**Q:** Path to Python file accessed?
**A:** /opt/trypingme/main.py

**Q:** Flag inside file?
**A:** THM{i_am_vulnerable!}

---

## 🔹 Task 5

**Q:** PPID of whoami command?
**A:** 1018

**Q:** PID of vulnerable app?
**A:** 577

**Q:** Program used for reverse shell?
**A:** Python

---

## 🔹 Task 6

**Q:** Which technique is used when trusted app runs malicious commands?
**A:** Supply Chain Compromise

**Q:** Detection method for multiple attacks?
**A:** Process Tree Analysis

---

## 🔹 Task 7

**Q:** Let's continue!
**A:** No answer needed

---

# 🚀 Attack Flow Summary

1. SSH exposed → brute force
2. Credentials compromised
3. Web service exploited
4. Commands executed via injection
5. Reverse shell established
6. Process tree reveals origin

---

## ⚠️ Key Takeaways

* SSH is a major attack vector
* Weak passwords = easy compromise
* Logs are your first line of defense
* Web apps can expose full systems
* Process tree analysis is critical

---

## 💡 Final Insight

Linux attacks often start simple:

➡️ Weak SSH credentials
➡️ Exposed services
➡️ Poor input validation

Detection depends on:

✔ Log analysis
✔ Correlation
✔ Process tracing

---

## 📚 Reference

TryHackMe — Linux Threat Detection 1 

---
