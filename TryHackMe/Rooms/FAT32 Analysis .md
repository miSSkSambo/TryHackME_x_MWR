# 💾 FAT32 Analysis  
🔗 Link to the room: https://tryhackme.com/room/fat32analysis  

---

## 📌 Overview  
This room focuses on **FAT32 filesystem forensics**, teaching how data is stored, analyzed, and recovered.

It covers:
- FAT32 structure (Boot Sector, FAT, Data Area)
- Forensic analysis techniques
- Data recovery from deleted files
- Detection of attacker techniques (MITRE ATT&CK)

---

## 🎯 Learning Objectives  
- Understand FAT32 filesystem structure  
- Perform forensic analysis on FAT32 images  
- Recover deleted and hidden files  
- Detect attacker techniques like timestomping  
- Use tools like Autopsy and HxD  

---

## 🧠 Key Concepts  
- FAT32 Structure (Reserved Area, FAT, Data Area)  
- Cluster Chains  
- Root Directory (LFN & SFN entries)  
- Hidden Files & Attributes  
- Timestomping  
- File Deletion & Recovery  
- Slack Space & Data Carving  

---

## ✅ Questions and Answers  

### 🔹 Task 1: Introduction  
**Q:** Are you ready to start analyzing FAT32?  
**A:** No answer needed  

---

### 🔹 Task 2: Environment and Setup  
**Q:** Boot up the VM and continue with the next task.  
**A:** No answer needed  

---

### 🔹 Task 3: FAT32 Relevancy  
**Q:** What is the name of the attack that targeted the Iranian nuclear program?  
**A:** Stuxnet :contentReference[oaicite:0]{index=0}  

**Q:** What category of tactic is MITRE ATT&CK TA0005?  
**A:** Defense Evasion :contentReference[oaicite:1]{index=1}  

---

### 🔹 Task 4: FAT32 Structure (Reserved & FAT Areas)  
**Q:** What would be the value of the FAT entry at cluster F?  
**A:** 10000000 :contentReference[oaicite:2]{index=2}  

**Q:** At which offset does FAT2 start?  
**A:** 00387E00 :contentReference[oaicite:3]{index=3}  

---

### 🔹 Task 5: FAT32 Data Area  
**Q:** What is the filename of the file that starts at cluster 9?  
**A:** careers.txt :contentReference[oaicite:4]{index=4}  

**Q:** What is the creation time (hex)?  
**A:** F484 :contentReference[oaicite:5]{index=5}  

---

### 🔹 Task 6: Analysis Techniques  
**Q:** Which technique is used to find hidden files?  
**A:** Directory Structure and File Name Analysis :contentReference[oaicite:6]{index=6}  

---

### 🔹 Task 7: Hidden Files  
**Q:** What is the short file name of the hidden file?  
**A:** BEMYVA~1 :contentReference[oaicite:7]{index=7}  

**Q:** What is the flag found?  
**A:** THM{F0uNdTh3H!Dd3nF1l3} :contentReference[oaicite:8]{index=8}  

---

### 🔹 Task 8: Timestomp  
**Q:** What is the accessed timestamp of the suspicious file?  
**A:** 2018-01-10 00:00:00 :contentReference[oaicite:9]{index=9}  

**Q:** What is the flag found?  
**A:** THM{T1m3St0Mp3D} :contentReference[oaicite:10]{index=10}  

---

### 🔹 Task 9: File Deletion  
**Q:** Which hex value identifies a deleted file?  
**A:** E5 :contentReference[oaicite:11]{index=11}  

**Q:** What is the output of the recovered script?  
**A:** THM{r3Tr!3v3D_3v!d3nC3} :contentReference[oaicite:12]{index=12}  

---

### 🔹 Task 10: Challenge  

**Q:** FAT1 offset?  
**A:** 0020FC00 :contentReference[oaicite:13]{index=13}  

**Q:** Hidden directory name?  
**A:** Exfiltrated_data :contentReference[oaicite:14]{index=14}  

**Q:** Flag in hidden directory?  
**A:** THM{D@t@3xf!lL} :contentReference[oaicite:15]{index=15}  

**Q:** Archive file size?  
**A:** 10862 :contentReference[oaicite:16]{index=16}  

**Q:** Deleted file name?  
**A:** Reverseshell.py :contentReference[oaicite:17]{index=17}  

**Q:** Flag in deleted file?  
**A:** THM{B@ckD00rF0unD} :contentReference[oaicite:18]{index=18}  

**Q:** File with suspicious timestamps?  
**A:** Legal_Affairs_Notes.txt :contentReference[oaicite:19]{index=19}  

**Q:** Flag in suspicious file?  
**A:** THM{D@t@g@tH3r!nG} :contentReference[oaicite:20]{index=20}  

---

### 🔹 Task 11: Conclusion  
**Q:** Are you ready for the next filesystem?  
**A:** No answer needed  

---

## 🚀 Summary  
This room builds strong foundational skills in **filesystem forensics**, specifically:

- Understanding FAT32 internal structure  
- Identifying hidden and deleted files  
- Detecting attacker techniques (timestomping, defense evasion)  
- Recovering forensic artifacts  
- Using tools like Autopsy for efficient investigations  

These skills are essential for:
- Digital Forensics  
- SOC Analysis  
- Incident Response  
- Threat Hunting  
