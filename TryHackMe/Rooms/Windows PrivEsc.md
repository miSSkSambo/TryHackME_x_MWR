# 🪟 Windows Privilege Escalation 

---

link to the room: https://tryhackme.com/room/windows10privesc

---
## 📌 Overview

This room focuses on **Windows Privilege Escalation techniques** using an intentionally vulnerable machine.

You practice:
- Service exploitation  
- Registry abuse  
- Credential harvesting  
- Token impersonation  
- Scheduled tasks abuse  

---

# 🧪 FULL QUESTIONS & ANSWERS

---

## 🔹 Task 1: Deploy the Vulnerable Windows VM

**Q:** Deploy the Windows VM and login using the "user" account.  
**A:** No answer needed  

---

## 🔹 Task 2: Generate a Reverse Shell Executable

**Q:** Generate a reverse shell executable and transfer it to the Windows VM. Check that it works!  
**A:** No answer needed  

---

## 🔹 Task 3: Service Exploits — Insecure Service Permissions

**Q:** What is the original BINARY_PATH_NAME of the daclsvc service?  
**A:** C:\Program Files\DACL Service\daclservice.exe  

---

## 🔹 Task 4: Service Exploits — Unquoted Service Path

**Q:** What is the BINARY_PATH_NAME of the unquotedsvc service?  
**A:** C:\Program Files\Unquoted Path Service\Common Files\unquotedpathservice.exe  

---

## 🔹 Task 5: Service Exploits — Weak Registry Permissions

**Q:** Read and follow along with the above.  
**A:** No answer needed  

---

## 🔹 Task 6: Service Exploits — Insecure Service Executables

**Q:** Read and follow along with the above.  
**A:** No answer needed  

---

## 🔹 Task 7: Registry — AutoRuns

**Q:** Read and follow along with the above.  
**A:** No answer needed  

---

## 🔹 Task 8: Registry — AlwaysInstallElevated

**Q:** Read and follow along with the above.  
**A:** No answer needed  

---

## 🔹 Task 9: Passwords — Registry

**Q:** What was the admin password you found in the registry?  
**A:** password123  

---

## 🔹 Task 10: Passwords — Saved Creds

**Q:** Read and follow along with the above.  
**A:** No answer needed  

---

## 🔹 Task 11: Passwords — Security Account Manager (SAM)

**Q:** What is the NTLM hash of the admin user?  
**A:** a9fdfa038c4b75ebc76dc855dd74f0da  

---

## 🔹 Task 12: Passwords — Passing the Hash

**Q:** Read and follow along with the above.  
**A:** No answer needed  

---

## 🔹 Task 13: Scheduled Tasks

**Q:** Read and follow along with the above.  
**A:** No answer needed  

---

## 🔹 Task 14: Insecure GUI Apps

**Q:** Read and follow along with the above.  
**A:** No answer needed  

---

## 🔹 Task 15: Startup Apps

**Q:** Read and follow along with the above.  
**A:** No answer needed  

---

## 🔹 Task 16: Token Impersonation — Rogue Potato

**Q:** Name one user privilege that allows this exploit to work.  
**A:** SeImpersonatePrivilege  

**Q:** Name the other user privilege that allows this exploit to work.  
**A:** SeAssignPrimaryTokenPrivilege  

---

## 🔹 Task 17: Token Impersonation — PrintSpoofer

**Q:** Read and follow along with the above.  
**A:** No answer needed  

---

## 🔹 Task 18: Privilege Escalation Scripts

**Q:** Do all tools identify the techniques used in this room?  
**A:** No answer needed  

---

# 🚀 Summary

This room demonstrates multiple real-world privilege escalation techniques on Windows systems.

---

## ⚠️ Key Takeaways

- Misconfigured services = easy SYSTEM access  
- Registry misconfigurations can be exploited  
- Stored credentials are dangerous  
- Scheduled tasks can be abused for persistence  
- Token privileges enable powerful escalation  

---

## 🔐 Key Techniques Covered

- Service misconfigurations  
- Unquoted service paths  
- Weak file/registry permissions  
- AlwaysInstallElevated abuse  
- Credential dumping (SAM)  
- Pass-the-hash  
- Token impersonation (Rogue Potato, PrintSpoofer)  

---

## 💡 Final Insight

Privilege escalation in Windows often comes down to:

➡️ Misconfigurations  
➡️ Poor permissions  
➡️ Credential exposure  

Mastering enumeration is the key to finding these weaknesses.

---

## 📚 Reference

TryHackMe — Windows PrivEsc 

---
