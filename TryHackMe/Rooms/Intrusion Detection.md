# 🚨 Intrusion Detection

---
link to the room: https://tryhackme.com/room/idsevasion

---

## 📌 Overview

This room introduces **Intrusion Detection Systems (IDS)** and how attackers use **evasion techniques** to avoid detection.

You perform a full attack chain while interacting with:
- **Suricata (NIDS)**
- **Wazuh (HIDS)**

The goal is to understand:
- How IDS detect attacks
- How attackers evade detection
- Trade-offs between stealth and information gathering

---

## 🎯 Learning Objectives

- Understand IDS types and detection methods
- Learn differences between NIDS and HIDS
- Perform reconnaissance with evasion
- Use tools like Nmap and Nikto stealthily
- Exploit vulnerabilities and escalate privileges
- Establish persistence while avoiding detection

---

## 🧠 Key Concepts

- **IDS (Intrusion Detection System)**
- **NIDS vs HIDS**
- **Signature-based vs Anomaly-based detection**
- **Cyber Kill Chain**
- **Reconnaissance & Evasion**
- **Privilege Escalation**
- **Persistence Techniques**
- **OSINT (Open Source Intelligence)**

---

# ✅ Questions and Answers

## 🔹 Task 1: Introduction

**Q:** Deploy machine and register  
**A:** No answer needed  

---

## 🔹 Task 2: Intrusion Detection Basics

**Q:** Which IDS method uses rules?  
**A:** signature-based detection  

---

## 🔹 Task 3: NIDS

**Q:** Which protocol reduces NIDS effectiveness?  
**A:** TLS  

---

## 🔹 Task 4: Reconnaissance & Evasion

**Q:** What severity scale does Suricata use?  
**A:** 1-3  

**Q:** How many services does Nmap detect with -sV?  
**A:** 3  

---

## 🔹 Task 5: Further Reconnaissance

**Q:** What interesting path does Nikto find?  
**A:** /login  

**Q:** What value toggles DoS in Nikto?  
**A:** 6  

**Q:** Which flags modify request spacing?  
**A:** 6,A,B  

---

## 🔹 Task 6: OSINT

**Q:** Grafana version?  
**A:** 8.2.5  

**Q:** Vulnerable CVE?  
**A:** CVE-2021-43798  

**Q:** Which site can reveal services?  
**A:** shodan  

**Q:** Google search for PDFs?  
**A:** site:example.com filetype:pdf  

---

## 🔹 Task 7: Rulesets

**Q:** Grafana admin password?  
**A:** GraphingTheWorld32  

**Q:** Can we access server directly?  
**A:** yay  

**Q:** Which IDS detects /etc/shadow exploit?  
**A:** Suricata  

---

## 🔹 Task 8: HIDS

**Q:** HTTP 400 errors fall under which category?  
**A:** web  

---

## 🔹 Task 9: Privilege Escalation Recon

**Q:** Which tool reveals escalation vector?  
**A:** docker  

**Q:** Severity of linPEAS alert?  
**A:** 5  

---

## 🔹 Task 10: Privilege Escalation

**Q:** Root flag?  
**A:** {SNEAK_ATTACK_CRITICAL}  

---

## 🔹 Task 11: Persistence

**Q:** Establish persistence via Docker  
**A:** No answer needed  

---

## 🔹 Task 12: Conclusion

**Q:** Read the above  
**A:** No answer needed  

---

## 🚀 Summary

This room demonstrates how attackers:
- Perform reconnaissance
- Evade detection systems
- Exploit vulnerabilities
- Escalate privileges
- Maintain persistence

While defenders:
- Use NIDS (Suricata) to monitor network traffic
- Use HIDS (Wazuh) to monitor system activity

---

## ⚠️ Key Takeaways

- **NIDS** detects network traffic but struggles with encryption (TLS)
- **HIDS** detects system-level activity (logs, files, processes)
- Evasion reduces detection but also reduces information gathered
- Aggressive scans = more detection
- OSINT is stealthy and highly effective

---

## 🔐 Detection vs Evasion Trade-off

| Approach        | Detection Risk | Information Gain |
|----------------|--------------|----------------|
| Aggressive Scan | High         | High           |
| Stealth Scan    | Low          | Low            |
| OSINT           | Very Low     | Medium         |

---

## 💡 Key Insight

Perfect evasion is rare — attackers often aim for **low-severity alerts** rather than complete invisibility.

---
