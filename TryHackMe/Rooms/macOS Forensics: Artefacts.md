# 🍎 macOS Forensics: Artefacts  
🔗 Link to the room: https://tryhackme.com/room/macosforensicsartefacts  

---

## 📌 Overview  
This room focuses on **macOS forensic artefacts** and how investigators extract valuable evidence from a system.

It builds on basic macOS forensics and explores:

- System artefacts  
- Network artefacts  
- User activity  
- File system evidence  
- Connected devices  

---

## 🎯 Learning Objectives  
- Identify key macOS forensic artefacts  
- Locate artefacts on disk images and live systems  
- Use tools to parse plist files, logs, and databases  
- Analyse user activity and system events  
- Investigate file system and device connections  

---

## 🧠 Key Concepts  
- Plist Files  
- SQLite Databases  
- System Logs (ASL, Unified Logs)  
- User Activity Tracking  
- File System Events  
- Network Artefacts  
- Digital Evidence Analysis  

---

## 🛠️ Tools Used  
- `apfs-fuse`  
- `plistutil`  
- DB Browser for SQLite  
- APOLLO  
- mac_apt  
- Unified Log Parser  
- Linux CLI tools  

---

## ✅ Questions and Answers  

### 🔹 Task 1: Introduction  

**Q:** What command can be used to mount the image named mac-disk.img to the directory ~/mac?  
**A:** apfs-fuse -v 4 mac-disk.img ~/mac  

---

### 🔹 Task 2: Before We Begin  

**Q:** Which utility can we use to parse plist files in the attached VM?  
**A:** plistutil  

---

### 🔹 Task 3: System Information  

**Q:** When was the OS installed? (YYYY-MM-DD hh:mm:ss)  
**A:** 2024-12-08 17:42:28  

**Q:** What is the country code for this machine?  
**A:** AE  

**Q:** When was the last boot time (GMT)?  
**A:** 2025-01-19 15:47:05  

---

### 🔹 Task 4: Network Information  

**Q:** What is the built-in network interface?  
**A:** en0  

**Q:** What is the router IP address?  
**A:** 192.168.64.1  

---

### 🔹 Task 5: Account Activity  

**Q:** What is the name of the last logged-in user?  
**A:** thm  

**Q:** What is the password hint?  
**A:** count to 5  

**Q:** When was the last logout? (MMM DD hh:mm:ss)  
**A:** Jan 19 07:52:43  

---

### 🔹 Task 6: Evidence of Execution  

**Q:** What was the last command executed?  
**A:** vim creds.txt  

**Q:** What is the terminal session GUID?  
**A:** 452AEA93-AEE7-420B-871E-C57053E15DD0  

**Q:** When was the terminal last closed?  
**A:** 2025-01-19 15:52:33  

**Q:** How long was the terminal in focus (seconds)?  
**A:** 176  

---

### 🔹 Task 7: File System Activity  

**Q:** What are the viewing options for the Users/thm folder?  
**A:** Open in list view  

**Q:** What is the last directory visited?  
**A:** Recents  

---

### 🔹 Task 8: Connected Devices  

**Q:** Which stream contains Bluetooth connection info?  
**A:** Bluetooth/isConnected  

---

### 🔹 Task 9: Conclusion  

**Q:** Yoohoo! I loved exploring macOS Forensics!  
**A:** No answer needed  

---

## 🚀 Summary  

This room demonstrates how to:

- Mount and analyse macOS disk images  
- Extract system, network, and user artefacts  
- Investigate logs and databases  
- Track user activity and executed commands  
- Identify connected devices and file system changes  

---

## 🧠 Key Takeaway  

> macOS stores a vast amount of forensic evidence —  
> knowing where to look is key to successful investigations.

---

## 🏁 Skills Gained  
- macOS Forensics  
- Artefact Analysis  
- Log Investigation  
- Disk Image Analysis  
- Evidence Correlation  
