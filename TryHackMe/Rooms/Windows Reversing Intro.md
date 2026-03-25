# 🧠 Windows Reversing Intro 

---

link to the room: https://tryhackme.com/room/windowsreversingintro

---

## 📌 Overview

This room introduces **reverse engineering Windows x64 applications** using tools like IDA.

You learn how high-level code (C/C++) translates into:
- Assembly instructions
- Function calls
- Loops
- Memory structures

It builds the foundation for deeper reverse engineering and malware analysis.

---

## 🎯 Learning Objectives

- Understand static vs dynamic analysis
- Learn how to use IDA Freeware
- Identify function calls and parameters
- Analyze loops in assembly
- Understand stack frames (prologue/epilogue)
- Learn basics of structures and DLLs

---

## 🧠 Key Concepts

- **Reverse Engineering**
- **Static vs Dynamic Analysis**
- **Disassembly vs Decompilation**
- **Calling Conventions (fastcall)**
- **Stack Frames (RSP, RBP)**
- **Function Prologue/Epilogue**
- **Loops in Assembly**
- **Structures & Memory Layout**
- **DLL Imports/Exports**
- **Name Mangling**

---

# ✅ Questions and Answers

## 🔹 Task 1: Introduction

**Q:** Let's get started!  
**A:** No answer needed  

---

## 🔹 Task 2: IDA Overview

**Q:** Once comfortable with IDA  
**A:** No answer needed  

---

## 🔹 Task 3: Function Prologue/Epilogue

**Q:** Read the above  
**A:** No answer needed  

---

## 🔹 Task 4: Function Call Analysis

**Q:** Which instruction sets up the first parameter for printf()?  
**A:** lea rcx, Format  

---

## 🔹 Task 5: Loop Analysis

**Q:** Which instruction identifies the loop counter?  
**A:** inc rcx  

---

## 🔹 Task 6: Structures

**Q:** Read the above  
**A:** No answer needed  

---

## 🔹 Task 7: DLLs

**Q:** Read the above  
**A:** No answer needed  

---

## 🔹 Task 8: Conclusion

**Q:** Go forth and do great things!  
**A:** No answer needed  

---

## 🚀 Summary

This room teaches the **fundamentals of reverse engineering Windows programs**.

You learned how to:
- Read assembly code in IDA
- Identify function calls and parameters
- Understand loops at a low level
- Recognize compiler optimizations (like inlining)
- Analyze structures in memory
- Understand DLL behavior and imports/exports

---

## ⚠️ Key Takeaways

- Reverse engineering requires **pattern recognition**
- Always focus on the **big picture**, not individual instructions
- Compilers optimize code → not always straightforward
- IDA graph view helps visualize program flow
- Strings and XREFs are powerful for navigation

---

## 🔐 Important Concepts

### Function Parameters (x64 fastcall)
- RCX → 1st parameter  
- RDX → 2nd parameter  
- R8 → 3rd parameter  
- R9 → 4th parameter  

---

### Loop Pattern (Assembly)
- Initialize counter  
- Compare with limit  
- Increment (`inc rcx`)  
- Jump back  

---

## 💡 Key Insight

Reverse engineering is about:
- Making **educated guesses**
- Verifying them step-by-step
- Understanding patterns over time

---

## 🎯 Final Note

This room is your **starting point for advanced reverse engineering**, leading into:
- Malware analysis  
- Exploit development  
- Binary exploitation  

---
