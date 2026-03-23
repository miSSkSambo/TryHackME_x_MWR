# 🏢 Active Directory Basics 

---
link to this room: https://tryhackme.com/room/winadbasics

---
## 📌 Overview

This room introduces the core concepts of **Active Directory (AD)**, the central system used by organisations to manage users, computers, and security policies in a Windows domain environment.

It explains how large networks are managed efficiently using:
- Domains
- Domain Controllers
- Organizational Units (OUs)
- Group Policies (GPOs)
- Authentication protocols

---

## 🎯 Learning Objectives

- Understand what Active Directory is
- Learn how Windows domains work
- Identify key AD components (Users, Groups, Machines)
- Understand Organizational Units (OUs) and Group Policies (GPOs)
- Learn authentication methods (Kerberos & NetNTLM)
- Understand Trees, Forests, and Trust relationships

---

## 🧠 Key Concepts

- **Active Directory (AD)**
- **Domain Controller (DC)**
- **Organizational Units (OUs)**
- **Security Groups**
- **Group Policy Objects (GPOs)**
- **Kerberos & NetNTLM**
- **SYSVOL Share**
- **Trees, Forests, Trusts**

---

# ✅ Questions and Answers

## 🔹 Task 1: Introduction

**Q:** Click and continue learning!  
**A:** No answer needed  

---

## 🔹 Task 2: Windows Domains

**Q:** In a Windows domain, credentials are stored in a centralised repository called...  
**A:** Active Directory  

**Q:** The server in charge of running the Active Directory services is called...  
**A:** Domain Controller  

---

## 🔹 Task 3: Active Directory

**Q:** Which group normally administrates all computers and resources in a domain?  
**A:** Domain Admins  

**Q:** What would be the name of the machine account associated with a machine named TOM-PC?  
**A:** TOM-PC$  

**Q:** Suppose our company creates a new department for Quality Assurance. What type of containers should we use to group all Quality Assurance users so that policies can be applied consistently to them?  
**A:** Organizational Units  

---

## 🔹 Task 4: Managing Users in AD

**Q:** What was the flag found on Sophie's desktop?  
**A:** THM{thanks_for_contacting_support}  

**Q:** The process of granting privileges to a user over some OU or other AD Object is called...  
**A:** delegation  

---

## 🔹 Task 5: Managing Computers in AD

**Q:** After organising the available computers, how many ended up in the Workstations OU?  
**A:** 7  

**Q:** Is it recommendable to create separate OUs for Servers and Workstations? (yay/nay)  
**A:** yay  

---

## 🔹 Task 6: Group Policies

**Q:** What is the name of the network share used to distribute GPOs to domain machines?  
**A:** sysvol  

**Q:** Can a GPO be used to apply settings to users and computers? (yay/nay)  
**A:** yay  

---

## 🔹 Task 7: Authentication Methods

**Q:** Will a current version of Windows use NetNTLM as the preferred authentication protocol by default? (yay/nay)  
**A:** nay  

**Q:** When referring to Kerberos, what type of ticket allows us to request further tickets known as TGS?  
**A:** Ticket Granting Ticket  

**Q:** When using NetNTLM, is a user's password transmitted over the network at any point? (yay/nay)  
**A:** nay  

---

## 🔹 Task 8: Trees, Forests and Trusts

**Q:** What is a group of Windows domains that share the same namespace called?  
**A:** Tree  

**Q:** What should be configured between two domains for a user in Domain A to access a resource in Domain B?  
**A:** A Trust Relationship  

---

## 🔹 Task 9: Conclusion

**Q:** Click and continue learning!  
**A:** No answer needed  

---

## 🚀 Summary

Active Directory is the backbone of enterprise networks, enabling:

- Centralised user and device management
- Secure authentication across systems
- Policy enforcement using GPOs
- Scalable network structures using Trees and Forests

This room builds a strong foundation for both:
- **Defensive Security (System Administration, Blue Team)**
- **Offensive Security (AD exploitation & privilege escalation)**

---
