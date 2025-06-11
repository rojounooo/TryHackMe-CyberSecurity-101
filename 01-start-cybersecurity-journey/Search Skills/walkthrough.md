# 🚩 TryHackMe Room Walkthrough: Search Skills

> Room URL: <a href="https://tryhackme.com/room/searchskills"> Search Skills </a>

---

## 🧑‍💻 Environment Setup

- N/A

---

## 📌 Task Walkthrough

### 🧩 Task 2: Evaluation of Search Results
> **Question:** What do you call a cryptographic method or product considered bogus or fraudulent?

**Steps Taken:**
Search for the answer

**Explanation:**
The answer is not provided in the room it has to be searched for.

<details>
    <summary><strong>Answer</strong></summary>
        snake oil
</details>

> **Question:** What is the name of the command replacing `netstat` in Linux systems?

**Steps Taken:**
Search for the answer

**Explanation:**
The answer is not provided in the room it has to be searched for.

<details>
    <summary><strong>Answer</strong></summary>
        ss
</details>
---

### 🧩 Task 3: Search Results
> **Question:** How would you limit your Google search to PDF files containing the terms cyber warfare report?

**Steps Taken:**
-Using Google: 
    - Search for filetype:pdf cyber warfare report

**Explanation:**
We specifically want PDFs so we want to use **filetype:** we could also use **exact phrase** as well but it is not needed here.

<details>
    <summary><strong>Answer</strong></summary>
        filetype:pdf cyber warfare report
</details>

> **Question:** What phrase does the Linux command ss stand for?

**Steps Taken:**
Search for "What phrase does the linux command "ss" stand for? 

**Explanation:**
We are looking for the exact phrase "ss" so we put it in double quotation marks when searching for it.

<details>
    <summary><strong>Answer</strong></summary>
        socket statistics
</details>
---

### 🧩 Task 4: Specialized Search Engines
> **Question:** What is the top country with lighttpd servers?

**Steps Taken:**
- Open Shodan search engine
- Search for lighttpd

**Explanation:**
We are looking for the number of servers, a device connected to the internet, so we will be using Shodan.

<details>
    <summary><strong>Answer</strong></summary>
        United States
</details>

> **Question:** What does BitDefenderFalx detect the file with the hash `2de70ca737c1f4602517c555ddd54165432cf231ffc0e21fb2e23b9dd14e7fb4` as?

**Steps Taken:**
- Open VirusTotal search engine
- Pick the "search" option and enter the file hash

**Explanation:**
As we are dealing with a file hash we will be using VirusTotal this time. 
There are multiple options, but we want to use the Search option as we have a hash and not an actual file

<details>
    <summary><strong>Answer</strong></summary>
        Android.Riskware.Agent.LHH
</details>
---

### 🧩 Task 5: Vulnerabilities and Exploits
> **Question:** What utility does CVE-2024-3094 refer to?

**Steps Taken:**
Check the CVE website for the vulnerability

**Explanation:**
Was provided with a CVE ID so checked the CVE Website which contains information about CVEs

<details>
    <summary><strong>Answer</strong></summary>
        xz
</details>
---

### 🧩 Task 6: Technical Documentation
> **Question:** What does the Linux command cat stand for?

**Steps Taken:**
On a linux terminal run `man cat` or do a quick search for it online.

**Explanation:**
All linux commands have a **manual** page with the full name for the command

<details>
    <summary><strong>Answer</strong></summary>
        concatenate
</details>

> **Question:** What is the netstat parameter in MS Windows that displays the executable associated with each active connection and listening port?

**Steps Taken:**
Check Microsoft Technical Documentation

**Explanation:**
All microsoft terminal commands have official documentation

<details>
    <summary><strong>Answer</strong></summary>
        -b
</details>
---

### 🧩 Task 7: Social Media
> **Question:** You are hired to evaluate the security of a particular company. What is a popular social media website you would use to learn about the technical background of one of their employees?

**Steps Taken:**
Searched for professional social media platforms

**Explanation:**
Common platforms such as snapchat or twitter probably aren't used to talk about professional environments.

<details>
    <summary><strong>Answer</strong></summary>
        LinkedIn
</details>

> **Question:** Continuing with the previous scenario, you are trying to find the answer to the secret question, “Which school did you go to as a child?”. What social media website would you consider checking to find the answer to such secret questions?

**Explanation:**
I know the answer has an option to show education.

<details>
    <summary><strong>Answer</strong></summary>
        Facebook
</details>
---

## 📊 Summary

- Total Flags: 8
- Difficulty: Easy
- Time Taken: 15 Minutes



---

## 🧰 Toolbox

| Tool       | Usage Summary |
|------------|----------------|
| `hydra`    | Password brute-forcing |
| `john`     | Hash cracking |

---
## 🔗 Additional Resources

- [Red Hat](https://www.redhat.com/en/blog/ss-command#:~:text=Formally%2C%20ss%20is%20the%20socket%20statistics%20command%20that%20replaces%20netstat%20.) – A blog from red hat to answer the netstat question
---


## 📝 Personal Reflections

What you learned, what you found challenging, and what you'll try differently next time.
