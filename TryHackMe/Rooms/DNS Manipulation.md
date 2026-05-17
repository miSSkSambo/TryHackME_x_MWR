# 🛡️ DNS Manipulation 

🔗 **Room Link:** https://tryhackme.com/room/dnsmanipulation

---

# 📖 Overview

This room focuses on how attackers abuse the **Domain Name System (DNS)** for offensive cybersecurity operations.

The room demonstrates techniques used to:
- Exfiltrate sensitive data through DNS queries
- Infiltrate malicious payloads into a network
- Tunnel protocols such as HTTP through DNS
- Bypass firewalls and network monitoring systems

You will also learn:
- How DNS works internally
- DNS hierarchy and root servers
- Common DNS record types
- DNS packet analysis
- DNS tunneling techniques

The room includes practical demonstrations and exercises using:
- Python scripts
- Wireshark
- tshark
- iodine
- nslookup
- dig

---

# 🎯 Learning Objectives

- Understand DNS fundamentals
- Learn common DNS record types
- Understand DNS exfiltration techniques
- Understand DNS infiltration techniques
- Learn how DNS tunneling works
- Capture and analyze DNS traffic
- Understand covert communication channels

---

# 🧠 Key Concepts

- DNS
- DNS Records
- TXT Records
- PTR Records
- DNS Zones
- Root Servers
- DNS Exfiltration
- DNS Infiltration
- DNS Tunneling
- Base64 Encoding
- Base58 Encoding
- Wireshark
- tshark
- iodine
- HTTP over DNS

---

# ✅ Questions and Answers

---

# 🔹 Task 1: Introduction

## 📖 Summary

This task introduces:
- DNS lookups
- DNS exfiltration
- DNS infiltration
- DNS tunneling

It explains how attackers can abuse DNS traffic for covert communication and data transfer.

---

### Q: Read the above
**A:** No answer needed

---

# 🔹 Task 2: Installation

## 📖 Summary

This task covers installation of:
- Python modules
- iodine
- Wireshark
- tshark

Required repositories and tools:
- `dns-exfil-infil`
- `iodine`

---

### Q: Ready!
**A:** No answer needed

---

# 🔹 Task 3: [Setup] Custom Public DNS Server

## 📖 Summary

This task explains how to:
- Configure a public DNS server
- Use a public domain name
- Prepare an Out-of-Band (OOB) exfiltration environment

---

### Q: Read the above.
**A:** No answer needed

---

# 🔹 Task 4: What is DNS?

## 📖 Summary

This section explains:
- DNS hierarchy
- Root name servers
- DNS zones
- DNS lookups
- FQDN resolution
- DNS record types

It also explains:
- A Records
- AAAA Records
- TXT Records
- PTR Records

---

### Q: If you were on Windows, what command could you use to query a txt record for 'youtube.com'?
**A:** `nslookup -type=txt youtube.com`

---

### Q: If you were on Linux, what command could you use to query a txt record for 'facebook.com'?
**A:** `dig facebook.com TXT`

---

### Q: AAAA stores what type of IP Address along with the hostname?
**A:** `IPv6`

---

### Q: Maximum characters for a DNS TXT Record is 256. (Yay/Nay)
**A:** `Nay`

---

### Q: What DNS Record provides a domain name in reverse-lookup?
**A:** `PTR`

---

### Q: What would the reverse-lookup be for the following IPv4 Address? (192.168.203.2)
**A:** `2.203.168.192.in-addr.arpa`

---

# 🔹 Task 5: What is DNS Exfiltration?

## 📖 Summary

This section explains:
- DNS-based data theft
- Covert data transfer through DNS queries
- Malware-based DNS exfiltration
- Why DNS traffic is difficult to detect

Attackers can hide encoded data inside DNS queries sent to rogue DNS servers.

---

### Q: What is the maximum length of a DNS name? (Length includes dots!)
**A:** `253`

---

# 🔹 Task 6: DNS Exfiltration - Demo

## 📖 Summary

This section demonstrates:
- Exfiltrating data using DNS queries
- Encoding files using:
  - Base64
  - Base58
- Capturing traffic with Wireshark
- Reconstructing exfiltrated files

Python scripts used:
- `packety.py`
- `packetyGrabber.py`

---

### Q: Read the above.
**A:** No answer needed

---

# 🔹 Task 7: DNS Exfiltration - Practice

## 📖 Summary

This task provides practical challenges involving:
- DNS traffic analysis
- Packet captures
- Decoding exfiltrated data
- Identifying suspicious DNS traffic

---

### Q: ~/challenges/exfiltration/orderlist/

ORDER-ID: 1

What is the Transaction name? (Type it as you see it)
**A:** `Network Equip.`

---

### Q: ~/challenges/exfiltration/orderlist/

TRANSACTION: Firewall

How much was the Firewall? (Without the $)
**A:** `2500`

---

### Q: ~/challenges/exfiltration/identify/

Which file contains suspicious DNS queries?
**A:** `cap3.pcap`

---

### Q: ~/challenges/exfiltration/identify/

Enter the plain-text after you have decoded the data using packetyGrabber.py found in ~/dns-exfil-infil/ folder.
**A:** `administrator:s3cre7P@ssword`

---

# 🔹 Task 8: What is DNS Infiltration?

## 📖 Summary

This section explains:
- Delivering malicious payloads through DNS
- Using TXT records for malware staging
- DNS-based command and control (C2)
- Covert payload delivery

---

### Q: What type of DNS Record is usually used to infiltrate data into a network?
**A:** `TXT`

---

# 🔹 Task 9: DNS Infiltration - Demo

## 📖 Summary

This section demonstrates:
- Delivering encoded payloads via TXT records
- Decoding malicious payloads
- Simulating malware delivery through DNS

Tools used:
- `nslookup`
- `packetSimple.py`

---

### Q: Read the above.
**A:** No answer needed

---

# 🔹 Task 10: DNS Infiltration - Practice

## 📖 Summary

This challenge requires:
- Querying TXT records
- Decoding infiltrated payloads
- Executing recovered Python payloads

---

### Q: Follow the instructions in the TASK file to complete this question.

Enter the output from the executed python file
**A:** `4.4.0-186-generic`

---

# 🔹 Task 11: DNS Tunneling

## 📖 Summary

This section demonstrates:
- HTTP over DNS
- Bypassing network restrictions
- Creating DNS tunnels using iodine
- SOCKS proxy tunneling
- SSH over DNS

The demo shows how attackers tunnel traffic through DNS to bypass:
- Firewalls
- IDS
- IPS systems

---

### Q: What program was used to Tunnel HTTP over DNS?
**A:** `iodine`

---

# 🔹 Task 12: The End

## 📖 Summary

The final section recommends additional research into:
- Dependency Confusion attacks
- Advanced DNS abuse techniques
- Real-world covert communication attacks

---

### Q: End
**A:** No answer needed

---

# 🚀 Summary

This room demonstrated:

- DNS fundamentals
- DNS hierarchy and records
- DNS data exfiltration
- DNS data infiltration
- DNS tunneling
- HTTP over DNS
- Packet analysis
- Covert communication techniques

---

# 🧠 Key Takeaway

> DNS is one of the most trusted protocols in enterprise environments, making it an effective covert communication channel for attackers to exfiltrate data and bypass security controls.

---

# 🏁 Skills Gained

- DNS Enumeration
- DNS Analysis
- Data Exfiltration
- Data Infiltration
- DNS Tunneling
- Packet Analysis
- Wireshark Usage
- Covert Channel Techniques
- Network Security Awareness

---

# 🛠️ Tools Used

- Wireshark
- tshark
- iodine
- Python3
- nslookup
- dig
- Linux CLI

---

# ⚠️ Disclaimer

This repository is for **educational purposes only**.  
All activities were performed in a **controlled TryHackMe lab environment**.

---
