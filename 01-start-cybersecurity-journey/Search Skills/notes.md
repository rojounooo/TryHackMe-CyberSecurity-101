# 🏫 TryHackMe Room: Search Skills
> Room URL: <a href="https://tryhackme.com/room/searchskills"> Search Skills </a>

> Category: Reconnaissance

> Difficulty: Easy
---

## 🗂️ Overview

This room covers techniques to use to find relevant information when researching.

---

## 📚 Learning Objectives

- Evaluate information sources
- Use search engines efficiently
- Explore specialized search engines
- Read technical documentation
- Make use of social media
- Check news outlets
---

## 🧾 Section Summaries

### 📦 Task 2: Evaluation of Search Results
**Concepts Covered**:
- Things to consider:
    - Source:
        - Is the author or organization reputable and are they authoritative on the matter, just publishing a blog doesn't make an author reputable
    - Evidence and reasoning:
        - Are the claims logical? Are they backed by evidence? Hard facts are needed, this can include citations or reports.
    - Objectivity and Bias:
        - Is the author biased, do they only provide one perspective or multiple?
    - Corroboration and Consistency:
        - Check multiple sources for similar claims, the first source is not a "be all end all"
---

### ⚙️ Task 3: Search Engines
**Concepts Covered**:
- Search Operators used by Google 
    - "exact phrase": Double quotes to indicate you are looking for pages with that exact phrase, results will only include pages with the phrase in it
    - site: Filters by domain name 
    - "-": The minus symbol removes results with a specific word or phrase
    - filetype: Only returns results with the specified filetype

### ⚙️ Task 4: Specialized Search Engines
**Concepts Covered**:
- **Shodan** - Search Engine for devices and systems connected to the internet like servers and IoT devices
- **Censys** - Search engine for hosts, website and certificates
- **VirusTotal** - Online virus scanning service
- **Have I Been Pwned** - Database to check whether email or password has been in recent leaked data breaches

### ⚙️ Task 5: Vulnerabilities and Exploits
**Concepts Covered**:
- **CVE**:
    - Common Vulnerabilities and Exposures
    - The program is like a dictionary of vulnerabilities
    - Standardized ID for vulnerabilites and issues in software and hardware products
    - Each is assigned a CVE ID with the following format `CVE-YEAR-XXXXX`
    - MITRE maintain the **CVE** program, there is a <a href="https://www.cve.org/">CVE Program </a> website and the <a href="https://nvd.nist.gov/">National Vulnerability Database </a> (**NVD**) website

- Exploit Database (**Exploit DB**)
    - Do not attempt exploitable unless given permission (usually via a legal contract) 
    - Exploit DB contains exploit codes from various authors for different vulnerabilities
    - Some are tested and verified
    - Exploit Database has a <a href="https://www.exploit-db.com/"> website </a> and there is also a terminal tool known as searchsploit

- **GitHub**
    - A web-based platform for software developers
    - Contains many CVE related tools, with proof-of-concept and exploit codes

### ⚙️ Task 6: Technical Documentation
**Concepts Covered**:
- **Linux Manual Pages**  
    - "man" for short  
    - `man {command}` to get the manual pages on Linux; can also search for them in a browser  
    - man pages contain detailed information about the tool, flags, and how to use them  

- **Microsoft Windows**  
    - Microsoft provides official technical documentation for its products  
    - Searching for commands like `ipconfig` on the Microsoft Technical Documentation website returns detailed, official results  
    - Official documentation is the most reliable, up-to-date source for understanding product features and functions  

### ⚙️ Task 7: Social Media 
**Concepts Covered**:
- - **Social Media and Cyber Security**  
    - Billions of users are registered on platforms like Facebook, Twitter, and LinkedIn  
    - Exploring new platforms is encouraged; temporary email addresses can be used for privacy during exploration  
    - Avoid using your primary account to prevent unwanted connections while testing platforms  
    - Social media is a powerful tool to connect with people and companies of interest  
    - It’s crucial to monitor oversharing by individuals, which could expose personal data used in account recovery (e.g., secret questions)  
    - Cyber security professionals can use social media to stay current with trends, tools, and industry news  
    - Following reliable channels, groups, and news outlets helps grow technical expertise and awareness
---


## 🛠️ Tools/Commands Learned

| Tool/Command | Purpose |
|--------------|---------|
| `Shodan`                    | Internet connected devices lookup                |
| `Censys`                    | Internet connected hosts, certificate etc lookup |
| `VirusTotal`                | File check                                       |
| `Have I Been Pwned`         | Check if credentials have been leaked in breach  |
| `CVE website`               | Contains CVE information                         |
| `Exploit DB`/ `Searchsploit`| List of exploit codes                            |
---


