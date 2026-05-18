# 📱 Android Hacking 101 (TryHackMe)

🔗 **Room Link:** https://tryhackme.com/room/androidhacking101

---

# 📖 Overview

This room introduces the fundamentals of **Android Mobile Application Penetration Testing**.

It focuses on:
- Android application architecture
- APK structure
- Reverse engineering Android applications
- Static analysis
- Dynamic analysis
- Smali code
- Android permissions
- AndroidManifest.xml analysis
- Mobile application security testing methodologies

The room demonstrates how penetration testers analyze Android applications to identify:
- Hardcoded secrets
- Insecure permissions
- Vulnerabilities
- Misconfigurations
- Sensitive information exposure
- Runtime protections

---

# 🎯 Learning Objectives

- Understand Android application architecture
- Learn APK file structure
- Understand Smali and Dalvik bytecode
- Perform Android reversing
- Perform static analysis
- Perform dynamic analysis
- Understand Android security testing methodologies
- Learn common Android protection bypasses

---

# 🧠 Key Concepts

- APK
- AndroidManifest.xml
- Dalvik VM
- Smali
- DEX Files
- Static Analysis
- Dynamic Analysis
- APK Reversing
- Android Permissions
- Intent Filters
- Activities
- Services
- Broadcast Receivers
- Content Providers
- SSL Pinning
- Root Detection
- Emulator Detection

---

# ✅ Questions and Answers

---

# 🔹 Task 1: Introduction

## 📖 Summary

This section explains:
- Native Android applications
- Hybrid Android applications
- APK structure
- Dalvik bytecode
- Smali assembly language
- Android registers
- APK components

The room explains how Android applications are packaged and how penetration testers reverse engineer APK files.

---

### Q: Read the above.
**A:** No answer needed

---

# 🔹 Task 2: Setup the environment

## 📖 Summary

This task focuses on preparing the Android penetration testing environment.

Tools commonly used:
- jadx
- apktool
- adb
- Android Studio
- Burp Suite
- Frida
- MobSF

The setup includes:
- Android emulators
- Rooted devices
- APK decompilers
- Dynamic analysis tooling

---

### Q: Read the above.
**A:** No answer needed

---

# 🔹 Task 3: Methodology

## 📖 Summary

This section explains Android pentesting methodology including:
- Information gathering
- APK extraction
- Static analysis
- Dynamic analysis
- Runtime testing
- Security validation

It demonstrates how testers systematically analyze mobile applications.

---

### Q: Read the above.
**A:** No answer needed

---

# 🔹 Task 4: Information Gathering

## 📖 Summary

This section focuses on:
- APK enumeration
- AndroidManifest.xml analysis
- Permission analysis
- Identifying exported components
- Discovering application metadata

---

### Q: What is the package name of the Black Hat Europe?
**A:** `com.swapcard.apps.android.blackhat`

---

# 🔹 Task 5: Reversing

## 📖 Summary

This section introduces Android reverse engineering.

Topics include:
- Decompiling APKs
- Reading Smali code
- Understanding Dalvik bytecode
- Analyzing logic flows
- Discovering hardcoded credentials
- Understanding registers

The room explains:
- `.registers`
- `.locals`
- Parameter registers (`p0`, `p1`, etc.)

---
### Q: Tool for convert dex file to smali code?
**A:** `d2j-dex2smali`

---

### Q: Which is the option for build apps with apktool?
**A:** `b`

---

### Q: What is the apk path of Black Hat Europe?
**A:** `/data/app/com.swapcard.apps.android.blackhat-1/base.apk`

---

### Q: Command for extract apk of Back Hat Europe?
**A:** `adb pull /data/app/com.swapcard.apps.android.blackhat-1/base.apk`

---

# 🔹 Task 6: Static analysis

## 📖 Summary

This section focuses on:
- Reviewing decompiled source code
- Searching for API keys
- Searching for tokens
- Hardcoded credentials
- Manifest misconfigurations
- Weak permissions

Common findings:
- Insecure logging
- Hardcoded secrets
- Debuggable applications
- Exported activities

---

### Q: What is the name of the firebase instance in the app Black Hat Europe?
**A:** `swapcard-android-app-2014`

### Q: Android-InsecureBankv2 debug realease, check this and what activity is not Protected.
**A:** `com.android.insecurebankv2.ChangePassword`

### Q: what is the malicious permissions in the app Android-InsecureBankv2?
**A:** `android.permission.SEND_SMS`

---

# 🔹 Task 7: Static analysis – Complications

## 📖 Summary

This section explains common complications during reversing such as:
- Code obfuscation
- Minified code
- Anti-tampering protections
- Encrypted strings
- Packed APKs

It explains why Android malware and secure applications use obfuscation.

---

### Q: Read the above.
**A:** No answer needed

---

# 🔹 Task 8: Dynamic Analysis

## 📖 Summary

This section explains runtime application testing.

Techniques include:
- Intercepting HTTP requests
- Monitoring runtime behavior
- Traffic analysis
- Runtime debugging
- Memory inspection

Tools commonly used:
- Burp Suite
- Frida
- Objection
- adb

---

### Q: Read the above.
**A:** No answer needed

---

# 🔹 Task 9: Dynamic Analysis – Complications

## 📖 Summary

This section focuses on protections used by applications to prevent runtime analysis.

Protections discussed:
- SSL pinning
- Root detection
- Emulator detection
- Anti-debugging
- Anti-hooking

These protections are common in:
- Banking apps
- Enterprise apps
- Secure messaging applications

---

### Q: Read the above.
**A:** No answer needed

---

# 🔹 Task 10: Bypass - Complications in Dynamic Analysis

## 📖 Summary

This section explains how penetration testers bypass:
- SSL pinning
- Root detection
- Emulator detection
- Runtime protections

Tools commonly used:
- Frida
- Objection
- Xposed

The room demonstrates how hooking frameworks modify application behavior at runtime.

---

### Q: Read the above.
**A:** No answer needed

---

# 🔹 Task 11: Final

## 📖 Summary

The final section concludes the room and encourages further mobile application security practice.

Recommended areas for further study:
- Android malware analysis
- Mobile API testing
- Runtime instrumentation
- Frida scripting
- Advanced reverse engineering

---

### Q: Read the above.
**A:** No answer needed

---

### Q: How likely are you to recommend this room to others?
**A:** Personal response

---

# 🚀 Summary

This room demonstrated:

- Android application architecture
- APK structure
- AndroidManifest.xml analysis
- Dalvik bytecode
- Smali code
- Static analysis
- Dynamic analysis
- Android reversing
- Runtime analysis
- Protection bypass techniques

---

# 🧠 Key Takeaway

> Android applications often contain sensitive information and insecure implementations that can be discovered through reverse engineering, static analysis, and dynamic analysis techniques.

---

# 🏁 Skills Gained

- Android APK Analysis
- Android Reversing
- Smali Analysis
- Static Analysis
- Dynamic Analysis
- Mobile Application Pentesting
- Android Security Testing
- Runtime Instrumentation Awareness

---

# 🛠️ Tools Mentioned

- apktool
- jadx
- adb
- Android Studio
- Burp Suite
- Frida
- MobSF
- Objection
- Xposed

---

# ⚠️ Disclaimer

This repository is for **educational purposes only**.  
All activities were performed in a **controlled TryHackMe lab environment**.

---
