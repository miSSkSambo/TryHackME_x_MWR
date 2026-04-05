# 💣 Intro to Pwntools 

---

link to the room: https://tryhackme.com/room/introtopwntools

---

## 📖 Overview

The **Intro to Pwntools TryHackMe room** introduces the fundamentals of **binary exploitation** using :contentReference[oaicite:0]{index=0}.

This room focuses on how attackers:
- Exploit vulnerable programs (buffer overflows)
- Control program execution (EIP/RIP)
- Develop automated exploits using Python
- Spawn shells and escalate privileges

It also introduces debugging tools like :contentReference[oaicite:1]{index=1} to simplify reverse engineering and analysis.

---

## 🎯 What You Learn

### 🧠 Binary Exploitation Basics
- Stack memory and buffer overflows  
- Instruction pointer (EIP/RIP) control  
- Vulnerability analysis  

### 🛠️ Exploit Development
- Writing exploits using Pwntools  
- Automating attacks (local + remote)  
- Payload crafting  

### 🔍 Debugging & Analysis
- Using GDB + pwndbg  
- Identifying memory offsets  
- Understanding protections (NX, PIE, Canary, RELRO)  

### ⚔️ Advanced Techniques
- NOP sleds  
- Shellcode injection  
- Privilege escalation  

---

## 🧪 Room Breakdown

### 🔹 Task 2: Checksec
Learn about binary protections:
- RELRO  
- Stack canaries  
- NX  
- PIE  

### 🔹 Task 3: Cyclic
- Find buffer overflow offsets  
- Control EIP  
- Redirect execution to functions  

### 🔹 Task 4: Networking
- Exploit a remote service  
- Send payloads over a socket  

### 🔹 Task 5: Shellcraft
- Generate shellcode  
- Inject into memory  
- Spawn a root shell  

---

## 📌 Task 1: Introduction

**Q: I understand how to set up Pwntools and pwndbg.**  
**A:** No answer needed  

**Q: I have started the machine and logged in.**  
**A:** No answer needed  

---

## 📌 Task 2: Checksec

**Q: Does intro2pwn1 have FULL RELRO? (Y/N)**  
**A:** Y  

**Q: Does intro2pwn1 have RWX segments? (Y/N)**  
**A:** N  

**Q: Does intro2pwn2 have a stack canary? (Y/N)**  
**A:** N  

**Q: Does intro2pwn2 not have PIE? (Y/N)**  
**A:** Y  

**Q: Buffer overflow on intro2pwn1 detects what?**  
**A:** Stack Smashing  

**Q: Buffer overflow on intro2pwn2 causes what error?**  
**A:** Segmentation Fault  

---

## 📌 Task 3: Cyclic

**Q: Who owns flag.txt and intro2pwn3?**  
**A:** dizmas  

**Q: What protection is missing?**  
**A:** canary  

**Q: What ASCII sequence is 0x4a4a4a4a?**  
**A:** JJJJ  

**Q: Output of `cyclic 12`?**  
**A:** aaaabaaacaaa  

**Q: What pattern overflowed EIP?**  
**A:** 0x6161616a  

**Q: What is the flag?**  
**A:** flag{13@rning_2_pwn!}  

---

## 📌 Task 4: Networking

**Q: What port is serving the challenge?**  
**A:** 1337  

**Q: Does serve_test have a stack canary? (Y/N)**  
**A:** Y  

**Q: What is the flag?**  
**A:** flag{n3tw0rk!ng_!$_fun}  

---

## 📌 Task 5: Shellcraft

**Q: What does ASLR stand for?**  
**A:** address space layout randomization  

**Q: Who owns intro2pwnFinal?**  
**A:** root  

**Q: Is NX enabled? (Y/N)**  
**A:** N  

**Q: What fills the EIP?**  
**A:** taaa  

**Q: Breakpoint result message?**  
**A:** Trace/breakpoint trap  

**Q: What function does shellcraft use?**  
**A:** execve  

**Q: Who are you after exploitation?**  
**A:** root  

**Q: What is the flag?**  
**A:** flag{pwn!ng_!$_fr33d0m}  

---

## 📌 Task 6: Conclusion

**Q: I have learned the basics of pwntools.**  
**A:** No answer needed  

---

## 🧠 Key Takeaways

- Pwntools simplifies exploit development  
- Buffer overflows allow control of execution flow  
- Memory protections significantly affect exploit difficulty  
- Automation is key in real-world exploitation  
- Shellcode + NOP sleds enable reliable attacks  

---

## 🚀 Skills Gained

- Binary exploitation fundamentals  
- Python-based exploit scripting  
- Debugging with GDB  
- Remote and local exploitation  
- Privilege escalation  

---



This repository contains a full walkthrough and answers for the **Intro to Pwntools TryHackMe Room**.
