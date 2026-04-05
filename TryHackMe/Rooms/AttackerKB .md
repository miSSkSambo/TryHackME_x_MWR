# 🔐 AttackerKB 

---
link to the room: https://tryhackme.com/room/attackerkb

---
## 📖 Overview

The **AttackerKB TryHackMe room** focuses on understanding how to **research, analyze, and exploit real-world vulnerabilities** using the :contentReference[oaicite:0]{index=0} platform.

It teaches you how attackers and defenders both:
- Investigate newly discovered vulnerabilities  
- Assess how dangerous they are  
- Find working exploits  
- Apply them in real-world scenarios  

---

## 🎯 What You Learn

### 🔍 Vulnerability Research
- Use AttackerKB to search for vulnerabilities  
- Understand community assessments and exploit insights  
- Identify affected versions and severity  

### 🧠 Threat Intelligence
- Learn how vulnerabilities are discovered (e.g. supply chain attacks)  
- Analyse real-world incidents and timelines  

### ⚔️ Exploitation
- Use :contentReference[oaicite:1]{index=1} to exploit vulnerabilities  
- Configure exploit modules correctly  
- Gain system access and escalate privileges  

### 🛡️ Defensive Insight
- Understand how defenders prioritize patching  
- Use vulnerability data to assess risk  

---

## 🧪 Scenario Summary

You act as an **attacker performing a black-box assessment**:
1. Scan a target machine  
2. Discover a vulnerable service (**Webmin**)  
3. Research the vulnerability using AttackerKB  
4. Exploit it using Metasploit  
5. Gain user and root access  

---

## ⚠️ Key Concept Highlight

### Supply Chain Attack
The vulnerability in this room is caused by a **malicious backdoor introduced into Webmin**, meaning:
- The software itself was compromised  
- Users installed a vulnerable version unknowingly  
- This allowed attackers to gain remote access  

---

## 📌 Task 1: I'm attacking what now?

**Q: Read the above and move onto task two!**  
**A:** No answer needed  

---

## 📌 Task 2: Discovering the Lay of the Land

**Q: What non-standard service is running on a high port?**  
**A:** Webmin  

**Q: What version is running?**  
**A:** 1.890  

**Q: What hostname is found in the certificate?**  
**A:** source  

---

## 📌 Task 3: Learning to Fly

**Q: Which version is vulnerable?**  
**A:** 1.890  

**Q: What type of attack is this?**  
**A:** Supply Chain  

**Q: When was Webmin informed of the 0day exploit?**  
**A:** August 17th 2019  

**Q: Metasploit module pull request number?**  
**A:** 12219  

---

## 📌 Task 4: Blasting Away

**Q: What option must be set to True?**  
**A:** ssl  

**Q: User flag?**  
**A:** THM{SUPPLY_CHAIN_COMPROMISE}  

**Q: Root flag?**  
**A:** THM{UPDATE_YOUR_INSTALL}  

---

## 📌 Task 5: Going Further

**Q: Read and continue learning**  
**A:** No answer needed  

---

## 🧠 Key Takeaways

- AttackerKB is a powerful tool for **vulnerability intelligence**
- Not all exploits are equal — context matters  
- Supply chain attacks are extremely dangerous  
- Always verify software sources and updates  
- Combining **research + exploitation tools** is critical in cybersecurity  

---



This repository documents the full walkthrough and answers for the **AttackerKB TryHackMe Room**.
