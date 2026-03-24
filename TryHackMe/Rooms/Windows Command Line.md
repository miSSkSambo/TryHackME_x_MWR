# 💻 Windows Command Line

---

link to the room: https://tryhackme.com/room/windowscommandline

---
## 📌 Overview

This room introduces the **Windows Command Prompt (cmd.exe)** and teaches how to efficiently interact with a system using the command line instead of a graphical interface.

You learn how to:
- Retrieve system information
- Troubleshoot network issues
- Manage files and directories
- Monitor and control processes

---

## 🎯 Learning Objectives

- Understand the purpose of the Windows CLI
- Display system and OS information
- Perform network troubleshooting
- Manage files and directories
- Monitor and control running processes

---

## 🧠 Key Concepts

- **Command Prompt (cmd.exe)**
- **System Information Commands**
- **Network Troubleshooting Tools**
- **File & Directory Management**
- **Process Management**
- **Automation & Efficiency**

---

# ✅ Questions and Answers

## 🔹 Task 1: Introduction

**Q:** What is the default command line interpreter in Windows?  
**A:** cmd.exe  

---

## 🔹 Task 2: Basic System Information

**Q:** What is the OS version of the Windows VM?  
**A:** 10.0.20348.2655  

**Q:** What is the hostname of the Windows VM?  
**A:** WINSRV2022-CORE  

---

## 🔹 Task 3: Network Troubleshooting

**Q:** Which command shows the MAC address?  
**A:** ipconfig /all  

**Q:** What service is listening on port 135?  
**A:** RpcSs  

**Q:** What service is listening on port 3389?  
**A:** TermService  

---

## 🔹 Task 4: File and Disk Management

**Q:** What are the file contents in C:\Treasure\Hunt?  
**A:** THM{CLI_POWER}  

---

## 🔹 Task 5: Task and Process Management

**Q:** Command to find processes related to notepad.exe?  
**A:** tasklist /FI "imagename eq notepad.exe"  

**Q:** Command to kill process with PID 1516?  
**A:** taskkill /PID 1516  

---

## 🔹 Task 6: Conclusion

**Q:** Command to restart a system?  
**A:** shutdown /r  

**Q:** Command to abort a shutdown?  
**A:** shutdown /a 

---

## 🚀 Summary

This room shows how powerful the **Windows Command Line** can be.

Key takeaways:
- CLI is faster and more efficient than GUI
- Useful for **automation and remote management**
- Essential for **cybersecurity and system administration**

---

## ⚡ Useful Commands Recap

- `systeminfo` → View system details  
- `ipconfig` → Network configuration  
- `ping` → Check connectivity  
- `netstat` → View connections  
- `dir` → List files  
- `cd` → Navigate directories  
- `tasklist` → View processes  
- `taskkill` → Kill processes  

---

## ⚠️ Key Insight

Mastering the command line:
- Saves time
- Improves efficiency
- Is essential for **ethical hacking, SOC roles, and IT administration**

---
