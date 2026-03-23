# 📊 KQL (Kusto) Introduction 

---
link to the room: https://tryhackme.com/room/kqlkustointroduction
## 📌 Overview

This room introduces **Kusto Query Language (KQL)** and how it is used within **Microsoft Sentinel** to analyze security logs and detect threats.

KQL allows security analysts to:
- Search and filter large volumes of logs
- Detect suspicious activity
- Investigate incidents
- Perform threat hunting

It is a powerful tool for turning raw log data into actionable security insights.

---

## 🎯 Learning Objectives

- Understand Microsoft Sentinel as a SIEM + SOAR solution
- Learn what KQL is and how it works
- Understand KQL query structure and syntax
- Learn key KQL operators and functions
- Apply KQL in real-world security scenarios

---

## 🧠 Key Concepts

- **Kusto Query Language (KQL)**
- **Log Analytics Workspace**
- **Tables (SecurityEvent, Heartbeat, etc.)**
- **Operators (where, summarize, render, etc.)**
- **Pipelines ( | )**
- **Expressions**
- **Threat Hunting**
- **Security Log Analysis**

---

# ✅ Questions and Answers

## 🔹 Task 1: Introduction

**Q:** Let's go!  
**A:** No answer needed  

---

## 🔹 Task 2: Overview of Microsoft Sentinel

**Q:** In addition to being a SIEM solution, what else is Microsoft Sentinel? (use the abbreviation)  
**A:** SOAR  

**Q:** How does MS Sentinel support other security solutions that are not included in the built-in connectors?  
**A:** REST API Integration  

---

## 🔹 Task 3: What Is KQL

**Q:** What initial service was KQL created for?  
**A:** Azure Data Explorer  

**Q:** Analyze the example query from the task. How many computers will the query return?  
**A:** 10  

**Q:** What table is the example query retrieving its data from?  
**A:** Heartbeat  

---

## 🔹 Task 4: KQL Concepts in Microsoft Sentinel

**Q:** What operator can be used to output results in graphical form?  
**A:** render  

**Q:** What operator can be used to filter a specified table based on specified conditions?  
**A:** where  

**Q:** What user account name was queried in our second example query above?  
**A:** JBOX00$ :contentReference[oaicite:0]{index=0}  

---

## 🔹 Task 5: KQL Statement Structure

**Q:** What is the name of the table queried in our example query?  
**A:** SecurityEvent  

**Q:** Analyze the example query from the task. What does the query aggregate per computer?  
**A:** EventCount  

---

## 🔹 Task 6: KQL Use Cases

**Q:** What are we searching for in the SecurityEvent table on the first query?  
**A:** failed login attempts  

**Q:** Which operator was used on the second query to streamline our search to a range of user accounts from the TargetUserName column?  
**A:** Contains  

---

## 🔹 Task 7: Conclusion

**Q:** I am ready to learn more about KQL in the KQL (Kusto): Basic Queries room.  
**A:** No answer needed  

---

## 🚀 Summary

KQL is a powerful query language that allows security analysts to:

- Analyze massive amounts of log data
- Detect suspicious patterns and anomalies
- Investigate incidents efficiently
- Perform proactive threat hunting

When combined with Microsoft Sentinel, it becomes a **critical tool for modern cybersecurity operations**.

---
