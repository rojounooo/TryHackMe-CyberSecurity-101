# 🏫 TryHackMe Room: Defensive Security Intro

> Room URL: <a href="https://tryhackme.com/room/defensivesecurityintro"> Defensive Security Intro </a>

> Category: Defensive Security

> Difficulty: Easy


---

## 🗂️ Overview
This room aims to explain the foundations of defensive security, explaining its importance and topics falling under the umbrella of DefSec.

These topics are:
- Security Operations Center (**SOC**)
- Threat Intelligence (**IR**)
- Digital Forensics and Incident Response (**DFIR**)
- Malware Analysis (**MA**)
---

## 🧾 Section Summaries

### 📦 Task 1: Introduction to Defensive Security
**Concepts Covered**:
- What is Defensive Security
- What are the responsibilities


**My Notes**:
```
This task just explains the fundamentals of defensive security. It is the counterpart to offensive security.
- Two main tasks:
    - Preventing intrusions from happening 
    - Detecting an intrusion that has happened and responding accordingly
- Blue teams are a core part of defensive security 
- Subtasks include:
    - Providing cybersecurity training for employees 
    - Documenting and managing assets. Make sure everything is protected adequately
    - Updating and patching regularly, systems running older versions of software are more likely to be exploited
    - Setting up protective security devices such as **Firewalls** and **IPS** (Intrusion Prevention System)
    - Setting up logging and monitoring devices. Malicious activities can be logged for later analysis
```
---

### ⚙️ Task 2: Areas of Defensive Security
**Concepts Covered**:
- Covers the topics I included above

**My Notes**:
```
- SOC:
    - A team of professionals that monitor networks and systems to detect malicious events
    Main Responsibilities include:
        - If a vulnerability is discovered, issue a proper update or patch. If no update or patch is available take necessary measures to prevent exploitation.
        - Implement a security policy for employees to follow
        - If unauthorized activity is detected e.g. due to credentials being stolen, block events asap
        - Detect intrusions asap to prevent further damage such as ransomware or priv esc.
```

```
- TI: 
Threat Intelligence falls under the responsibilities of a SOC team
    - Information gathered about possible malicious actors.
    - Aims to achieve a "threat-informed defense" 
    - Different companies have different adversaries so defenses will be more company specific
    - Data is collected from logs and forums and then processed into a format for analysis
    - Analysis aims to find out more info about attackers and their motives
    - Learning about malicious actors lets you know their Tactics, Techniques and Procedures (**TTP**)
```

```
DF: 
    - Digital Forensics investigates digital evidence to uncover facts about cyber incidents.
    - Involves analyzing digital copies of storage, memory, logs, and network traffic.
    - Used to investigate crimes like data theft, cyber espionage, and unauthorized content possession.
    - File System: Reveals created, modified, deleted, or partially overwritten files.
    - System Memory: Useful when malware operates only in RAM.
    - System Logs: Show system events; some traces often remain despite attacker efforts to clear them.
    - Network Logs: Help detect and understand attack vectors and communication patterns.
```
```
IR:
Incident Response outlines how to manage and mitigate cyber attacks effectively.

    - Goal: Minimize damage and recover quickly.
    - Preparation: Establish trained teams and preventive measures.
    - Detection and Analysis: Identify and evaluate the severity of incidents.
    - Containment, Eradication, Recovery: Stop the spread, eliminate threats, and restore systems.
    - Post-Incident Activity: Document findings and share lessons learned to improve future responses.
```

MA:
Malware Analysis is the process of examining malicious software to understand its behavior and impact. It falls under DF

    - Virus: Attaches to files and spreads, causing file damage and system issues.
    - Trojan Horse: Disguises itself as legitimate software while performing malicious actions.
    - Ransomware: Encrypts files and demands payment for decryption.
    - Static Analysis: Inspects malware without execution—requires assembly knowledge.
```
---

## 🧠 Key Takeaways

- DefSec is a wide spanning branch of Cybersecurity, ranging from monitoring networks to responding to incidents and reverse engineering malware. It's not just systems that need to be protected but policies and training need to be put in place for employees and users of any software. Patching and updating is critical and should always be done asap to reduce an exploitation window.
---


