# 💥 DLL Hijacking (Invoke-PrintDemon) 

---

link to the room: https://tryhackme.com/room/dllhijacking

---

## 📌 Overview

This room demonstrates **DLL Hijacking** and **Privilege Escalation** using the **Invoke-PrintDemon** technique.

It combines:
- **Faxhell DLL Hijacking**
- **PrintDemon exploit (CVE-2020-1048)**

to escalate privileges from a low-level user to **SYSTEM**.

---

## 🎯 Learning Objectives

- Understand DLL hijacking attacks
- Learn how Windows services load DLLs
- Exploit Print Spooler vulnerabilities
- Use Empire and Evil-WinRM
- Perform privilege escalation to SYSTEM
- Achieve persistence on a target machine

---

## 🧠 Key Concepts

- **DLL Hijacking**
- **CVE-2020-1048 (Print Spooler vulnerability)**
- **Fax Service Exploitation (Faxhell)**
- **Privilege Escalation**
- **Empire Framework**
- **Evil-WinRM**
- **Persistence via Registry**
- **SYSTEM-level Access**

---

# ✅ Questions and Answers

## 🔹 Task 1: Overview of DLL Hijacking

**Q:** Read the above  
**A:** No answer needed  

---

## 🔹 Task 2: Install Tools

**Q:** Empire and Evil-WinRM successfully installed  
**A:** No answer needed  

---

## 🔹 Task 3: Windows Remote Management (WinRM)

**Q:** Successfully connected to the VM  
**A:** No answer needed  

---

## 🔹 Task 4: Launch Empire Agent

**Q:** Created HTTP Listener  
**A:** No answer needed  

**Q:** Generated Multi/Launcher Stager  
**A:** No answer needed  

---

## 🔹 Task 5: Deploy an Agent

**Q:** Stager successfully connects back  
**A:** No answer needed  

---

## 🔹 Task 6: Spawn as a New Process

**Q:** Which process may work with psinject?  
**A:** explorer  

---

## 🔹 Task 7: System Check

**Q:** What is the Windows build number?  
**A:** 1903  

---

## 🔹 Task 8: Invoke-PrintDemon

**Q:** Successfully created print job and wrote launcher  
**A:** No answer needed  

---

## 🔹 Task 9: Network Persistence

**Q:** What DLL is written to System32?  
**A:** ualapi.dll  

---

## 🔹 Task 10: Bonus — Find Other Users

**Q:** What is the other user?  
**A:** John  

---

## 🔹 Task 11: Bonus — Steal Credentials

**Q:** What is the other user’s password?  
**A:** 1q2w3e!Q@W#E1q2w3e 
---

## 🔹 Task 12: Conclusion

**Q:** #HackThePlanet  
**A:** No answer needed  

---

## 🚀 Summary

This room demonstrates a **real-world privilege escalation attack chain**:

1. Gain initial access via **WinRM**
2. Deploy an **Empire agent**
3. Use **Print Spooler vulnerability (CVE-2020-1048)**
4. Perform **DLL Hijacking**
5. Achieve **SYSTEM-level access**
6. Establish **persistence**

---

## ⚠️ Key Takeaways

- Services running as SYSTEM can be abused via DLL hijacking  
- Misconfigured or vulnerable services = **privilege escalation paths**  
- Print Spooler is a **common attack vector**  
- Restarting services can trigger exploits  

---

## 🔐 Mitigation

- Patch systems (especially Print Spooler vulnerabilities)
- Restrict write access to system directories
- Monitor suspicious DLL loads
- Disable unnecessary services (Fax, Print Spooler if not needed)
- Use endpoint detection tools (EDR)

---
