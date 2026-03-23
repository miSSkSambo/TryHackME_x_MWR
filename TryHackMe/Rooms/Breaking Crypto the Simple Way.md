# 🔐 Cryptography Mistakes 

---
link to the room: https://tryhackme.com/room/breakingcryptothesimpleway

## 📌 Overview

This room explores **common cryptographic mistakes** and how attackers exploit them. It shows that cryptography itself is usually secure — but poor implementation can lead to serious vulnerabilities.

You will learn how weak keys, exposed secrets, insecure hashing, and unauthenticated encryption can be broken in real-world scenarios.

---

## 🎯 Learning Objectives

- Understand why cryptographic mistakes occur
- Learn how to exploit weak encryption keys
- Break insecure hashing implementations
- Identify exposed keys in applications
- Perform bit-flipping attacks
- Learn best practices for secure cryptography

---

## 🧠 Key Concepts

- **RSA Weak Keys (p & q vulnerabilities)**
- **Brute-force Attacks**
- **Hash Cracking (HMAC, SHA1)**
- **Client-side Key Exposure**
- **AES Encryption (CBC Mode)**
- **Bit Flipping Attacks**
- **Secure Cryptographic Practices**

---

# ✅ Questions and Answers

## 🔹 Task 1: Introduction

**Q:** I have started the target machine and I'm ready to break crypto!  
**A:** No answer needed  

---

## 🔹 Task 2: Brute-forcing Keys

**Q:** What is the flag?  
**A:** THM{Psssss_4nd_Qsssssss}  

---

## 🔹 Task 3: Breaking Hashes

**Q:** What is the secret used to encrypt the message?  
**A:** sunshine :contentReference[oaicite:0]{index=0}  

---

## 🔹 Task 4: Exposed Keys

**Q:** What is the flag?  
**A:** THM{3nD_2_3nd_is_n0t_c0mpl1c4ted}  

---

## 🔹 Task 5: Bit Flipping Attacks

**Q:** What is the flag?  
**A:** THM{flip_n_flip}  

---

## 🔹 Task 6: Conclusion

**Q:** Click me to proceed to the next task.  
**A:** No answer needed  

---

## 🚀 Summary

This room demonstrates that **cryptography is only as strong as its implementation**.

Key takeaways:
- Weak or predictable keys can be brute-forced
- Fast hash functions (like SHA-256) are not suitable for passwords
- Exposed keys in frontend code lead to full compromise
- AES without integrity protection is vulnerable to bit-flipping attacks

---

## 🔐 Best Practices

- Use strong, random keys (high entropy)
- Use secure hashing (bcrypt, Argon2, PBKDF2)
- Never expose keys in client-side code
- Use authenticated encryption (AES-GCM)
- Regularly audit and test cryptographic implementations

---
