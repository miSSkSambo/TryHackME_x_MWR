# 💥 Follina MSDT 


--- 
link to the room: https://tryhackme.com/room/follinamsdt

---
<p align="center">
  <img src="https://img.shields.io/badge/TryHackMe-Follina-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Difficulty-Intermediate-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-Windows%20RCE-blue?style=for-the-badge" />
</p>

---

## 📌 Overview

This room explores **CVE-2022-30190 (Follina)** — a critical Windows vulnerability affecting:

* Microsoft Office
* Microsoft Support Diagnostic Tool (MSDT)

✔ Allows **Remote Code Execution (RCE)**
✔ Requires **no macros**
✔ Can be triggered with **zero-click (preview pane)**

---

## 🎯 Learning Objectives

* Understand MSDT service
* Learn how Follina works
* Exploit the vulnerability
* Perform threat hunting
* Detect malicious activity
* Apply mitigation techniques

---

## 🧠 Key Concepts

* Remote Code Execution (RCE)
* OLE Objects (Word documents)
* PowerShell injection
* Process tree analysis
* Event log analysis
* Threat hunting
* Detection & remediation

---

# 🧪 WALKTHROUGH

---

## 🔹 1. Vulnerability Background

✔ First discovered:

```id="m31y2k"
2020
```

✔ Researcher:

```id="r2slbz"
Benjamin Altpeter
```

✔ First APT reporting exploitation:

```id="s6z2zy"
Shadowchasing1
```

---

## 🔹 2. MSDT Overview

✔ Purpose:

* Collect diagnostic data

✔ Requirement:

```id="3dl2q8"
Passkey
```

---

## 🔹 3. Exploitation

### ⚡ How it works:

1. Malicious Word document (.docx)
2. External OLE reference → malicious HTML
3. HTML triggers:

```id="ksl1vd"
ms-msdt
```

4. Executes PowerShell payload

---

### 🧪 Indicators of Compromise

✔ Application executed:

```id="b8b6rq"
win32calc.exe
```

✔ Malicious document:

```id="6n8zw1"
05-2022-0438.doc
```

✔ Reverse shell binary:

```id="i8j0t1"
netcat
```

✔ Download location:

```id="k6p4r7"
C:\Windows\Tasks
```

---

## 🔹 4. Process Analysis

✔ Parent processes:

```id="vczc7r"
WINWORD.EXE
sdiagnhost.exe
```

✔ Child processes:

```id="9q7v7o"
msdt.exe
conhost.exe
```

✔ Zero-click indicator:

```id="r1yqsm"
prevhost.exe
```

---

## 🔹 5. Detection (Threat Hunting)

✔ Event ID:

```id="o2v9yy"
4688 (Process Creation)
```

✔ Suspicious indicator:

```id="7hj2zc"
PowerShell execution via WINWORD
```

✔ Encoded string:

```id="n0m8hc"
Y2FsYw== → calc
```

✔ Encoding:

```id="9sm7ml"
base64
```

✔ Parent of calc:

```id="xqk6pz"
sdiagnhost.exe
```

✔ Diagnostic path:

```id="zz4w4w"
C:\Windows\Diagnostics\Index
```

---

## 🔹 6. Remediation

### ✔ Patch

* June 2022 Windows Update

---

### ✔ Disable MSDT Protocol

```bash id="d3p3z1"
reg export HKEY_CLASSES_ROOT\ms-msdt ms-msdt_backup
reg delete HKEY_CLASSES_ROOT\ms-msdt /f
```

---

### ✔ Attack Surface Reduction

* Block Office spawning child processes

---

### ✔ Error Indicator

```id="r7y5ny"
You'll need a new app to open this ms-msdt
```

---

# ✅ FULL QUESTIONS & ANSWERS

---

## 🔹 Task 1

**Q:** Enjoy the room
**A:** No answer needed

---

## 🔹 Task 2

**Q:** Year vulnerability discovered?
**A:** 2020

**Q:** Author of thesis?
**A:** Benjamin Altpeter

**Q:** APT group?
**A:** Shadowchasing1

---

## 🔹 Task 3

**Q:** Required for MSDT support?
**A:** Passkey

---

## 🔹 Task 4

**Q:** App executed on compromise?
**A:** win32calc.exe

**Q:** Malicious doc name?
**A:** 05-2022-0438.doc

**Q:** Reverse shell binary?
**A:** netcat

**Q:** Download location?
**A:** C:\Windows\Tasks

**Q:** Other parent process?
**A:** sdiagnhost.exe

**Q:** Child of WINWORD?
**A:** msdt.exe

**Q:** Child of other parent?
**A:** conhost.exe

**Q:** Zero-click indicator?
**A:** prevhost.exe

---

## 🔹 Task 5

**Q:** Encoding used?
**A:** base64

**Q:** Parent of calc.exe?
**A:** sdiagnhost.exe

**Q:** Diagnostic path?
**A:** C:\Windows\Diagnostics\Index

---

## 🔹 Task 6

**Q:** Error message shown?
**A:** You'll need a new app to open this ms-msdt

---

## 🔹 Task 7

**Q:** Completed
**A:** No answer needed

---

# 🚀 Attack Flow Summary

1. Deliver malicious document
2. Word loads external HTML
3. HTML triggers MSDT
4. PowerShell executes payload
5. Code execution achieved
6. Reverse shell established

---

## ⚠️ Key Takeaways

* No macros required → highly dangerous
* Can be triggered via preview pane (zero-click)
* Uses legitimate Windows tools (LOLBins)
* Difficult to detect without proper logging

---

## 💡 Final Insight

Follina is powerful because:

➡️ Uses trusted Microsoft components
➡️ Requires minimal user interaction
➡️ Bypasses traditional defenses

---

## 📚 Reference

TryHackMe — Follina MSDT 

---

## 🏁 Final Thought

This vulnerability shows how:

➡️ Legitimate tools can be weaponized
➡️ Detection relies on behavioral analysis
➡️ Patching and monitoring are critical

---
