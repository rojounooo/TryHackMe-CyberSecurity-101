# 🚩 TryHackMe Room Walkthrough: Defensive Security Intro

> Room URL: <a href="https://tryhackme.com/room/defensivesecurityintro"> Defensive Security Intro</a>

---

## 🧑‍💻 Environment Setup

- Machine in room setup ✅

---

## 📌 Task Walkthrough

### 🧩 Task [2]: Areas of Defensive Security
> **Question 1:** What would you call a team of cyber security professionals that monitors a network and its systems for malicious events?

<details>
<summary><strong>Answer</strong></summary>
    Security Operations Center
</details>

> **Question 2:** What does DFIR stand for?

<details>
<summary><strong>Answer</strong></summary>
    Digital Forensics and Incident Response
</details>

> **Question 3:** Which kind of malware requires the user to pay money to regain access to their files?

<details>
<summary><strong>Answer</strong></summary>
    Ransomware
</details>

### 🧩 Task [3]: Practical Example of Defensive Security

**Steps Taken:**
- Find malicious IP address 
    `143.110.250.149`
- Click on alert
- Check if IP address is malicious or suspicious 
- Confirmed malicious IP address
- Escalate to SOC Team Lead
- Block IP address
- Get Flag

**Explanation:**
```
By taking note of the malicious IP address we can block future packets arriving from it 
We escalate to SOC lead to determine which steps we need to take next 
Blocking the IP Address prevents further packets, the firewall will check the SRC address to determine whether to drop the packet or not
```
> **Question** What is the flag that you obtained by following along?

<details>
<summary><strong>Flag</strong></summary>
    THM{THREAT-BLOCKED}
</details>

---
## 📊 Summary

- Total Flags: 1
- Difficulty: Easy
- Time Taken: 10 minutes
- Notes: Firewall Rules

---

## 📝 Personal Reflections

I learned about different roles in DefSec and the steps to respond to an incident
