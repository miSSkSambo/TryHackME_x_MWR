# 🌐 Nmap: Live Host Discovery  
🔗 Link to the room: https://tryhackme.com/room/nmap01  

---

## 📌 Overview  
This room introduces **Nmap host discovery techniques**, focusing on identifying which systems are online before performing port scanning.

It covers:
- ARP scanning  
- ICMP scanning  
- TCP/UDP ping techniques  
- Subnetting and target enumeration  

---

## 🎯 Learning Objectives  
- Discover live hosts efficiently  
- Understand different scanning techniques  
- Learn how Nmap uses protocols for discovery  
- Avoid scanning offline systems  
- Improve reconnaissance skills  

---

## 🧠 Key Concepts  
- Host Discovery  
- ARP (Address Resolution Protocol)  
- ICMP (Ping)  
- TCP SYN & ACK Ping  
- UDP Ping  
- Subnetting  
- Reverse DNS  

---

## ✅ Questions and Answers  

### 🔹 Task 1: Introduction  
**Q:** Completed  
**A:** No answer needed  

---

### 🔹 Task 2: Subnetworks  

**Q:** How many devices can see the ARP Request?  
**A:** 4 :contentReference[oaicite:0]{index=0}  

**Q:** Did computer6 receive the ARP Request?  
**A:** N :contentReference[oaicite:1]{index=1}  

**Q:** How many devices can see the ARP Request (second scenario)?  
**A:** 4 :contentReference[oaicite:2]{index=2}  

**Q:** Did computer6 reply to the ARP Request?  
**A:** Yea :contentReference[oaicite:3]{index=3}  

---

### 🔹 Task 3: Enumerating Targets  

**Q:** First IP in subnet 10.10.12.13/29?  
**A:** 10.10.12.8 :contentReference[oaicite:4]{index=4}  

**Q:** Number of IPs in range 10.10.0-255.101-125?  
**A:** 6400 :contentReference[oaicite:5]{index=5}  

---

### 🔹 Task 4: Discovering Live Hosts  

**Q:** Packet sent before ping?  
**A:** ARP Request :contentReference[oaicite:6]{index=6}  

**Q:** Packet received before ping?  
**A:** ARP Response :contentReference[oaicite:7]{index=7}  

**Q:** How many computers responded to ping?  
**A:** 1 :contentReference[oaicite:8]{index=8}  

**Q:** First device responding to first ARP request?  
**A:** router :contentReference[oaicite:9]{index=9}  

**Q:** First device responding to second ARP request?  
**A:** computer5 :contentReference[oaicite:10]{index=10}  

**Q:** Did another ping require new ARP requests?  
**A:** nay :contentReference[oaicite:11]{index=11}  

---

### 🔹 Task 5: ARP Host Discovery  

**Q:** How many devices discovered using ARP?  
**A:** 3 :contentReference[oaicite:12]{index=12}  

---

### 🔹 Task 6: ICMP Host Discovery  

**Q:** ICMP Timestamp option?  
**A:** -PP :contentReference[oaicite:13]{index=13}  

**Q:** ICMP Address Mask option?  
**A:** -PM :contentReference[oaicite:14]{index=14}  

**Q:** ICMP Echo option?  
**A:** -PE :contentReference[oaicite:15]{index=15}  

---

### 🔹 Task 7: TCP & UDP Discovery  

**Q:** TCP ping not requiring privileged account?  
**A:** TCP SYN Ping :contentReference[oaicite:16]{index=16}  

**Q:** TCP ping requiring privileged account?  
**A:** TCP ACK Ping :contentReference[oaicite:17]{index=17}  

**Q:** Option for TCP SYN ping on port 23?  
**A:** -PS23 :contentReference[oaicite:18]{index=18}  

---

### 🔹 Task 8: Reverse DNS  

**Q:** Option for reverse DNS lookup for all hosts?  
**A:** -R :contentReference[oaicite:19]{index=19}  

---

### 🔹 Task 9: Summary  
**Q:** Completed  
**A:** No answer needed  

---

## 🚀 Summary  

This room demonstrates how to discover live hosts using:

- ARP (local networks)  
- ICMP (ping-based discovery)  
- TCP/UDP probes (firewall evasion)  

---

## 🧠 Key Takeaway  

> Host discovery is the first step in reconnaissance —  
> scanning only live hosts saves time and reduces noise.

---

## 🏁 Skills Gained  
- Network Scanning  
- Nmap Usage  
- Host Discovery Techniques  
- Subnet Analysis  
- Reconnaissance Strategy  
