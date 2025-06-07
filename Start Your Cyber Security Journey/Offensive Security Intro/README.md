# TryHackMe: Offensive Security Intro

> **Room URL:** [https://tryhackme.com/room/offensivesecurityintro](https://tryhackme.com/room/offensivesecurityintro)  
> **Difficulty:** Easy  
> **Category:** Offensive Security  
---

## 🧠 Learning Objectives
  - Explanation of offensive security
  - Linux Terminal
  - Gobuster
 

---

## 🧰 Tools & Techniques Used

- Gobuster

---

## 🚀 Enumeration

### 🔍 Gobuster Scan

```bash
gobuster -u http://fakebank.thm -w wordlist.txt dir
```

**Results:**

- /images
- /bank-transfer

---

## ⚙️ Exploitation

### Entry Point

- Navigate to http://fakebank.thm/bank-transfer
- Fill in details 
- Transfer $2000

---

## 🧾 Flags

- **Flag:** `BANK-HACKED`

---

## 📌 Notes & Lessons Learned

- Learnt how to enumerate a websites subdirectories using gobuster 

---

## 📸 Screenshots (Optional)

> Place screenshots in a `screenshots/` folder and embed like:

```markdown
![Gobuster Scan](screenshots/gobuster.png)
```

---

## ✅ Checklist

- [✅] Enumeration
- [✅] Exploitation
- [✅] Flags captured

---
