# 💽 MBR & GPT Analysis  
🔗 Link to the room: https://tryhackme.com/room/mbrandgptanalysis  

---

## 📌 Overview  
This room focuses on **disk forensics**, specifically analyzing **MBR (Master Boot Record)** and **GPT (GUID Partition Table)** structures.

It covers:
- Boot process fundamentals  
- MBR and GPT structures  
- Partition analysis  
- Malware attacks targeting boot process  
- Hands-on forensic scenarios  

---

## 🎯 Learning Objectives  
- Understand system boot process  
- Analyse MBR and GPT structures  
- Identify boot-level attacks (bootkits, ransomware, wipers)  
- Perform disk forensics using tools like HxD and FTK Imager  
- Recover corrupted boot records  

---

## 🧠 Key Concepts  
- MBR vs GPT  
- Boot Process (BIOS vs UEFI)  
- Partition Tables  
- Logical Block Addressing (LBA)  
- Bootkits  
- Disk Forensics  
- EFI System Partition  

---

## ✅ Questions and Answers  

### 🔹 Task 1: Introduction  

**Q:** What are the separate sections on a disk known as?  
**A:** partitions :contentReference[oaicite:0]{index=0}  

**Q:** Which type of malware infects the boot process?  
**A:** bootkits :contentReference[oaicite:1]{index=1}  

---

### 🔹 Task 2: Boot Process  

**Q:** What is the hardware diagnostic check called?  
**A:** Power-On-Self-Test :contentReference[oaicite:2]{index=2}  

**Q:** Which firmware supports GPT?  
**A:** UEFI :contentReference[oaicite:3]{index=3}  

**Q:** Which device contains the OS for booting?  
**A:** bootable device :contentReference[oaicite:4]{index=4}  

---

### 🔹 Task 3: MBR Analysis  

**Q:** Which component contains partition details?  
**A:** partition table :contentReference[oaicite:5]{index=5}  

**Q:** Standard sector size?  
**A:** 512 :contentReference[oaicite:6]{index=6}  

**Q:** Which component finds bootable partition?  
**A:** bootloader code :contentReference[oaicite:7]{index=7}  

**Q:** MBR magic number?  
**A:** 55 AA :contentReference[oaicite:8]{index=8}  

**Q:** Maximum partitions in MBR?  
**A:** 4 :contentReference[oaicite:9]{index=9}  

**Q:** Size of second partition (GB)?  
**A:** 16 :contentReference[oaicite:10]{index=10}  

---

### 🔹 Task 4: Threats Targeting MBR  
**Q:** Completed  
**A:** No answer needed  

---

### 🔹 Task 5: MBR Tampering Case  

**Q:** Number of partitions?  
**A:** 1 :contentReference[oaicite:11]{index=11}  

**Q:** First byte at starting LBA?  
**A:** EB :contentReference[oaicite:12]{index=12}  

**Q:** Partition type?  
**A:** NTFS :contentReference[oaicite:13]{index=13}  

**Q:** Partition size (GB)?  
**A:** 32 :contentReference[oaicite:14]{index=14}  

**Q:** Flag found?  
**A:** THM{Cure_The_MBR} :contentReference[oaicite:15]{index=15}  

---

### 🔹 Task 6: GPT Analysis  

**Q:** Number of partitions supported by GPT?  
**A:** 128 :contentReference[oaicite:16]{index=16}  

**Q:** Partition Type GUID of 2nd partition?  
**A:** E3C9E316-0B5C-4DB8-817D-F92DF00215AE :contentReference[oaicite:17]{index=17}  

---

### 🔹 Task 7: Threats Targeting GPT  
**Q:** Completed  
**A:** No answer needed  

---

### 🔹 Task 8: UEFI Bootkit Case  

**Q:** Which partition contains bootloader?  
**A:** EFI System Partition :contentReference[oaicite:18]{index=18}  

**Q:** Malicious string found?  
**A:** Hello, EFI Bootkit! :contentReference[oaicite:19]{index=19}  

---

## 🚀 Summary  

This room demonstrates:

- How systems boot using MBR and GPT  
- How attackers target boot processes  
- How to analyse disk structures using forensic tools  
- How to recover corrupted boot records  

---

## 🧠 Key Takeaway  

> Boot-level attacks are extremely dangerous because they execute **before the OS loads**, making them harder to detect and remove.

---

## 🏁 Skills Gained  
- Disk Forensics  
- Boot Process Analysis  
- Malware Investigation  
- Hex Analysis (HxD)  
- Incident Response  
