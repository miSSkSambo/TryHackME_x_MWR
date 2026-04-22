# 🐧 Kenobi (Linux Exploitation)  
🔗 Link to the room: https://tryhackme.com/room/kenobi  

---

## 📌 Overview  
This room focuses on exploiting a Linux machine through:

- SMB enumeration  
- NFS mounting  
- Exploiting ProFTPD vulnerability  
- Privilege escalation using SUID and PATH manipulation  

---

## 🎯 Learning Objectives  
- Enumerate SMB shares  
- Identify vulnerable services  
- Exploit ProFTPD mod_copy vulnerability  
- Mount NFS shares  
- Perform privilege escalation via PATH manipulation  

---

## 🧠 Key Concepts  
- SMB Enumeration  
- NFS Mounting  
- ProFTPD Exploitation  
- SSH Key Access  
- SUID Binaries  
- PATH Variable Manipulation  
- Privilege Escalation  

---

## ✅ Questions and Answers  

### 🔹 Task 1: Deploy the Machine  

**Q:** Scan the machine with nmap, how many ports are open?  
**A:** 7  

---

### 🔹 Task 2: Enumerating Samba  

**Q:** How many SMB shares are found?  
**A:** 3  

**Q:** What file is found on the share?  
**A:** log.txt  

**Q:** What port is FTP running on?  
**A:** 21  

**Q:** What mount can we see?  
**A:** /var  

---

### 🔹 Task 3: Gain Initial Access (ProFTPD)  

**Q:** What is the version of ProFTPD?  
**A:** 1.3.5  

**Q:** How many exploits are available for this version?  
**A:** 4  

**Q:** What is Kenobi's user flag?  
**A:** d0b0f3f53b6caa532a83915e19224899  

---

### 🔹 Task 4: Privilege Escalation  

**Q:** Which SUID binary looks unusual?  
**A:** /usr/bin/menu  

**Q:** How many options does the binary show?  
**A:** 3  

**Q:** What is the root flag?  
**A:** 177b3cd8562289f37382721c28381f02  

---

## 🚀 Summary  

This room demonstrates a full exploitation chain:

1. **Enumeration**
   - Nmap scan  
   - SMB share discovery  
   - NFS enumeration  

2. **Initial Access**
   - Exploit ProFTPD mod_copy  
   - Extract SSH private key  
   - Login as user  

3. **Privilege Escalation**
   - Identify SUID binary  
   - Exploit PATH variable  
   - Gain root access  

---

## 🧠 Key Takeaway  

> Always check for misconfigured services and SUID binaries —  
> small misconfigurations can lead to full system compromise.

---

## 🏁 Skills Gained  
- Network Enumeration  
- Service Exploitation  
- Linux Privilege Escalation  
- NFS & SMB Usage  
- Real-world Attack Workflow  
