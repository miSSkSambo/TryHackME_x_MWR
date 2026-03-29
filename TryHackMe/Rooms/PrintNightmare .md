# 🖨️ PrintNightmare 

---

link to the room: https://tryhackme.com/room/printnightmarehpzqlp8

---

<p align="center">
  <img src="https://img.shields.io/badge/TryHackMe-PrintNightmare-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Difficulty-Medium-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-Windows%20Exploitation-blue?style=for-the-badge" />
</p>

---

## 📌 Overview

This room covers the **PrintNightmare vulnerability**, a critical Windows vulnerability affecting the **Print Spooler service**.

It includes:

* Exploitation (Offensive)
* Detection (Blue Team)
* Mitigation (Defensive)

### 🧠 What is PrintNightmare?

A vulnerability where:

> Attackers can execute arbitrary code with SYSTEM privileges via the Print Spooler service.

---

## 🎯 Learning Objectives

* Understand Print Spooler service
* Exploit PrintNightmare vulnerability
* Detect attacks using:

  * Windows Event Logs
  * Sysmon
  * Wireshark
* Apply mitigation techniques

---

## ⚠️ Vulnerabilities Covered

* CVE-2021-1675 (Local Privilege Escalation)
* CVE-2021-34527 (Remote Code Execution)

---

# 🧪 Walkthrough Summary

## 🔹 Exploitation Steps

1. Create malicious DLL using `msfvenom`
2. Setup Metasploit handler
3. Host DLL via SMB share
4. Run exploit script (`CVE-2021-1675.py`)
5. Gain Meterpreter session (SYSTEM)

---

## 🔹 Detection Techniques

* Monitor:

  * `spoolsv.exe` spawning processes
  * Suspicious DLLs in:

    ```
    C:\Windows\System32\spool\drivers\x64\3\
    ```
* Look for:

  * Event ID 808
  * Event ID 316
  * Event ID 7031

---

## 🔹 Mitigation

* Disable Print Spooler
* Apply Microsoft patches
* Use Group Policy restrictions

---

# ✅ FULL QUESTIONS & ANSWERS

---

## 🔹 Task 1

**Q:** Read the above
**A:** No answer needed

---

## 🔹 Task 2

**Q:** Where would you enable or disable Print Spooler Service?
**A:** Services

---

## 🔹 Task 3

**Q:** Provide the CVE that does NOT require local access
**A:** CVE-2021-34527

**Q:** What date was the CVE assigned?
**A:** 07/02/2021

---

## 🔹 Task 4

**Q:** What is the flag on Administrator Desktop?
**A:** THM{SiGBQPMkSvejvmQNEL}

---

## 🔹 Task 5

**Q:** First folder path for dropped DLL?
**A:** C:\Windows\System32\spool\drivers\x64\3\

**Q:** Function used to install printer drivers?
**A:** pcAddPrinterDriverEx()

**Q:** Tool used to scan vulnerable servers?
**A:** rpcdump.py

---

## 🔹 Task 6

**Q:** Dropped DLL + error code?
**A:** svch0st.dll,0x45A

**Q:** Event log + ID detecting DLL?
**A:** Microsoft-Windows-PrintService/Admin,808

**Q:** Service stop event details?
**A:** Service Control Manager,7031,1

**Q:** Attacker shell detection?
**A:** Microsoft-Windows-Sysmon/Operational,3,4747

**Q:** Attacker IP + hostname?
**A:** 10.10.210.100,ip-10-10-210-100.eu-west-1.compute.internal

**Q:** DLL path + creation time?
**A:** C:\Windows\System32\spool\drivers\x64\3\New\svch0st.dll,2021-08-13 17:33:37

---

## 🔹 Task 7

**Q:** Domain controller hostname?
**A:** WIN-1O0UJBNP9G7

**Q:** Local domain?
**A:** printnightmare.local

**Q:** Exploiting user account?
**A:** lowprivlarry

**Q:** Malicious DLL?
**A:** letmein.dll

**Q:** Attacker IP?
**A:** 10.10.124.236

**Q:** UNC path?
**A:** \10.10.124.236\sharez

**Q:** Encrypted protocol?
**A:** SMB3

---

## 🔹 Task 8

**Q:** Two ways to disable Print Spooler?
**A:** PowerShell,Group Policy

**Q:** Group Policy path?
**A:** Computer Configuration/Administrative Templates/Printers

**Q:** PowerShell command to check service?
**A:** Get-Service -Name Spooler

---

## 🔹 Task 9

**Q:** Read the above
**A:** No answer needed

---

# 🚀 Attack Flow Summary

1. Create malicious DLL
2. Setup listener
3. Host DLL via SMB
4. Execute exploit
5. Gain SYSTEM access
6. Detect via logs
7. Mitigate vulnerability

---

## ⚠️ Key Takeaways

* Print Spooler is enabled by default → high risk
* Remote exploitation makes it critical
* Detection requires log + network analysis
* Mitigation must include patching + disabling service

---

## 💡 Final Insight

PrintNightmare is dangerous because:

➡️ No local access required
➡️ SYSTEM-level compromise
➡️ Default Windows service

---

## 📚 Reference

TryHackMe — PrintNightmare Room 

---
