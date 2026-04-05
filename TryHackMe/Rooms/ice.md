# ❄️ Ice 
---

link the room: https://tryhackme.com/room/ice

---
## 📖 Description

The **Ice TryHackMe room** is a beginner-friendly Windows exploitation lab that demonstrates how attackers can compromise a poorly secured system. It focuses on enumeration, exploitation of vulnerable services, privilege escalation, and post-exploitation techniques.

The room covers:
- Network scanning and service enumeration  
- Exploiting vulnerable software (Icecast)  
- Using Metasploit for exploitation  
- Privilege escalation techniques  
- Credential dumping with Mimikatz  
- Post-exploitation actions on Windows systems  

---

## 🧪 Full Questions & Answers

**Q: Connect to network / setup VPN**  
**A:** No answer needed  

---

**Q: What port is RDP running on?**  
**A:** 3389  

---

**Q: What service is running on port 8000?**  
**A:** Icecast  

---

**Q: What is the hostname?**  
**A:** DARK-PC  

---

**Q: What is the Impact Score of the vulnerability?**  
**A:** 6.4  

---

**Q: What is the CVE number?**  
**A:** CVE-2004-1561  

---

**Q: What is the Metasploit module path?**  
**A:** exploit/windows/http/icecast_header  

---

**Q: What required option is missing?**  
**A:** rhosts  

---

**Q: What shell do we get?**  
**A:** meterpreter  

---

**Q: What user is running Icecast?**  
**A:** Dark  

---

**Q: What Windows build is the system?**  
**A:** 7601  

---

**Q: What is the process architecture?**  
**A:** x64  

---

**Q: First suggested privilege escalation exploit?**  
**A:** exploit/windows/local/bypassuac_eventvwr  

---

**Q: What option must be set for listener IP?**  
**A:** LHOST  

---

**Q: What privilege allows file ownership?**  
**A:** SeTakeOwnershipPrivilege  

---

**Q: What is the printer service name?**  
**A:** spoolsv.exe  

---

**Q: What user are we after migration?**  
**A:** NT AUTHORITY\SYSTEM  

---

**Q: Command to retrieve all credentials?**  
**A:** creds_all  

---

**Q: What is Dark's password?**  
**A:** Password01  

---

**Q: Command to dump password hashes?**  
**A:** hashdump  

---

**Q: Command to view remote desktop?**  
**A:** screenshare  

---

**Q: Command to record microphone?**  
**A:** record_mic  

---

**Q: Command to modify timestamps?**  
**A:** timestomp  

---

**Q: Command to create a golden ticket?**  
**A:** golden_ticket_create  

---

## 🧠 Key Takeaways

- Weak configurations can expose systems to easy compromise  
- Enumeration is critical for identifying attack vectors  
- Metasploit simplifies exploitation workflows  
- Privilege escalation is essential for full system control  
- Credential dumping exposes sensitive user data  
- Post-exploitation techniques allow persistence and deeper access  

---

## 🚀 Skills Gained

- Network scanning with Nmap  
- Exploiting services using Metasploit  
- Windows privilege escalation  
- Credential harvesting (Mimikatz/Kiwi)  
- Post-exploitation techniques  
- Understanding real-world attack chains  

---

