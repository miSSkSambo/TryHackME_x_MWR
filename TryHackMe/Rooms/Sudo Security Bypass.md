# 🔓 Sudo Security Bypass (CVE-2019-14287)

---

Link to the room: https://tryhackme.com/room/sudovulnsbypass

---

## 📌 Overview

This room explores **CVE-2019-14287**, a privilege escalation vulnerability affecting vulnerable versions of the Unix **Sudo** program.

The vulnerability allows a user who is explicitly denied root access through sudoers configuration to bypass the restriction and execute commands as **root**.

By abusing how Sudo handles the UID value **-1**, an attacker can gain full administrative privileges on the target system.

---

## 🎯 Learning Objectives

* Understand how Sudo works
* Learn about sudoers configurations
* Identify vulnerable Sudo versions
* Exploit CVE-2019-14287
* Escalate privileges to root
* Understand mitigation strategies

---

## 🧠 Key Concepts

* **Sudo**
* **sudoers Configuration**
* **User IDs (UIDs)**
* **Privilege Escalation**
* **Root Access**
* **Linux Security**
* **CVE-2019-14287**
* **Misconfigured Permissions**

---

# ✅ Questions and Answers

## 🔹 Task 1: Deploy!

**Q:** Deploy the machine and connect via SSH
**A:** No answer needed

---

## 🔹 Task 2: Security Bypass

**Q:** What command are you allowed to run with sudo?
**A:** /bin/bash

**Q:** What is the flag in /root/root.txt?
**A:** THM{l33t_s3cur1ty_bypass}

---

## ⚠️ Key Takeaways

* Sudo misconfigurations can lead to privilege escalation.
* UID values are critical when evaluating access controls.
* CVE-2019-14287 allows root access despite explicit sudo restrictions.
* Always verify the version of Sudo running on a system.
* Security updates are essential for preventing privilege escalation attacks.

---

## 🔐 Mitigation

* Upgrade Sudo to version **1.8.28** or later.
* Audit sudoers configurations regularly.
* Apply security patches promptly.
* Restrict unnecessary sudo permissions.
* Monitor privilege escalation attempts.

