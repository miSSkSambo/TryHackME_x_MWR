# 🎲 Insecure Randomness 

---
link to the room: https://tryhackme.com/room/insecurerandomness


---

## 📌 Overview

This room focuses on **insecure randomness in web applications** and how predictable random values can lead to serious security vulnerabilities.

Randomness is critical for:
- Session tokens
- Password reset links
- Cryptographic keys

If implemented incorrectly, attackers can **predict or brute-force values**, leading to account compromise and data breaches.

---

## 🎯 Learning Objectives

- Understand insecure randomness and entropy
- Learn differences between TRNG and PRNG
- Identify weak entropy and predictable seeds
- Exploit insecure token generation
- Perform attacks on PRNG-based systems
- Learn mitigation strategies for secure randomness

---

## 🧠 Key Concepts

- **Entropy (Randomness Measurement)**
- **TRNG vs PRNG vs CSPRNG**
- **Weak Token Generation**
- **Timestamp-based Attacks**
- **Predictable Seeds**
- **Session Hijacking**
- **Magic Link Exploitation**

---

# ✅ Questions and Answers

## 🔹 Task 1: Introduction

**Q:** I am ready to start the room.  
**A:** No answer needed  

---

## 🔹 Task 2: Few Important Concepts

**Q:** What measures the amount of randomness or unpredictability in a system?  
**A:** entropy  

**Q:** Is it a good practice to keep the same seed value for all cryptographic functions? (yea/nay)  
**A:** nay  

---

## 🔹 Task 3: Types of Random Number Generators

**Q:** Which type of RNG is suitable for games with no critical security requirements?  
**A:** b (Statistical PRNG)  

---

## 🔹 Task 4: Weak or Insufficient Entropy

**Q:** What is the flag value after logging in as the victim user?  
**A:** THM{VICTIM_SIGNED_IN}  

**Q:** What is the flag value after logging in as the master user?  
**A:** THM{ADMIN_SIGNED_IN007}  

**Q:** What is the PHP function used to create the token variable in the code above?  
**A:** time() :contentReference[oaicite:0]{index=0}  

---

## 🔹 Task 5: Predictable Seed in PRNGs

**Q:** What is the flag value after logging in as magic@mail.random.thm?  
**A:** THM{MAGIC_SIGNED_IN11010}  

**Q:** What is the flag value after logging in as hr@mail.random.thm?  
**A:** THM{HR_SIGNED_IN1337}  

**Q:** What is the PHP function used to seed the RNG in the code above?  
**A:** mt_srand  

---

## 🔹 Task 6: Mitigation Measures

**Q:** Which of the following can be considered as a weak seed value?  
**A:** d (All of the above)  

---

## 🔹 Task 7: Conclusion

**Q:** I have completed the room.  
**A:** No answer needed  

---

## 🚀 Summary

This room highlights how **poor randomness can completely break security systems**.

Key takeaways:
- Low entropy leads to predictable tokens
- Timestamp-based tokens are easy to brute-force
- PRNGs can be reversed if the seed is known
- Magic links and session tokens must be unpredictable

---

## 🔐 Best Practices

- Use **CSPRNGs** (e.g., `random_bytes()`, `SecureRandom`)
- Avoid predictable seeds (timestamps, emails, IPs)
- Generate **high-entropy tokens**
- Never reuse seeds or random values
- Use proper cryptographic libraries

---
