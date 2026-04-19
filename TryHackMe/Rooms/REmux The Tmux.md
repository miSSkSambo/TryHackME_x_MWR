# 🧵 REmux: The Tmux  
🔗 Link to the room: https://tryhackme.com/room/tmuxremux

---

## 📌 Overview  
This room teaches how to use **tmux**, a terminal multiplexer that allows you to manage multiple sessions, panes, and windows efficiently.

It covers:
- Sessions management  
- Pane splitting and navigation  
- Window handling  
- Copy mode  
- Custom configurations (`.tmux.conf`)  
- Plugins and workflow optimization  

---

## 🎯 Learning Objectives  
- Manage tmux sessions effectively  
- Work with panes and windows  
- Navigate and control terminal layouts  
- Use copy mode for extracting data  
- Customize tmux environment  
- Extend tmux using plugins  

---

## 🧠 Key Concepts  
- Sessions  
- Windows  
- Panes  
- Prefix Key (`Ctrl + b`)  
- Copy Mode  
- `.tmux.conf` Configuration  
- Plugins & Automation  

---

## ✅ Questions and Answers  

### 🔹 Task 1: Setup  
**Q:** Start the VM and connect  
**A:** No answer needed :contentReference[oaicite:0]{index=0}  

---

### 🔹 Task 2: Sessions  

**Q:** Do you hold Ctrl+B the whole time?  
**A:** nay :contentReference[oaicite:1]{index=1}  

**Q:** Start session named "thm"?  
**A:** tmux new -s thm :contentReference[oaicite:2]{index=2}  

**Q:** Change session name?  
**A:** ctrl b shift $ :contentReference[oaicite:3]{index=3}  

**Q:** Detach session?  
**A:** ctrl b d :contentReference[oaicite:4]{index=4}  

**Q:** List sessions?  
**A:** tmux ls :contentReference[oaicite:5]{index=5}  

**Q:** Reattach session "thm"?  
**A:** tmux a -t thm :contentReference[oaicite:6]{index=6}  

**Q:** Create session "kali" in background?  
**A:** tmux new -s kali -d :contentReference[oaicite:7]{index=7}  

**Q:** Switch sessions without detaching?  
**A:** ctrl b s :contentReference[oaicite:8]{index=8}  

**Q:** Kill session "thm"?  
**A:** tmux kill-session -t thm :contentReference[oaicite:9]{index=9}  

**Q:** Rename nested tmux session?  
**A:** ctrl b ctrl b shift $ :contentReference[oaicite:10]{index=10}  

**Q:** Enter tmux prompt?  
**A:** ctrl b shift : :contentReference[oaicite:11]{index=11}  

**Q:** Multiple ways to exit prompt?  
**A:** yea :contentReference[oaicite:12]{index=12}  

**Q:** Is tmux case sensitive?  
**A:** yea :contentReference[oaicite:13]{index=13}  

**Q:** Change directory in prompt to /opt?  
**A:** a -c /opt :contentReference[oaicite:14]{index=14}  

**Q:** Kill all sessions except "notes"?  
**A:** tmux kill-session -t notes -a :contentReference[oaicite:15]{index=15}  

---

### 🔹 Task 3: Panes  

**Q:** Split horizontally?  
**A:** ctrl b shift " :contentReference[oaicite:16]{index=16}  

**Q:** Close pane?  
**A:** exit :contentReference[oaicite:17]{index=17}  

**Q:** Split vertically?  
**A:** ctrl b shift % :contentReference[oaicite:18]{index=18}  

**Q:** Layout option 1?  
**A:** ctrl b esc 1 :contentReference[oaicite:19]{index=19}  

**Q:** Toggle layouts?  
**A:** ctrl b spacebar :contentReference[oaicite:20]{index=20}  

**Q:** Force kill pane?  
**A:** ctrl b x y :contentReference[oaicite:21]{index=21}  

**Q:** Switch between 2 panes?  
**A:** ctrl b ; :contentReference[oaicite:22]{index=22}  

**Q:** Arrow keys work?  
**A:** yea :contentReference[oaicite:23]{index=23}  

**Q:** Move pane clockwise?  
**A:** ctrl b shift { :contentReference[oaicite:24]{index=24}  

**Q:** Move pane counter-clockwise?  
**A:** ctrl b shift } :contentReference[oaicite:25]{index=25}  

**Q:** Show pane numbers?  
**A:** ctrl b q :contentReference[oaicite:26]{index=26}  

**Q:** Swap panes (move with it)?  
**A:** swap-pane -s 3 -t 1 :contentReference[oaicite:27]{index=27}  

**Q:** Swap panes (stay)?  
**A:** swap-pane -t 4 -s 1 :contentReference[oaicite:28]{index=28}  

---

### 🔹 Task 4: Windows  

**Q:** New window?  
**A:** ctrl b c :contentReference[oaicite:29]{index=29}  

**Q:** Rename window?  
**A:** ctrl b , :contentReference[oaicite:30]{index=30}  

**Q:** Move pane to new window?  
**A:** ctrl b shift ! :contentReference[oaicite:31]{index=31}  

**Q:** Join pane (source bash)?  
**A:** join-pane -s bash :contentReference[oaicite:32]{index=32}  

**Q:** Join pane (destination sudo)?  
**A:** join-pane -t sudo :contentReference[oaicite:33]{index=33}  

**Q:** Vertical join option?  
**A:** -v :contentReference[oaicite:34]{index=34}  

**Q:** Horizontal join option?  
**A:** -h :contentReference[oaicite:35]{index=35}  

**Q:** Can use window number?  
**A:** yea :contentReference[oaicite:36]{index=36}  

**Q:** Kill window?  
**A:** ctrl b shift & :contentReference[oaicite:37]{index=37}  

**Q:** View/switch windows?  
**A:** ctrl b w :contentReference[oaicite:38]{index=38}  

**Q:** Previous window?  
**A:** ctrl b p :contentReference[oaicite:39]{index=39}  

**Q:** Next window?  
**A:** ctrl b n :contentReference[oaicite:40]{index=40}  

---

### 🔹 Task 5: Copy Mode  

**Q:** Start copy mode?  
**A:** ctrl b [ :contentReference[oaicite:41]{index=41}  

**Q:** Search up?  
**A:** ctrl r :contentReference[oaicite:42]{index=42}  

**Q:** Search down?  
**A:** ctrl s :contentReference[oaicite:43]{index=43}  

**Q:** Exit search?  
**A:** esc :contentReference[oaicite:44]{index=44}  

**Q:** Exit copy mode?  
**A:** q :contentReference[oaicite:45]{index=45}  

**Q:** Highlight text?  
**A:** ctrl spacebar :contentReference[oaicite:46]{index=46}  

**Q:** Copy text?  
**A:** alt w :contentReference[oaicite:47]{index=47}  

**Q:** Paste text?  
**A:** ctrl b ] :contentReference[oaicite:48]{index=48}  

**Q:** View clipboard?  
**A:** ctrl b shift # :contentReference[oaicite:49]{index=49}  

---

### 🔹 Task 6: Config & Plugins  

**Q:** Default config exists?  
**A:** nay :contentReference[oaicite:50]{index=50}  

**Q:** Config examples path?  
**A:** /usr/share/doc/tmux :contentReference[oaicite:51]{index=51}  

**Q:** Use hex colors?  
**A:** yea :contentReference[oaicite:52]{index=52}  

**Q:** Config location?  
**A:** home :contentReference[oaicite:53]{index=53}  

**Q:** Reload config?  
**A:** source-file ~/.tmux.conf :contentReference[oaicite:54]{index=54}  

**Q:** Reset tmux?  
**A:** tmux kill-server :contentReference[oaicite:55]{index=55}  

**Q:** Add extra hotkeys?  
**A:** bind :contentReference[oaicite:56]{index=56}  

**Q:** Change prefix?  
**A:** set -g prefix C-a :contentReference[oaicite:57]{index=57}  

**Q:** Display shell output?  
**A:** yea :contentReference[oaicite:58]{index=58}  

**Q:** Load plugin?  
**A:** set -g @plugin :contentReference[oaicite:59]{index=59}  

**Q:** Run plugin?  
**A:** run-shell :contentReference[oaicite:60]{index=60}  

---

### 🔹 Task 7: Conclusion  
**Q:** git clone or fork it  
**A:** No answer needed :contentReference[oaicite:61]{index=61}  

---

## 🚀 Summary  

This room demonstrates how to:

- Manage multiple terminal sessions  
- Split and control panes efficiently  
- Work across multiple windows  
- Extract and reuse terminal output  
- Customize tmux for productivity  

---

## 🧠 Key Takeaway  

> tmux is a must-have tool for cybersecurity —  
> it enables efficient multitasking and persistent workflows.

---

## 🏁 Skills Gained  
- Linux Terminal Mastery  
- Workflow Optimization  
- Session Management  
- Productivity Tools  
- Automation Basics  
