# 🔍 Redline 

---

link to the room: https://tryhackme.com/room/btredlinejoxr3d

---

## 📌 Overview

This room teaches how to use **Redline**, a tool developed by :contentReference[oaicite:0]{index=0}, for:

- Memory analysis  
- Incident response triage  
- IOC (Indicators of Compromise) hunting  

You learn how to:
- Collect endpoint data  
- Analyse system artifacts  
- Identify malicious activity  
- Perform IOC-based investigations  

---

# 🧪 FULL QUESTIONS & ANSWERS

---

## 🔹 Task 1: Introduction

**Q:** Which company created Redline?  
**A:** FireEye  

---

## 🔹 Task 2: Data Collection

**Q:** What data collection method takes the least amount of time?  
**A:** Standard Collector  

**Q:** You want to collect data based on known indicators (domains, hashes, etc.). Which method would you use?  
**A:** IOC Search Collector  

**Q:** What script is used to start data collection?  
**A:** RunRedlineAudit.bat  

**Q:** Where do you collect disk and volume data?  
**A:** Disk Enumeration  

**Q:** What is the default output filename?  
**A:** AnalysisSession1.mans  

---

## 🔹 Task 3: The Redline Interface

**Q:** Where can you view logged-in user information?  
**A:** System Information  

---

## 🔹 Task 4: Standard Collector Analysis

**Q:** What Operating System is detected?  
**A:** Windows Server 2019 Standard 17763  

**Q:** What suspicious scheduled task was created?  
**A:** MSOfficeUpdateFa.ke  

**Q:** What message did the intruder leave in the task?  
**A:** THM-p3R5IStENCe-m3Chani$m  

**Q:** What is the Event ID created by the attacker?  
**A:** 546  

**Q:** What is the Event message?  
**A:** Someone cracked my password. Now I need to rename my puppy-++-  

**Q:** What URL was used to download the file?  
**A:** https://wormhole.app/download-stream/gI9vQtChjyYAmZ8Ody0AuA  

**Q:** Where was the file downloaded?  
**A:** C:\Program Files (x86)\Windows Mail\SomeMailFolder\flag.txt  

**Q:** What message is inside the file?  
**A:** THM{600D-C@7cH-My-FR1EnD}  

---

## 🔹 Task 5: IOC Search Collector

**Q:** What is the actual filename of the keylogger?  
**A:** psylog.exe  

**Q:** What filename is it masquerading as?  
**A:** THM1768.exe  

**Q:** Who is the owner of the file?  
**A:** WIN-2DET5DP0NPT\charles  

**Q:** What is the file size?  
**A:** 35400  

**Q:** Where is the IOC file stored?  
**A:** C:\Users\charles\Desktop\Keylogger-IOCSearch\IOCs\keylogger.ioc  

---

## 🔹 Task 6: IOC Search Collector Analysis

**Q:** Full file path (with filename)?  
**A:** C:\Users\Administrator\AppData\Local\Temp\8eJv8w2id6IqN85dfC.exe  

**Q:** File path (without filename)?  
**A:** C:\Users\Administrator\AppData\Local\Temp\  

**Q:** File owner?  
**A:** BUILTIN\Administrators  

**Q:** Subsystem?  
**A:** Windows_CUI  

**Q:** Device path?  
**A:** \Device\HarddiskVolume2  

**Q:** SHA-256 hash?  
**A:** 57492d33b7c0755bb411b22d2dfdfdf088cbbfcd010e30dd8d425d5fe66adff4  

**Q:** Real filename (after hash lookup)?  
**A:** PsExec.exe  

---

## 🔹 Task 7: Endpoint Investigation

**Q:** What is the product name of the machine?  
**A:** Windows 7 Home Basic  

**Q:** What is the ransom note filename?  
**A:** _R_E_A_D___T_H_I_S___AJYG1O_.txt  

**Q:** What is the Windows Defender service DLL?  
**A:** MpSvc.dll  

**Q:** What ZIP file was downloaded?  
**A:** eb5489216d4361f9e3650e6a6332f7ee21b0bc9f3f3a4018c69733949be1d481.zip  

**Q:** What is the malicious executable?  
**A:** Endermanch@Cerber5.exe  

**Q:** What is its MD5 hash?  
**A:** fe1bc60a95b2c2d77cd5d232296a7fa4  

**Q:** What ransomware is this?  
**A:** Cerber  

---

## 🔹 Task 8: Conclusion

**Q:** Read the above  
**A:** No answer needed  

---

# 🚀 Summary

This room teaches practical **incident response and threat hunting** using Redline.

You performed:
- Memory triage  
- IOC-based detection  
- Malware identification  
- Ransomware investigation  

---

## ⚠️ Key Takeaways

- Redline provides quick triage vs deep tools like Volatility  
- Scheduled tasks are common persistence mechanisms  
- Event logs reveal attacker activity  
- File hashes are critical for malware identification  
- IOC accuracy is important to avoid false positives  

---

## 🔐 Important Concepts

- IOC (Indicators of Compromise)  
- Memory Analysis  
- Persistence (Scheduled Tasks)  
- Hash Analysis (MD5 / SHA256)  
- Timeline Investigation  

---

## 💡 Final Insight

Redline is powerful for:
➡️ Rapid incident response  
➡️ Threat hunting  
➡️ Endpoint compromise analysis  

It gives analysts a **high-level but actionable view** of attacks.  

---

## 📚 Reference

TryHackMe — Redline Room

---
