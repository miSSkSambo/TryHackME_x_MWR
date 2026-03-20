# 🔐 Burp Suite – Detailed Q&A Notes
---
## 🎯 What This Assignment Is About

This assignment introduces you to **web application security (AppSec)** using **Burp Suite**, a powerful tool used by ethical hackers and security professionals.
Link to the room: https://tryhackme.com/jr/MWR-CyberSec-Week-1-8w-9ypa  

You learn how to:
- 🌍 Understand how web apps communicate (HTTP/HTTPS)
- 🛠️ Intercept and modify requests between browser and server
- 🔍 Test applications for vulnerabilities
- ⚡ Use core tools like Proxy, Repeater, Intruder, Decoder, Comparer, and Sequencer

👉 The goal is to move from just *using websites* to **analyzing and testing how they work behind the scenes**.

💡 Perfect for frontend developers who want to build **secure and robust applications**.

---

## 🚀 Overview
This repo contains structured **Q&A notes** for learning Burp Suite.  
Perfect for developers stepping into **AppSec & Web Testing**.

---


## 📘 Task 1: Introduction
**Q:** From which primary tool or platform do experienced Application Security (AppSec) professionals conduct most of their web application testing?  
**A:** Burp Suite  

## 📘 Task 2: What is Burp Suite
**Q:** Which edition of Burp Suite is designed to run on a server and perform continuous, automated vulnerability scanning of target web applications?  
**A:** Burp Suite Enterprise  

**Q:** Burp Suite is commonly used when performing security testing on web applications as well as which other type of applications?  
**A:** Mobile  

**Q:** Which company is responsible for developing and maintaining Burp Suite?  
**A:** PortSwigger  

**Q:** If you want to further develop your application security skills using official PortSwigger resources, which platform should you use?  
**A:** Web Security Academy  

## 📘 Task 3: Features of Burp Community
**Q:** By default, what IP address and port does the Burp Suite Proxy use to intercept and route web traffic?  
**A:** 127.0.0.1:8080  

**Q:** What keyboard shortcut is used to send an intercepted HTTP request from the Proxy to the Repeater tool?  
**A:** CTRL + R  

**Q:** What keyboard shortcut is used to send an intercepted HTTP request from the Proxy to the Intruder tool?  
**A:** CTRL + I  

**Q:** In the Burp Suite Decoder tool, which encoding/decoding scheme is represented by the color pink?  
**A:** Binary  

**Q:** When performing race condition testing, where in Burp Suite would you execute simultaneous requests?  
**A:** Repeater → Send → Send Group in Parallel  

## 📘 Task 4: Options
**Q:** Within the Burp Suite settings, under which category can you find configurations related to the "Cookie jar"?  
**A:** Sessions  

**Q:** Under which main settings category can the "Updates" sub-category be found?  
**A:** Suite  

**Q:** Can client-side TLS certificates be overridden on a per-project basis?  
**A:** Yea  

## 📘 Task 5: Burp Target and Proxy
**Q:** Where can you view a complete log of all HTTP requests that have passed through the proxy?  
**A:** HTTP History  

**Q:** Which feature allows you to view all discovered endpoints?  
**A:** Site Map  

**Q:** Which functionality allows excluding domains from interception?  
**A:** Scope  

**Q:** Where can you find vulnerability knowledge in Burp Suite?  
**A:** Issues  

**Q:** Which browser should you use with Burp Suite?  
**A:** Personal Preference  

## 📘 Task 6: Intruder
**Q:** Which attack type inserts one payload at a time into each position?  
**A:** Sniper  

**Q:** Which attack type is used for race conditions?  
**A:** Battering Ram  

**Q:** Maximum payload sets in Pitchfork mode?  
**A:** 20  

**Q:** Total requests in Cluster Bomb (100×2×30)?  
**A:** 6000  

**Q:** Which rule adds characters to payloads?  
**A:** Add suffix  

**Q:** Which symbol defines payload positions?  
**A:** §  

## 📘 Task 7: Repeater
**Q:** Which section provides intuitive request control?  
**A:** Inspector  

**Q:** Which section is specific to POST requests?  
**A:** Body Parameters  

**Q:** Which option renders the response visually?  
**A:** Render  

**Q:** Which view is populated when sending from Proxy?  
**A:** Request  

## 📘 Task 8: Decoder
**Q:** Base64 encode "Let's Start Simple."  
**A:** TGV0J3MgU3RhcnQgU2ltcGxl  

**Q:** URL decode result?  
**A:** Next: Decoding  

**Q:** Decode Base64 string result?  
**A:** encoding is very kewl  

**Q:** Linux tool for Base64?  
**A:** base64  

**Q:** Final multi-encoding string?  
**A:** 24034214a720270024142d541357471232250253552c1162d1206c  

**Q:** Characters removed in JWT Base64?  
**A:** +, =, /  

## 📘 Task 9: Comparer
**Q:** Linux equivalent tool?  
**A:** diff  

## 📘 Task 10: Sequencer
**Q:** What does Sequencer evaluate?  
**A:** Entropy  
