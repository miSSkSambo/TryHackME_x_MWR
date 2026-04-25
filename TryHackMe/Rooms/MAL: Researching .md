# 🦠 MAL: Researching  
🔗 Link to the room: https://tryhackme.com/room/malresearching  

---

## 📌 Overview  
This room focuses on **malware research fundamentals**, teaching how analysts identify and investigate potentially malicious files using:

- Cryptographic checksums (hashes)  
- File integrity verification  
- Online sandboxing platforms  
- Threat intelligence tools like VirusTotal  

It combines **theory + practical analysis**, helping build a strong foundation in malware investigation.

---

## 🎯 Learning Objectives  
- Understand how checksums (hashes) work  
- Learn why hashes are important in malware analysis  
- Generate MD5, SHA256, and SHA512 hashes  
- Analyse malware safely using sandbox environments  
- Investigate malware reports using VirusTotal  
- Interpret behaviour such as network activity and file actions  

---

## 🧠 Key Concepts  
- Checksums / Hashes  
- MD5, SHA-256, SHA-512  
- Hash Collisions  
- Malware Sandboxing  
- Threat Intelligence  
- File Integrity Verification  
- Static vs Dynamic Analysis  

---

## 🛠️ Tools Used  
- PowerShell (`Get-FileHash`, `CertUtil`)  
- HashTab  
- VirusTotal  
- Hybrid Analysis  
- Any.run  

---

## ✅ Questions and Answers  

### 🔹 Task 1: Intro  
**Q:** Let’s go!  
**A:** No answer needed  

---

### 🔹 Task 2: Deploy  
**Q:** I’ve deployed my instance and ensured I am connected to the THM VPN!  
**A:** No answer needed  

---

### 🔹 Task 3: Checksums  

**Q:** Name the term for an individual piece of binary  
**A:** Bit  

**Q:** What are checksums also known as?  
**A:** Hashes  

**Q:** Name the algorithm that is next in the series after SHA-256  
**A:** SHA-512  

**Q:** According to this task, how long will you need to hash 6 million files before a MD5 hash collision occurs?  
**A:** 100 Years  

**Q:** Who developed the MD5 algorithm?  
**A:** Ronald Rivest  

---

### 🔹 Task 4: Online Sandboxing  

**Q:** Name the key term for the type of malware that Emotet is classified as  
**A:** Trojan  

**Q:** What type of emails does Emotet use as its payload?  
**A:** spam emails  

**Q:** Timestamp of analysis?  
**A:** 9/16/2019, 13:54:48  

**Q:** File detected as a Network Trojan?  
**A:** easywindow.exe  

**Q:** PID of first HTTP GET request?  
**A:** 2748  

**Q:** DNS request made?  
**A:** blockchainjoblist.com  

---

### 🔹 Task 5: Practical (Checksums)  

**Q:** MD5 checksum of LoginForm.exe?  
**A:** FF395A6D528DC5724BCDE9C844A0EE89  

**Q:** SHA256 of TryHackMe.exe?  
**A:** 6F870C80361062E8631282D31A16872835F7962222457730BC55676A61AD1EE0  

**Q:** CertUtil syntax for SHA256?  
**A:** CertUtil -hashfile TryHackMe.exe SHA256  

---

### 🔹 Task 6: VirusTotal  

**Q:** Other filename detected?  
**A:** HxD.exe  

**Q:** Compilation timestamp?  
**A:** 2020-02-28 11:16:36  

**Q:** Flag?  
**A:** THM{TryHackMe_Malware_Series_Research_Flag}  

---

### 🔹 Task 7: Conclusion  
**Q:** Thanks! I’ll stay tuned  
**A:** No answer needed  

---

## 🚀 Summary  

This room teaches how malware analysts:

- Use hashes to uniquely identify files  
- Detect malicious behaviour through sandbox reports  
- Analyse network activity and file execution  
- Use platforms like VirusTotal for threat intelligence  

---

## 🧠 Key Takeaway  

> Hashes act like fingerprints for files —  
> they allow analysts worldwide to identify and track malware quickly and reliably.

---

## 🏁 Skills Gained  
- Malware Analysis Fundamentals  
- Hash Generation & Verification  
- Threat Intelligence Usage  
- Sandbox Analysis  
- Security Research Techniques  
