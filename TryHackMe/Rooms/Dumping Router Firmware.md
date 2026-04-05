# 📡 Dumping Router Firmware 
---

link to the room: https://tryhackme.com/room/rfirmware

---
## 📖 Description

The **Dumping Router Firmware TryHackMe room** explores how embedded devices like routers operate internally by extracting and analyzing firmware images. It focuses on reverse engineering techniques used to uncover system details, configurations, and potential vulnerabilities.

The room covers:
- Extracting firmware using tools like binwalk  
- Analyzing firmware contents with strings  
- Understanding embedded Linux systems  
- Mounting and exploring filesystems (JFFS2)  
- Investigating router configurations and services  

---

## 🧪 Full Questions & Answers

**Q: Setup workspace and download firmware**  
**A:** No answer needed  

---

**Q: What does the first clear text line say?**  
**A:** Linksys WRT1900ACS Router  

---

**Q: What OS is the device running?**  
**A:** Linux  

---

**Q: What binwalk option extracts files?**  
**A:** -e  

---

**Q: What was the first extracted item?**  
**A:** uImage header  

---

**Q: What is the creation date?**  
**A:** 2020-04-22 11:07:26  

---

**Q: What is the CRC of the image?**  
**A:** 0xABEBC439  

---

**Q: What is the image size?**  
**A:** 4229755 bytes  

---

**Q: What architecture does the device run?**  
**A:** ARM  

---

**Q: Is that architecture correct?**  
**A:** Yes  

---

**Q: What Linux kernel version is included?**  
**A:** 3.10.39  

---

**Q: Where does linuxrc link to?**  
**A:** /bin/busybox  

---

**Q: What parent folder do mnt, opt, and var link to?**  
**A:** /tmp/  

---

**Q: Where is the HTTP server located?**  
**A:** /www/  

---

**Q: Most files in /bin link to what?**  
**A:** busybox  

---

**Q: What database runs in /bin?**  
**A:** sqlite3  

---

**Q: What is the build date?**  
**A:** 2020-04-22 11:44  

---

**Q: What SSH server is used?**  
**A:** dropbear  

---

**Q: Which company developed the media server?**  
**A:** Cisco  

---

**Q: Which file lists network services and ports?**  
**A:** services  

---

**Q: Which file contains default system settings?**  
**A:** system_defaults  

---

**Q: What is the firmware version?**  
**A:** 2.0.3.201002  

---

**Q: What three networks exist in /JNAP/modules?**  
**A:** guest_lan, lan, wan  

---

## 🧠 Key Takeaways

- Firmware analysis reveals **hidden system details and configs**  
- Tools like **binwalk and strings** are essential for reverse engineering  
- Routers often run **embedded Linux systems**  
- Misconfigurations can expose vulnerabilities  
- File systems like **JFFS2** are commonly used in embedded devices  
- Reverse engineering firmware is key in IoT security  

---

## 🚀 Skills Gained

- Firmware extraction and analysis  
- Embedded system investigation  
- Filesystem mounting (JFFS2)  
- Identifying services and configurations  
- Reverse engineering fundamentals  

---

