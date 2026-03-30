# 🌐 Introductory Networking 

---

link to the room: https://tryhackme.com/room/introtonetworking

---
<p align="center">
  <img src="https://img.shields.io/badge/TryHackMe-Networking-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Difficulty-Easy-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-Networking-yellow?style=for-the-badge" />
</p>

---

## 📌 Overview

This room introduces **fundamental networking concepts**, including:

* OSI Model
* TCP/IP Model
* Encapsulation
* Networking tools (Ping, Traceroute, Whois, Dig)

It builds the **foundation for cybersecurity and networking skills**.

---

## 🎯 Learning Objectives

* Understand the OSI and TCP/IP models
* Learn how data moves across networks
* Use basic networking tools
* Understand DNS and domain resolution

---

## 🧠 Key Concepts

* OSI 7-layer model
* TCP/IP 4-layer model
* Encapsulation & de-encapsulation
* DNS resolution process
* Networking tools

---

# 🧪 Walkthrough Summary

## 🔹 1. OSI Model (7 Layers)

| Layer | Name         |
| ----- | ------------ |
| 7     | Application  |
| 6     | Presentation |
| 5     | Session      |
| 4     | Transport    |
| 3     | Network      |
| 2     | Data Link    |
| 1     | Physical     |

✔ Mnemonic: *Anxious Pale Shakespeare Treated Nervous Drunks Patiently*

---

## 🔹 2. TCP/IP Model (4 Layers)

* Application
* Transport
* Internet
* Network Interface

---

## 🔹 3. Encapsulation

Data changes names across layers:

* Data → Segment/Datagram → Packet → Frame → Bits

✔ Reverse process = **De-encapsulation**

---

## 🔹 4. TCP Three-Way Handshake

1. SYN
2. SYN/ACK
3. ACK

✔ Establishes connection

---

## 🔹 5. Networking Tools

### Ping

```bash
ping target
```

### Traceroute

```bash
traceroute target
```

### Whois

```bash
whois domain
```

### Dig

```bash
dig domain
```

---

# ✅ FULL QUESTIONS & ANSWERS

---

## 🔹 Task 1

**Q:** Let's get started
**A:** No answer needed

---

## 🔹 Task 2 (OSI Model)

**Q:** Which layer chooses TCP/UDP?
**A:** 4

**Q:** Which layer checks data corruption?
**A:** 2

**Q:** Which layer formats data?
**A:** 2

**Q:** Which layer transmits data?
**A:** 1

**Q:** Which layer encrypts/compresses data?
**A:** 6

**Q:** Which layer tracks communication?
**A:** 5

**Q:** Which layer accepts app requests?
**A:** 7

**Q:** Which layer handles logical addressing?
**A:** 3

**Q:** TCP "bite-sized" pieces?
**A:** Segments

**Q:** FTP operates on which layer?
**A:** 7

**Q:** Best protocol for live video?
**A:** UDP

---

## 🔹 Task 3 (Encapsulation)

**Q:** Layer 2 data name?
**A:** Frames

**Q:** Layer 4 (UDP) data name?
**A:** Datagrams

**Q:** Process on received message?
**A:** De-encapsulation

**Q:** Which layer adds trailer?
**A:** Data Link

**Q:** Does encapsulation add security?
**A:** Aye

---

## 🔹 Task 4 (TCP/IP Model)

**Q:** Which model came first?
**A:** TCP/IP

**Q:** TCP/IP layer matching OSI Transport?
**A:** Transport

**Q:** TCP/IP layer matching OSI Session?
**A:** Application

**Q:** Network Interface matches Data Link + ?
**A:** Physical

**Q:** TCP/IP layer for OSI Network?
**A:** Internet

**Q:** TCP type?
**A:** Connection-based

**Q:** SYN stands for?
**A:** Synchronise

**Q:** Second handshake step?
**A:** SYN/ACK

**Q:** ACK short form?
**A:** ACK

---

## 🔹 Task 5 (Ping)

**Q:** Command to ping BBC?
**A:** ping bbc.co.uk

**Q:** IP of muirlandoracle.co.uk?
**A:** 217.160.0.152

**Q:** Interval switch?
**A:** -i

**Q:** Force IPv4?
**A:** -4

**Q:** Verbose output?
**A:** -v

---

## 🔹 Task 6 (Traceroute)

**Q:** View route path
**A:** No answer needed

**Q:** Interface switch?
**A:** -i

**Q:** TCP SYN switch?
**A:** -T

**Q:** Default TCP/IP layer?
**A:** Internet

---

## 🔹 Task 7 (Whois)

**Q:** Facebook postal code?
**A:** 94025

**Q:** Facebook registration date?
**A:** 29/03/1997

**Q:** Microsoft registrant city?
**A:** Redmond

**Q:** Nearby golf course?
**A:** Bellevue Golf Course

**Q:** Microsoft tech email?
**A:** [msnhst@microsoft.com](mailto:msnhst@microsoft.com)

---

## 🔹 Task 8 (DNS & Dig)

**Q:** DNS stands for?
**A:** Domain Name System

**Q:** First DNS server queried?
**A:** Recursive

**Q:** Server handling domain extensions?
**A:** Top-Level Domain

**Q:** First lookup location?
**A:** Hosts File

**Q:** Second Google DNS server?
**A:** 8.8.4.4

**Q:** TTL for 24 hours?
**A:** 86400

---

## 🔹 Task 9

**Q:** Read final thoughts
**A:** No answer needed

---

# 🚀 Networking Flow Summary

1. Application generates data
2. Data moves down OSI layers
3. Encapsulation occurs
4. Data transmitted across network
5. Receiver performs de-encapsulation
6. Data delivered to application

---

## ⚠️ Key Takeaways

* OSI model = conceptual framework
* TCP/IP = real-world implementation
* DNS resolves domains → IP addresses
* Tools like ping & traceroute help troubleshoot networks
* Encapsulation ensures structured communication

---

## 💡 Final Insight

Networking is the foundation of cybersecurity:

➡️ Every attack uses networking
➡️ Every defense depends on understanding traffic

Mastering this = mastering cyber fundamentals

---

## 📚 Reference

TryHackMe — Introductory Networking 

---
