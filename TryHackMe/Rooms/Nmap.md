# 🛡️ TryHackMe: Nmap Room (Full Questions & Answers)

---
link to the room: https://tryhackme.com/room/furthernmap

---

## Task 2 – Introduction

### ❓ What networking constructs are used to direct traffic to the right application on a server?
### ✅ Answer
Ports

---

### ❓ How many of these are available on any network-enabled computer?
### ✅ Answer
65535

---

### ❓ How many of these are considered "well-known" (standard ports)?
### ✅ Answer
1024

---

## Task 3 – Nmap Switches

### ❓ What is the first switch listed in the help menu for a "Syn Scan"?
### ✅ Answer
-sS

---

### ❓ Which switch would you use for a UDP scan?
### ✅ Answer
-sU

---

### ❓ If you wanted to detect which operating system the target is running on, which switch would you use?
### ✅ Answer
-O

---

### ❓ Which switch is used to detect the version of services running on the target?
### ✅ Answer
-sV

---

### ❓ How would you increase the verbosity of Nmap output?
### ✅ Answer
-v

---

### ❓ How would you set verbosity level to two?
### ✅ Answer
-vv

---

### ❓ What switch would you use to save Nmap results in all major formats?
### ✅ Answer
-oA

---

### ❓ What switch saves results in normal format?
### ✅ Answer
-oN

---

### ❓ What switch saves results in grepable format?
### ✅ Answer
-oG

---

### ❓ How would you enable aggressive mode in Nmap?
### ✅ Answer
-A

---

### ❓ How would you set timing template level 5?
### ✅ Answer
-T5

---

### ❓ How would you scan only port 80?
### ✅ Answer
-p 80

---

### ❓ How would you scan ports 1000 to 1500?
### ✅ Answer
-p 1000-1500

---

### ❓ How would you scan all ports?
### ✅ Answer
-p-

---

### ❓ How would you activate an NSE script?
### ✅ Answer
--script

---

### ❓ How would you run all scripts in the "vuln" category?
### ✅ Answer
--script=vuln

---

## Task 5 – TCP Connect Scans

### ❓ Which RFC defines the appropriate behaviour for the TCP protocol?
### ✅ Answer
RFC 9293

---

### ❓ If a port is closed, which flag should the server send back?
### ✅ Answer
RST

---

## Task 6 – SYN Scans

### ❓ What are the two other names for a SYN scan?
### ✅ Answer
Half-Open, Stealth

---

### ❓ Can Nmap use a SYN scan without sudo permissions (Y/N)?
### ✅ Answer
N

---

## Task 7 – UDP Scans

### ❓ If a UDP port doesn't respond to an Nmap scan, what will it be marked as?
### ✅ Answer
open|filtered

---

### ❓ When a UDP port is closed, which protocol sends the "port unreachable" message?
### ✅ Answer
ICMP

---

## Task 8 – NULL, FIN, Xmas Scans

### ❓ Which scan type uses the URG flag?
### ✅ Answer
xmas

---

### ❓ Why are NULL, FIN and Xmas scans generally used?
### ✅ Answer
Firewall Evasion

---

### ❓ Which operating system may respond with RST for all ports?
### ✅ Answer
Microsoft Windows

---

## Task 9 – ICMP Network Scanning

### ❓ How would you perform a ping sweep on the 172.16.x.x network (CIDR notation)?
### ✅ Answer
nmap -sn 172.16.0.0/16

---

## Task 10 – NSE Scripts Overview

### ❓ What language are NSE scripts written in?
### ✅ Answer
Lua

---

### ❓ Which category of scripts is unsafe for production environments?
### ✅ Answer
intrusive

---

## Task 11 – Working with NSE

### ❓ What optional argument can the ftp-anon.nse script take?
### ✅ Answer
maxlist

---

## Task 12 – Searching for Scripts

### ❓ What is the filename of the script that determines the OS of an SMB server?
### ✅ Answer
smb-os-discovery.nse

---

### ❓ What does this script depend on?
### ✅ Answer
smb-brute

---

## Task 13 – Firewall Evasion

### ❓ Which protocol is often blocked, requiring the use of the -Pn switch?
### ✅ Answer
ICMP

---

### ❓ Which switch allows you to append random data to packets?
### ✅ Answer
--data-length

---

## Task 14 – Practical

### ❓ Does the target IP respond to ICMP (ping) requests (Y/N)?
### ✅ Answer
N

---

### ❓ How many ports are open|filtered in the Xmas scan (first 999 ports)?
### ✅ Answer
999

---

### ❓ What is the reason given for this result?
### ✅ Answer
No Response

---

### ❓ How many ports are open in the TCP SYN scan (first 5000 ports)?
### ✅ Answer
5

---

### ❓ Can Nmap successfully log into FTP anonymously (Y/N)?
### ✅ Answer
Y

---

## 🚀 Notes
- Always perform enumeration before exploitation  
- Use SYN scans for stealth  
- Save scan results for reporting  
- NSE scripts are powerful for automation  

---

