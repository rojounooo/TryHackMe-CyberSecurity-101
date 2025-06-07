# TryHackMe: [Room Name]

> **Room URL:** [https://tryhackme.com/room/roomname](https://tryhackme.com/room/roomname)  
> **Difficulty:** [Easy | Medium | Hard]  
> **Category:** [e.g., Offensive Security, CTF, Web, Networking]  
> **Date Completed:** YYYY-MM-DD

---

## 🧠 Learning Objectives

- List key concepts or tools the room covers.
- For example:
  - Nmap scanning techniques
  - Exploiting buffer overflows
  - Privilege escalation methods

---

## 🧰 Tools & Techniques Used

- Nmap
- Gobuster
- Burp Suite
- John the Ripper
- [Add any relevant tools]

---

## 🚀 Enumeration

### 🔍 Nmap Scan

```bash
nmap -sC -sV -oN initial_scan.txt [IP]
```

**Results:**

- Port 22: OpenSSH 7.6p1
- Port 80: Apache HTTPD 2.4.29

[Include insights and observations.]

---

## 🌐 Web Enumeration (if applicable)

- Ran `gobuster` on `/`
- Found `/admin`, `/robots.txt`
- Used `whatweb`, `dirsearch`, etc.

---

## ⚙️ Exploitation

### Entry Point

- Vulnerability found in `CMS Made Simple`
- Used exploit `exploit.py` with credentials

```bash
python exploit.py -u http://[IP]/ -U admin -P password
```

---

## 🧗 Privilege Escalation

- Enumerated users with `linpeas.sh`
- Found SUID binary `/usr/bin/python` – used for root shell

```bash
python -c 'import pty;pty.spawn("/bin/bash")'
```

---

## 🧾 Flags

- **User Flag:** `THM{xxxxxxxxxxxxxxxxxxxx}`
- **Root Flag:** `THM{yyyyyyyyyyyyyyyyyyyy}`

---

## 📌 Notes & Lessons Learned

- Got stuck on X, but solved it by Y.
- Learned how to escalate via cronjob abuse.
- Need more practice with buffer overflows.

---

## 📸 Screenshots (Optional)

> Place screenshots in a `screenshots/` folder and embed like:

```markdown
![Nmap Scan](screenshots/nmap.png)
```

---

## ✅ Checklist

- [x] Enumeration
- [x] Exploitation
- [x] Privilege Escalation
- [x] Root access
- [x] Flags captured

---

## 🧩 References

- [Link to exploit DB]
- [Room’s walkthrough or writeup, if applicable]
