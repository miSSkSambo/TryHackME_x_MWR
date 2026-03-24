# ☁️ M365 Monitoring Basics 

---

link to the room: https://tryhackme.com/room/m365monitoringbasics

---

## 📌 Overview

This room introduces how **Microsoft Entra ID** and **Microsoft 365 (M365)** logs are used in modern SOC environments to investigate identity-based attacks.

You step into the role of a SOC analyst investigating:
- Multiple failed logins
- A successful compromise
- Suspicious activity in cloud services

The focus is on building an **attack timeline using logs**.

---

## 🎯 Learning Objectives

- Understand identity providers and cloud identity risks
- Learn how attackers target Entra ID accounts
- Analyse Entra ID Sign-in and Audit logs
- Investigate M365 activity logs
- Correlate logs to detect and understand attacks

---

## 🧠 Key Concepts

- **Identity Providers (IdP)**
- **Microsoft Entra ID (Azure AD)**
- **M365 Unified Audit Logs**
- **Authentication vs Authorization**
- **SOC Log Analysis**
- **Attack Timeline Correlation**
- **Cloud Identity Attacks**

---

# ✅ Questions and Answers

## 🔹 Task 1: Introduction

**Q:** Let's start!  
**A:** No answer needed  

---

## 🔹 Task 2: Identity Providers

**Q:** What type of application is Entra ID?  
**A:** Identity Provider  

**Q:** What type of identity is a server account?  
**A:** Device  

---

## 🔹 Task 3: Identities as the Target

**Q:** What authentication resource can prevent attackers from authenticating with only a stolen password?  
**A:** MFA  

**Q:** What can help us detect and monitor cloud identity threats?  
**A:** Logs  

---

## 🔹 Task 4: Entra ID Sign-in Logs

**Q:** What is the email address of the compromised identity?  
**A:** allan.smith@finegalo.thm  

**Q:** What is the IP address used by the attacker?  
**A:** 2804:2488:7082:a4c0:fd97:b11b:9895:49c0  

**Q:** What is the city of the IP address used by the attacker?  
**A:** Belo Horizonte  

**Q:** When was the first successful sign-in after failed attempts?  
**A:** 2/11/26 6:16:53.000 PM  

**Q:** What is the first application accessed after Office Home?  
**A:** One Outlook Web  

---

## 🔹 Task 5: Entra ID Audit Logs

**Q:** What was the first change made by the attacker?  
**A:** User started security info registration  

**Q:** What activity reveals all modified properties in a user?  
**A:** Update user  

**Q:** What is the second change made in the account?  
**A:** Reset password (self-service)  

---

## 🔹 Task 6: M365 Introduction

**Q:** Let's explore M365 logs!  
**A:** No answer needed  

---

## 🔹 Task 7: M365 Audit Logs

**Q:** What is the application used by the attacker?  
**A:** Exchange  

**Q:** What change did the attacker make in the application?  
**A:** New-InboxRule  

**Q:** What is the subject of the email sent by the attacker?  
**A:** URGENT: Approval for new internal VPN Access  

**Q:** When did the attacker access the response?  
**A:** 2/11/26 6:20:09.000 PM  

**Q:** Which path was the response stored in?  
**A:** \Deleted Items  

---

## 🔹 Task 8: Conclusion

**Q:** Ready to explore Entra ID threats!  
**A:** No answer needed  

---

## 🚀 Summary

This room demonstrates how **cloud identity attacks are investigated using logs**.

Key takeaways:
- Entra ID logs show **who logged in and from where**
- Audit logs reveal **what changes attackers made**
- M365 logs show **what attackers did after access**
- Correlating logs builds a **complete attack timeline**

---

## 🔐 Investigation Flow

1. **Sign-in Logs** → Detect suspicious login  
2. **Audit Logs** → Identify account changes  
3. **M365 Logs** → Analyse attacker actions  

---

## ⚠️ Key Insight

Modern attacks often:
- Use **valid credentials**
- Leave **no malware traces**
- Can only be detected through **log analysis**

---
