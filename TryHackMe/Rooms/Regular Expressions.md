# 🔍 Regular Expressions 

---
link to the room:https://tryhackme.com/room/catregex

---

## 📌 Overview

This room introduces **Regular Expressions (Regex)** — powerful patterns used to search, match, and manipulate text.

Regex is widely used in:
- Cybersecurity (log analysis, data extraction)
- Programming
- Data validation
- CTF challenges

---

## 🎯 Learning Objectives

- Understand basic regex syntax
- Use character sets and wildcards
- Apply repetition and metacharacters
- Match patterns using groups and anchors
- Extract structured data (emails, IPs, etc.)

---

## 🧠 Key Concepts

- **Charsets `[ ]`**
- **Wildcards `.`**
- **Repetition (`*`, `+`, `{}`)**
- **Metacharacters (`\d`, `\w`, `\s`)**
- **Anchors (`^`, `$`)**
- **Grouping `( )`**
- **Alternation `|`**

---

# ✅ Questions and Answers

## 🔹 Task 1: Introduction

**Q:** Read the above  
**A:** No answer needed  

---

## 🔹 Task 2: Charsets

**Q:** Match characters c, o, g  
**A:** `[cog]`  

**Q:** Match words cat, fat, hat  
**A:** `[cfh]at`  

**Q:** Match Cat, cat, Hat, hat  
**A:** `[CcHh]at`  

**Q:** Match filenames File1–file9  
**A:** `[Ff]ile[1-9]`  

**Q:** Exclude File7  
**A:** `[Ff]ile[^7]`  

---

## 🔹 Task 3: Wildcards & Optional Characters

**Q:** Match Cat, fat, hat, rat  
**A:** `.at`  

**Q:** Match Cat, cats  
**A:** `[Cc]ats?`  

**Q:** Match cat.xyz  
**A:** `cat\.xyz`  

**Q:** Match cat.xyz, cats.xyz, hats.xyz  
**A:** `[ch]ats?\.xyz`  

**Q:** Match 4-letter strings not ending in n–z  
**A:** `...[^n-z]`  

**Q:** Match bat, bats, hat, hats (not rat)  
**A:** `[^r]ats?`  

---

## 🔹 Task 4: Metacharacters & Repetitions

**Q:** Match catssss  
**A:** `cats{4}`  

**Q:** Match Cat, cats, catsss  
**A:** `[Cc]ats*`  

**Q:** Match regex go brrrr  
**A:** `regex go br+`  

**Q:** Match binary filenames  
**A:** `[abc]{1,3}[01]{4}`  

**Q:** Match File01, File2, file12  
**A:** `[Ff]ile\d{1,2}`  

**Q:** Match kali tools (variable spaces)  
**A:** `kali\s+tools`  

**Q:** Match notes~, stuff@, etc.  
**A:** `\w{5}\W`  

**Q:** Match complex string  
**A:** `\S*\s*\S*`  

**Q:** Match 9-char string not ending in !  
**A:** `\S{8}[^!]`  

**Q:** Match .bash_rc, note1  
**A:** `\.?\w+`  

---

## 🔹 Task 5: Anchors, Groups & OR

**Q:** Match Password with 10 non-zero chars  
**A:** `Password:[^0]{10}`  

**Q:** Match username at start  
**A:** `^username:\s`  

**Q:** Match lines not starting with digit  
**A:** `^\D`  

**Q:** Match EOF$ at end  
**A:** `EOF\$$`  

**Q:** Match nano or vim  
**A:** `I use (nano|vim)`  

**Q:** Match $digit$string  
**A:** `\$\d\$\S+`  

**Q:** Match IPv4  
**A:** `(\d{1,3}\.){3}\d{1,3}`  

**Q:** Match emails with groups  
**A:** `(\w+)@(\w+)\.com`   

---

## 🔹 Task 6: Conclusion

**Q:** Thanks!  
**A:** No answer needed  

---

## 🚀 Summary

Regex allows you to:
- Search complex patterns quickly
- Extract structured data (IPs, emails)
- Automate text processing

---

## ⚠️ Key Takeaways

- Be **specific but not overly complex**
- Use **metacharacters to simplify patterns**
- Groups and anchors make regex powerful
- Regex is essential for:
  - Log analysis
  - Data parsing
  - Security investigations

---

## 💡 Example Use Cases

- Extract emails from logs  
- Validate user input  
- Detect suspicious patterns  
- Parse network traffic  

---
