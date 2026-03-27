# 🎄 Advent of Cyber 2 (2020) — TryHackMe

---
link to the room: https://tryhackme.com/room/adventofcyber2

---
## 📌 Overview
A 25-day cybersecurity challenge covering:
- Web Exploitation
- Networking
- Forensics
- Privilege Escalation
- OSINT
- Reverse Engineering

---

## 🔹 Day 1

Q: What is the name of the cookie used for authentication?  
A: auth  

Q: In what format is the value of this cookie encoded?  
A: Hexadecimal  

Q: Having decoded the cookie, what format is the data stored in?  
A: JSON  

Q: What is the value of Santa's cookie?  
A: 7b22636f6d70616e79223a22546865204265737420466573746976616c20436f6d70616e79222c2022757365726e616d65223a2273616e7461227d  

---

## 🔹 Day 2

Q: What is the flag you're given when the line is fully active?  
A: THM{MjY0Yzg5NTJmY2Q1NzM1NjBmZWFhYmQy}  

---

## 🔹 Day 3

Q: What string of text needs adding to the URL to get access to the upload page?  
A: ?id=ODIzODI5MTNiYmYw  

Q: What type of file is accepted by the site?  
A: Image  

Q: In which directory are the uploaded files stored?  
A: /uploads/  

Q: What is the flag in /var/www/flag.txt?  
A: THM{MGU3Y2UyMGUwNjExYTY4NTAxOWJhMzhh}  

---

## 🔹 Day 4

Q: What is the flag?  
A: THM{885ffab980e049847516f9d8fe99ad1a}  

---

## 🔹 Day 5

Q: Given the URL "http://shibes.xyz/api.php", what would the entire wfuzz command look like to query the "breed" parameter using the wordlist "big.txt"?  
A: wfuzz -c -z file,big.txt http://shibes.xyz/api.php?breed=FUZZ  

---

## 🔹 Day 6

Q: Use GoBuster to find the API directory. What file is there?  
A: site-log.php  

Q: Fuzz the date parameter. What is the flag?  
A: THM{D4t3_AP1}  

---

## 🔹 Day 7

Q: Without using directory brute forcing, what's Santa's secret login panel?  
A: /santapanel  

Q: How many entries are there in the gift database?  
A: 22  

Q: What did Paul ask for?  
A: Github Ownership  

Q: What is the flag?  
A: thmfox{All_I_Want_for_Christmas_Is_You}  

---

## 🔹 Day 8

Q: What is admin's password?  
A: EhCNSWzzFP6sc7gB  

Q: What vulnerability type was used?  
A: Stored cross-site scripting  

Q: What query string can be abused?  
A: q  

Q: How many XSS alerts?  
A: 2  

---

## 🔹 Day 9

Q: What is the IP address that initiates ICMP?  
A: 10.11.3.2  

Q: What filter shows HTTP GET requests?  
A: http.request.method == GET  

Q: What article was visited?  
A: reindeer-of-the-week  

---

## 🔹 Day 10

Q: What FTP password was leaked?  
A: plaintext_password_fiasco  

Q: What protocol is encrypted?  
A: SSH  

---

## 🔹 Day 11

Q: What is on Elf McSkidy's wishlist?  
A: Rubber ducky  

Q: When was Snort created?  
A: 1998  

---

## 🔹 Day 12

Q: What ports are open?  
A: 80,2222,3389  

Q: What Linux distribution?  
A: Ubuntu  

Q: What is the HTTP title?  
A: Blog  

---

## 🔹 Day 13

Q: FTP directory?  
A: public  

Q: Script executed?  
A: backup.sh  

Q: Movie?  
A: The Polar Express  

Q: Flag?  
A: THM{even_you_can_be_santa}  

---

## 🔹 Day 14

Q: How many users on Samba?  
A: 3  

Q: How many shares?  
A: 4  

Q: Share without password?  
A: tbfc-santa  

Q: Directory?  
A: jingle-tunes  

---

## 🔹 Day 15

Q: PrivEsc type?  
A: Vertical  

Q: File containing sudo users?  
A: sudoers  

Q: Root flag?  
A: thm{2fb10afe933296592}  

---

## 🔹 Day 16

Q: Web server version?  
A: 9.0.17  

Q: CVE?  
A: CVE-2019-0232  

Q: Flag?  
A: thm{whacking_all_the_elves}  

---

## 🔹 Day 17

Q: Deprecated protocol?  
A: telnet  

Q: Credential?  
A: clauschristmas  

Q: OS version?  
A: Ubuntu 12.04  

---

## 🔹 Day 18

Q: Who got there first?  
A: grinch  

Q: Compile command?  
A: gcc -pthread dirty.c -o dirty -lcrypt  

Q: New username?  
A: firefart  

---

## 🔹 Day 19

Q: MD5 hash output?  
A: 8b16f00dd3b51efadb02c1df7f8427cc  

---

## 🔹 Day 20

Q: Reddit URL?  
A: https://www.reddit.com/user/IGuidetheClaus2020/comments  

Q: Where was he born?  
A: Chicago  

Q: Last name?  
A: May  

Q: Platform?  
A: Twitter  

Q: Username?  
A: IGuideClaus2020  

Q: Favourite show?  
A: Bachelorette  

Q: Parade location?  
A: Chicago  

Q: Coordinates?  
A: 41.891815, -87.624277  

Q: Flag?  
A: {FLAG}ALWAYSCHECKTHEEXIFD4T4  

---

## 🔹 Day 21

Q: Breached password?  
A: spygame  

Q: Hotel address number?  
A: 540  

---

## 🔹 Day 22

Q: True + True?  
A: 2  

Q: Python library database?  
A: PyPi  

Q: bool("False")?  
A: True  

Q: Library to download HTML?  
A: Requests  

Q: Output?  
A: [1, 2, 3, 6]  

Q: Cause?  
A: Pass by reference  

---

## 🔹 Day 23

Q: Web server port?  
A: 80  

Q: API directory?  
A: /api/  

Q: Santa location?  
A: Winter Wonderland, Hyde Park, London  

Q: API key?  
A: 57  

---

## 🔹 Day 24

Q: local_ch?  
A: 1  

Q: eax?  
A: 6  

Q: local_4h?  
A: 6  

---

## 🔹 Day 25

Q: Santa's password?  
A: santapassword321  

Q: Flag?  
A: thm{046af}  

---

## 🔹 FINAL

Q: What is the challenge flag?  
A: THM{EVERYONE_GETS_PRESENTS}  

---
