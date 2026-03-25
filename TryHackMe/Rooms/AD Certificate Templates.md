# 🏢 AD Certificate Templates 

---

link to the room: https://tryhackme.com/room/adcertificatetemplates

---
## 📌 Overview

This room explores **Active Directory Certificate Services (AD CS)** and how **misconfigured certificate templates** can lead to **privilege escalation to Domain Admin**.

Using a vulnerable template, a low-privileged user can:
- Request a malicious certificate
- Impersonate privileged users
- Gain **persistent access** to the domain

---

## 🎯 Learning Objectives

- Understand AD CS and PKI concepts
- Enumerate certificate templates
- Identify vulnerable configurations
- Generate malicious certificates
- Perform user impersonation
- Achieve Domain Admin privileges

---

## 🧠 Key Concepts

- **AD CS (Active Directory Certificate Services)**
- **PKI (Public Key Infrastructure)**
- **Certificate Templates**
- **EKU (Extended Key Usage)**
- **SAN (Subject Alternative Name)**
- **Kerberos Authentication**
- **Privilege Escalation**
- **Persistence via Certificates**

---

# ✅ Questions and Answers

## 🔹 Task 1: Introduction

**Q:** Read the above  
**A:** No answer needed  

---

## 🔹 Task 2: Certificate Templates Basics

**Q:** What does the user create to request a certificate?  
**A:** Certificate Signing Request  

**Q:** What is Microsoft’s PKI implementation?  
**A:** Active Directory Certificate Services  

---

## 🔹 Task 3: Enumeration

**Q:** Which AD group allows all users to request certificates?  
**A:** Domain Users  

**Q:** Which AD group allows computers to request certificates?  
**A:** Domain Computers  

**Q:** Which EKU allows Kerberos authentication?  
**A:** Client Authentication  

**Q:** Which certificate template is misconfigured?  
**A:** User Request  

---

## 🔹 Task 4: Malicious Certificate

**Q:** Where do we inject the UPN of the target account?  
**A:** Subject Alternative Name  

**Q:** Which option allows using the machine account if admin access exists?  
**A:** Computer account  

---

## 🔹 Task 5: User Impersonation

**Q:** What is the final flag?  
**A:** THM{AD.Certs.Can.Get.You.DA}

---

## 🔹 Task 6: Mitigation

**Q:** Read the above  
**A:** No answer needed  

---

## 🔹 Task 7: Conclusion

**Q:** Read the above  
**A:** No answer needed  

---

## 🚀 Summary

This room demonstrates how **misconfigured certificate templates** can be abused to:

1. Request a malicious certificate  
2. Impersonate privileged users  
3. Obtain a Kerberos TGT  
4. Reset Domain Admin passwords  
5. Gain full control of the domain  

---

## ⚠️ Key Takeaways

- Certificates can bypass password resets → **persistent access**
- AD CS is often overlooked but **highly dangerous if misconfigured**
- SAN manipulation allows **user impersonation**
- Low-privileged users can escalate to **Domain Admin**

---

## 🔐 Mitigation

- Audit certificate templates (use tools like PSPKIAudit)
- Restrict **Enroll permissions**
- Disable SAN specification where unnecessary
- Require **admin approval for certificate requests**
- Revoke compromised certificates
- Monitor abnormal certificate usage

---

## 💡 Key Insight

Unlike passwords, certificates can remain valid for years — making them a **powerful persistence mechanism** in Active Directory environments.

---
