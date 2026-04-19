# 🛡️ MWR CyberSec Virtual Internship – Week 7 (CSRF)  
🔗 Link to the room: https://tryhackme.com/room/MWR-CyberSec-Week-7-Cross-Site-Request-Forgery

---

## 📌 Overview  
This lab focuses on **Cross-Site Request Forgery (CSRF)** — how it works, how to exploit it, and how to prevent it.

---

## 🎯 Learning Objectives  
- Understand CSRF attacks  
- Identify vulnerable endpoints  
- Perform CSRF exploitation  
- Bypass weak defenses  
- Implement mitigation techniques  

---

## 🧠 Key Concepts  
- CSRF  
- Cookies & Sessions  
- SameSite Attribute  
- CSRF Tokens  
- Double Submit Cookies  
- CORS & SOP  

---

## ✅ Questions and Answers  

### 🔹 Task 1: Introduction  
**Q:** Completed  
**A:** No answer needed  

---

### 🔹 Task 2: What is CSRF?  

**Q:** What relationship between the browser and the web application does CSRF abuse?  
**A:** Trust  

**Q:** What does the browser automatically include with requests after login?  
**A:** Cookies  

**Q:** What flag for the above resource mitigates CSRF?  
**A:** SameSite  

**Q:** What type of action is usually required for a CSRF attack to succeed?  
**A:** State-changing  

**Q:** What type of request is normally used to perform the above action?  
**A:** POST  

**Q:** What are the 3 values of the SameSite flag?  
**A:** Strict, Lax, None  

**Q:** Where is the malicious request generated from?  
**A:** Victim's Browser  

---

### 🔹 Task 3: Finding CSRF  

**Q:** What HTTP method do developers incorrectly believe prevents CSRF?  
**A:** POST  

**Q:** What mechanism prevents CSRF attacks?  
**A:** CSRF tokens  

---

### 🔹 Task 4: Practical  

**Q:** Flag after updating email to attacker@evilmail.thm?  
**A:** MWR{New-Mail-Who-Dis}  

**Q:** Flag after updating email to special@evilmail.thm?  
**A:** MWR{This-one-was-special}  

**Q:** Flag after demoting the user from admin to staff?  
**A:** MWR{Demotion-Day}  

**Q:** Encoding scheme used for CSRF tokens?  
**A:** base64  

---

### 🔹 Task 5: CSRF Bypasses  

**Q:** Flag after successful transfer from Josh's account?  
**A:** MWR{For-Profit}  
<img width="954" height="778" alt="Screenshot 2026-04-14 162813" src="https://github.com/user-attachments/assets/5a797931-14d1-438f-9198-ec5ad457f450" />


**Q:** Flag after CSRF detection?  
**A:** MWR{No-more-profit}  
<img width="961" height="491" alt="Screenshot 2026-04-14 163238" src="https://github.com/user-attachments/assets/fd15e27b-60c8-44d6-9660-65922874b970" />


**Q:** Decoded CSRF token value?  
**A:** GB82MYBANK5699  

**Q:** Updated password for Josh’s account?  
**A:** GB82MYBANK5697  

**Q:** Hidden field added to prevent CSRF?  
**A:** csrf_token  

**Q:** Logout cookie value?  
**A:** 7kRt2x9LpQyW  

**Q:** Flag after logout attack?  
**A:** MWR{Bon-voyage}  
<img width="935" height="688" alt="Screenshot 2026-04-15 215633" src="https://github.com/user-attachments/assets/ebc265fa-2e56-4f74-adc4-3c44d2635304" />

**Q:** Flag after detection when cookie modified?  
**A:** MWR{We-see-your-attack}  
<img width="941" height="811" alt="Screenshot 2026-04-15 220949" src="https://github.com/user-attachments/assets/4c7eb496-e286-466e-a15c-43921edb4d75" />

**Q:** Flag after banning user? 
**A:** MWR{User-met-the-ban-hammer}  
<img width="968" height="691" alt="Screenshot 2026-04-15 221156" src="https://github.com/user-attachments/assets/085654c3-d47b-4478-b281-dbdf39906bd1" />

---

### 🔹 Task 6: More Bypasses  
**Q:** No questions  
**A:** No answer needed  

---

### 🔹 Task 7: Preventing CSRF  

**Q:** What is the best remedial action for CSRF?  
**A:** CSRF Tokens  

---

### 🔹 Task 8: Extra Content  
**Q:** Completed  
**A:** No answer needed  

---

## 🚀 Summary  

This lab shows how attackers can:
- Exploit trust between browser and server  
- Perform actions without user consent  
- Bypass weak CSRF protections  

---

## 🧠 Key Takeaway  

> CSRF is about exploiting **trusted sessions**, not stealing credentials.

---

## 🏁 Skills Gained  
- Web Security Testing  
- CSRF Exploitation  
- Security Mitigation  
- Real-world Attack Simulation  
