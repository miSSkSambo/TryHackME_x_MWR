# 🛡️ Snort 

---

link to the room: https://tryhackme.com/room/snort

---

<p align="center">
  <img src="https://img.shields.io/badge/TryHackMe-Snort-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Difficulty-Intermediate-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-BlueTeam-green?style=for-the-badge" />
</p>

---

## 📌 Overview

This room focuses on **Snort**, a powerful:

* Network Intrusion Detection System (NIDS)
* Network Intrusion Prevention System (NIPS)

You will learn how to:

* Detect threats in real-time
* Analyse traffic (live & PCAP)
* Write custom detection rules
* Use Snort operational modes

---

## 🎯 Learning Objectives

* Understand IDS vs IPS
* Learn Snort architecture
* Use Snort modes (Sniffer, Logger, IDS/IPS)
* Analyse PCAP files
* Write and test Snort rules

---

## 🧠 Key Concepts

* IDS vs IPS
* Signature-based detection
* Behaviour-based detection (NBA)
* Packet analysis
* Rule-based detection

---

# 🧪 WALKTHROUGH

---

## 🔹 Task 1 — Introduction

**Q:** Read the task
**A:** No answer needed

---

## 🔹 Task 2 — Setup

**Q:** Run `./.easy.sh` output?
**A:** Too Easy!

---

## 🔹 Task 3 — IDS/IPS Concepts

**Q:** Stop threats on local machine?
**A:** HIPS

**Q:** Detect threats on network?
**A:** NIDS

**Q:** Detect threats on local machine?
**A:** HIDS

**Q:** Stop threats on network?
**A:** NIPS

**Q:** Detect anomalies?
**A:** NBA

**Q:** Snort is what type of NIPS?
**A:** full-blown

**Q:** NBA training period?
**A:** baselining

---

## 🔹 Task 4 — First Interaction

**Q:** Snort build number?
**A:** 149

**Q:** Rules loaded (snort.conf)?
**A:** 4151

**Q:** Rules loaded (snortv2.conf)?
**A:** 1

---

## 🔹 Task 5 — Sniffer Mode

📌 Key flags:

```bash
snort -v        # verbose
snort -d        # payload
snort -e        # headers
snort -X        # full packet
snort -i eth0   # interface
```

**Q:** Practice
**A:** No answer needed

---

## 🔹 Task 6 — Packet Logger Mode

📌 Key commands:

```bash
snort -dev -l .              # log packets
snort -dev -K ASCII -l .     # readable logs
snort -r file.log            # read logs
```

**Q:** Source port to port 53?
**A:** 3009

**Q:** IP ID of 10th packet?
**A:** 49313

**Q:** Referer (4th packet)?
**A:** http://www.ethereal.com/development.html

**Q:** ACK number (8th packet)?
**A:** 0x38AFFFF3

**Q:** TCP port 80 packets?
**A:** 41

---

## 🔹 Task 7 — IDS/IPS Mode

📌 Key commands:

```bash
snort -c /etc/snort/snort.conf -A console
snort -c /etc/snort/snort.conf -A full
snort -c /etc/snort/snort.conf -A fast
snort -c /etc/snort/snort.conf -A none
```

📌 IPS mode:

```bash
snort -c /etc/snort/snort.conf -Q --daq afpacket -i eth0:eth1
```

**Q:** HTTP GET detected?
**A:** 2

---

## 🔹 Task 8 — PCAP Analysis

📌 Commands:

```bash
snort -r file.pcap
snort --pcap-list="file1 file2"
snort --pcap-show
```

**Q:** Alerts (mx-1, default)?
**A:** 170

**Q:** TCP segments queued?
**A:** 18

**Q:** HTTP response headers?
**A:** 3

**Q:** Alerts (snortv2.conf)?
**A:** 68

**Q:** Alerts (mx-2)?
**A:** 340

**Q:** TCP packets?
**A:** 82

**Q:** Alerts (mx-2 + mx-3)?
**A:** 1020

---

## 🔹 Task 9 — Snort Rules

📌 Rule structure:

```bash
action protocol src_ip src_port direction dst_ip dst_port (options)
```

📌 Example:

```bash
alert icmp any any <> any any (msg:"ICMP Packet Found"; sid:100001; rev:1;)
```

---

### Answers

**Q:** Request name (ID 35369)?
**A:** TIMESTAMP REQUEST

**Q:** SYN packets count?
**A:** 1

**Q:** PSH-ACK packets?
**A:** 216

**Q:** Same source/destination IP?
**A:** 7

**Q:** Which field to update after rule change?
**A:** rev

---

## 🔹 Task 10 — Snort Logic

📌 Components:

* Packet Decoder
* Preprocessors
* Detection Engine
* Logging & Alerting
* Output Modules

📌 Important files:

* `/etc/snort/snort.conf`
* `/etc/snort/rules/local.rules`

---

## 🔹 Task 11 — Conclusion

**Q:** Read task
**A:** No answer needed

---

# 🚀 Snort Modes Summary

| Mode    | Purpose        |
| ------- | -------------- |
| Sniffer | View packets   |
| Logger  | Save packets   |
| IDS     | Detect threats |
| IPS     | Block threats  |

---

## ⚠️ Key Takeaways

* Snort is **rule-based detection system**
* IDS = detect only
* IPS = detect + block
* Rules are the core of Snort
* PCAP analysis speeds up investigations

---

## 💡 Pro Tips

* Always test rules before deployment
* Use simple rules first
* Avoid duplicate SIDs
* Keep backups of configs

---

## 📚 Reference

TryHackMe — Snort Room 

---

## 🏁 Final Insight

Snort is a **core blue-team tool**:

➡️ Used in SOC environments
➡️ Detects real-time attacks
➡️ Builds foundation for SIEM tools

---
