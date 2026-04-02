# 🛡️ Incident Response — Preparation Phase 


---

link to the room: https://tryhackme.com/room/preparation

---
<p align="center">
  <img src="https://img.shields.io/badge/TryHackMe-Incident%20Response-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Phase-Preparation-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-Blue%20Team-yellow?style=for-the-badge" />
</p>

---

## 📌 Overview

This room focuses on the **Preparation phase of Incident Response (IR)** — ensuring an organisation is ready to detect and respond to cyber incidents effectively.

It covers:

* Incident response fundamentals
* People, processes, and technology
* Documentation and policies
* Logging and visibility
* Detection readiness

---

## 🎯 Learning Objectives

* Understand incident response concepts
* Differentiate events vs incidents
* Learn IR lifecycle phases
* Prepare people, policies, and tools
* Configure logging and visibility
* Improve detection readiness

---

## 🧠 Key Concepts

* Incident Response (IR) lifecycle
* Event vs Incident
* CSIRT teams
* Chain of custody
* Asset inventory
* Logging & SIEM
* Visibility & monitoring

---

# 🧪 WALKTHROUGH

---

## 🔹 1. Incident Response Basics

✔ Definitions:

* **Event** → Observed activity
* **Incident** → Security violation

✔ IR Phases:

1. Preparation
2. Identification
3. Analysis
4. Containment
5. Eradication
6. Recovery & Lessons Learned

---

## 🔹 2. People & Documentation

### 👥 CSIRT Team

* Cyber Security Incident Response Team
* Includes: technical, legal, business roles

---

### 📄 Documentation

* Policies
* Communication plans
* Incident response plans (IRP)
* Playbooks
* Chain of custody

---

## 🔹 3. Technology Preparation

### 🗂️ Asset Inventory

Example:

* Servers
* Applications
* IP addresses

---

### 🧰 Tools

* EDR
* DLP
* IDS/IPS
* SIEM
* Anti-malware

---

### 🎒 Jump Bag

✔ Contains:

* Forensic tools
* Storage devices
* Cables/adapters
* IR documentation

---

## 🔹 4. Visibility

### 📊 Log Types

* Event logs
* Audit logs
* Error logs
* Debug logs

---

### 📂 Log Sources

* Network devices
* Firewalls
* Systems
* Applications

---

### 🔍 SIEM

* Central log collection
* Correlation & analysis

---

## 🔹 5. Practical Setup

✔ Enable Windows Event Logs

✔ Registry fix:

```bash
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\EventLog\start = 2
```

✔ Test logging using Atomic Red Team

---

# ✅ FULL QUESTIONS & ANSWERS

---

## 🔹 Task 1

**Q:** Ready to prepare
**A:** No answer needed

---

## 🔹 Task 2

**Q:** Observed occurrence?
**A:** Event

**Q:** Violation of security?
**A:** Incident

**Q:** Phase for procedures?
**A:** Preparation

**Q:** Phase for recovery?
**A:** Recovery and Lessons Learned

---

## 🔹 Task 3

**Q:** Team handling incidents?
**A:** cyber security incident response team

**Q:** Evidence tracking document?
**A:** chain of custody documents

---

## 🔹 Task 4

**Q:** Incident response toolkit?
**A:** Jump bag

---

## 🔹 Task 5

**Q:** Event ID for file creation?
**A:** 11

**Q:** Default security level?
**A:** Unrestricted

**Q:** Audit logon events setting?
**A:** Failure

---

## 🔹 Task 6

**Q:** Completed
**A:** No answer needed

---

# 🚀 Incident Response Flow

1. Prepare systems and team
2. Monitor logs and alerts
3. Identify suspicious activity
4. Analyse scope
5. Contain attack
6. Eradicate threat
7. Recover systems

---

## ⚠️ Key Takeaways

* Preparation is the most critical IR phase
* Logs provide visibility into attacks
* CSIRT ensures coordinated response
* Documentation improves response speed
* SIEM enables centralized detection

---

## 💡 Final Insight

Incident response starts **before** an attack:

➡️ Prepared teams respond faster
➡️ Logs = visibility
➡️ Policies = consistency

---

## 📚 Reference

TryHackMe — Preparation Room 

---

## 🏁 Final Thought

Strong preparation = strong defense

---
