# 🔐 Snyk Open Source S

---

🔗 Room Link: https://tryhackme.com/room/snykopensource

---

## 📖 Overview

The **Snyk Open Source room** focuses on understanding how to **identify, analyse, and remediate vulnerabilities in open-source dependencies**.

It teaches how modern development teams:

- Detect vulnerabilities in dependencies  
- Prioritise risks using severity metrics  
- Fix issues securely without breaking systems  
- Integrate security into CI/CD pipelines  

---

## 🎯 What You Learn

### 🔍 Dependency Security
- Analyse `package.json` files  
- Identify outdated and vulnerable libraries  
- Understand dependency risks  

### 🧠 Vulnerability Analysis
- Use Snyk dashboards and IDE plugins  
- Interpret severity levels and CVSS scores  
- Understand real-world vulnerabilities  

### ⚔️ Exploitation Concepts
- Learn how vulnerabilities like:
  - Prototype Pollution  
  - Directory Traversal  
  can be abused  

### 🛡️ Secure Development
- Apply remediation strategies  
- Prioritise high-risk vulnerabilities  
- Integrate security into CI/CD pipelines  

---

## 🧪 Scenario Summary

You act as a **junior security engineer (Jessica)** tasked with improving security:

1. Analyse a Node.js project (`package.json`)  
2. Identify vulnerable dependencies  
3. Use Snyk to scan the project  
4. Investigate vulnerabilities  
5. Apply fixes and improvements  
6. Automate security using CI/CD  

---

## ⚠️ Key Concept Highlight

### Transitive Dependencies

- Dependencies that rely on other dependencies  
- Can introduce hidden vulnerabilities  
- Hard to track without proper tools  

---

# 📌 FULL QUESTIONS & ANSWERS

---

## 🧩 Task 1: Introduction

**Q:** Read the above and move onto task two!  
**A:** No answer needed  

---

## 🧩 Task 2: Meet Jessica

**Q:** Ready? Let’s get going!  
**A:** No answer needed  

---

## 🧩 Task 3: Understanding Open Source Security Risks

**Q:** Which JSON-formatted manifest file serves as the central hub for Node.js projects, listing metadata, scripts, and dependency declarations?  
**A:** `package.json`  

**Q:** How many dependencies do we have for this new feature?  
**A:** 5  

**Q:** Which term describes indirect package dependencies formed through shared prerequisites, possibly concealing vulnerabilities and demanding cautious assessment?  
**A:** Transitive dependencies  

---

## 🧩 Task 4: Getting Started with Snyk Open Source

**Q:** What single authentication mechanism allows users to transition smoothly amongst various linked platforms and services?  
**A:** Single Sign-On  

---

## 🧩 Task 5: Diving Deeper Into Vulnerabilities

**Q:** What is the version of the vulnerable lodash package?  
**A:** 2.4.2  

**Q:** Which vulnerability allows an attacker to modify an Object?  
**A:** Prototype Pollution  

---

## 🧩 Task 6: Remediating Vulnerabilities

**Q:** What does CVSS stand for?  
**A:** Common Vulnerability Scoring System  

**Q:** Should the development team bulk fix all the vulnerabilities found in this new feature? (y/n)  
**A:** n  

---

## 🧩 Task 7: Automating the Process Through CI/CD Pipelines

**Q:** How does CircleCI help streamline pipeline configuration and standardisation?  
**A:** Orb  

**Q:** What file defines the GitHub Actions workflow configuration that enables automation and customised sequences for building, testing, and deploying?  
**A:** YAML  

---

## 🧩 Task 8: Implementing Continuous Monitoring

**Q:** Which collaborative DevOps practice combines real-time communication channels, automation, and operational agility?  
**A:** ChatOps  

---

## 🧩 Task 9: Establishing Best Practices

**Q:** Well done Jessica, she did it!  
**A:** No answer needed  

---

## 🧠 Key Takeaways

- Open-source dependencies are a **major attack surface**  
- Snyk helps detect vulnerabilities early  
- Always prioritise **high-severity vulnerabilities**  
- Avoid bulk fixes without testing  
- CI/CD integration is essential for modern security  
- Continuous monitoring prevents regressions  

---

## 💻 Example Vulnerabilities

### Prototype Pollution
- Allows attackers to modify object behaviour  
- Can lead to:
  - Data manipulation  
  - Denial of Service  
  - Information leaks  

### Directory Traversal
- Uses `../` to access restricted files  
- Can expose sensitive system data  

---

## 🚀 Tools Used

- Snyk  
- GitHub  
- Visual Studio Code  
- Node.js  

---

## 📂 Repository Purpose

This repository documents:

- Full walkthrough answers  
- Vulnerability explanations  
- Security best practices  
- DevSecOps integration using Snyk  

---
