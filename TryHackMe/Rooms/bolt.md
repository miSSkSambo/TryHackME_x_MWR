# ⚡ Bolt 

---

link to the room: https://tryhackme.com/room/bolt

---

## 📖 Description

The **Bolt TryHackMe room** focuses on exploiting a vulnerable web application built on the **Bolt CMS**. It demonstrates how attackers can enumerate a target, discover credentials, and exploit a known vulnerability to achieve **Authenticated Remote Code Execution (RCE)**.

The room covers:
- Web enumeration and service discovery  
- Identifying CMS platforms and versions  
- Credential discovery  
- Exploiting known vulnerabilities using Exploit-DB and Metasploit  
- Gaining remote access and retrieving flags  

---

## 🧪 Full Questions & Answers

**Q: Start the machine**  
**A:** No answer needed  

---

**Q: What port number has a web server with a CMS running?**  
**A:** 8000  

---

**Q: What is the username we can find in the CMS?**  
**A:** bolt  

---

**Q: What is the password we can find for the username?**  
**A:** boltadmin123  

---

**Q: What version of the CMS is installed on the server?**  
**A:** Bolt 3.7.1  

---

**Q: There's an exploit for a previous version of this CMS. What is its EDB-ID?**  
**A:** 48296  

---

**Q: What is the full Metasploit module path?**  
**A:** exploit/unix/webapp/bolt_authenticated_rce  

---

**Q: Set required options and run exploit**  
**A:** No answer needed  

---

**Q: Look for flag.txt inside the machine**  
**A:** THM{wh0_d035nt_l0ve5_b0l7_r1gh7?}  

---

## 🧠 Key Takeaways

- CMS platforms are common attack surfaces  
- Version enumeration is critical for finding exploits  
- Weak credentials can lead to full compromise  
- Exploit-DB and Metasploit are powerful tools for attackers  
- Authenticated RCE allows complete system control  

---

## 🚀 Skills Gained

- Web application enumeration  
- Vulnerability identification  
- Exploit research (Exploit-DB)  
- Using Metasploit modules  
- Remote code execution techniques  

---
