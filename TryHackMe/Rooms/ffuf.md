# ⚡ ffuf (Fuzz Faster U Fool)  
🔗 Link to the room: https://tryhackme.com/room/ffuf  

---

## 📌 Overview  
This room introduces **ffuf**, a fast web fuzzing tool used for:

- Directory brute forcing  
- Parameter fuzzing  
- Subdomain & vhost discovery  
- Web application enumeration  

It is commonly used in penetration testing to discover hidden resources and vulnerabilities.

---

## 🎯 Learning Objectives  
- Understand how ffuf works  
- Perform directory and file fuzzing  
- Use filters and matchers  
- Fuzz parameters and inputs  
- Discover subdomains and vhosts  
- Use advanced ffuf options  

---

## 🧠 Key Concepts  
- Fuzzing  
- Directory Enumeration  
- Wordlists (SecLists)  
- HTTP Status Codes  
- Filters & Matchers  
- Parameter Discovery  
- Virtual Hosts  

---

## ✅ Questions and Answers  

### 🔹 Task 1: Introduction  
**Q:** I have ffuf installed  
**A:** No answer needed  

**Q:** I have SecLists installed  
**A:** No answer needed  

---

### 🔹 Task 2: Basics  

**Q:** What is the first file you found with a 200 status code?  
**A:** favicon.ico :contentReference[oaicite:0]{index=0}  

---

### 🔹 Task 3: Finding Pages & Directories  

**Q:** What text file did you find?  
**A:** robots.txt :contentReference[oaicite:1]{index=1}  

**Q:** What two file extensions were found for the index page?  
**A:** php, phps :contentReference[oaicite:2]{index=2}  

**Q:** What page has a size of 4840?  
**A:** about.php :contentReference[oaicite:3]{index=3}  

**Q:** How many directories are there?  
**A:** 4 :contentReference[oaicite:4]{index=4}  

---

### 🔹 Task 4: Using Filters  

**Q:** After applying the fc filter, how many results were returned?  
**A:** 11 :contentReference[oaicite:5]{index=5}  

**Q:** After applying the mc filter, how many results were returned?  
**A:** 6 :contentReference[oaicite:6]{index=6}  

**Q:** Which valuable file would have been hidden using -fc 403?  
**A:** wp-forum.phps :contentReference[oaicite:7]{index=7}  

---

### 🔹 Task 5: Fuzzing Parameters  

**Q:** What parameter did you find?  
**A:** id :contentReference[oaicite:8]{index=8}  

**Q:** What is the highest valid id?  
**A:** 14 :contentReference[oaicite:9]{index=9}  

**Q:** What is Dummy’s password?  
**A:** p@ssword :contentReference[oaicite:10]{index=10}  

---

### 🔹 Task 6: Finding VHosts & Subdomains  
**Q:** I read the task material  
**A:** No answer needed  

---

### 🔹 Task 7: Proxifying Traffic  
**Q:** I understand how to proxy ffuf traffic  
**A:** No answer needed  

---

### 🔹 Task 8: Reviewing Options  

**Q:** How do you save output to a markdown file?  
**A:** -of md -o ffuf.md :contentReference[oaicite:11]{index=11}  

**Q:** How do you reuse a raw HTTP request file?  
**A:** -request :contentReference[oaicite:12]{index=12}  

**Q:** How do you strip comments from a wordlist?  
**A:** -ic :contentReference[oaicite:13]{index=13}  

**Q:** How do you read a wordlist from STDIN?  
**A:** -w - :contentReference[oaicite:14]{index=14}  

**Q:** How do you print full URLs and redirects?  
**A:** -v :contentReference[oaicite:15]{index=15}  

**Q:** What option follows redirects?  
**A:** -r :contentReference[oaicite:16]{index=16}  

**Q:** How do you enable color output?  
**A:** -c :contentReference[oaicite:17]{index=17}  

---

### 🔹 Task 9: Conclusion  
**Q:** Thank you  
**A:** No answer needed  

---

## 🚀 Summary  

This room teaches how to use ffuf for:

- Discovering hidden files and directories  
- Filtering useful results from noise  
- Identifying parameters and vulnerabilities  
- Performing brute-force attacks  
- Enumerating subdomains and vhosts  

---

## 🧠 Key Takeaway  

> ffuf is one of the fastest and most powerful tools for web enumeration —  
> mastering it significantly improves your penetration testing workflow.

---

## 🏁 Skills Gained  
- Web Enumeration  
- Directory Brute Forcing  
- Parameter Fuzzing  
- Security Testing  
- Tool Automation  
