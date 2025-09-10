# 🏫 TryHackMe Room: Windows Fundamentals 3

> Category: Windows
> Difficulty: Easy
> Room URL: https://tryhackme.com/room/windowsfundamentals3xzx

---

## 🗂️ Overview

Built in Microsoft Security Tools such as Windows Updates and BitLocker

---

## 📚 Learning Objectives

- Understand the different tools 

---

## 🧾 Section Summaries

### ⚙️ Task 2: Windows Updates
**Concepts Covered**:
- Provide security updates, feature enhancements and patches for OS and other MS products 
- Typically released on 2nd Tuesday of the month 
- AKA **Patch Tuesday**
- Critical updates are released via Windows Update Service
- Located in settings 
- As of Win 10, updates can only be postponed temporarily

### ⚙️ Task 3: Windows Security
**Concepts Covered**:
- Contains tools to protect device and data

- 4 protection areas:
    - Virus & Threat Protection 
    - Firewall & Network Protection 
    - App and Browser Control 
    - Device Security 

- 3 Status icons:
    - Green
        - Sufficiently protected, no recommended actions 
    - Yellow
        - Safety recommendation 
    - Red 
        - Immediate action needed

### ⚙️ Task 4: Virus & Threat Protection 
**Concepts Covered**:
- 2 Parts:
    - Current Threats 
    - Virus & Threat Protection 

- **Current Threats:** 
    - Scan Options:
        - Quick scan - Checks folders 
        - Full scan - Checks all files and running programs, could take longer than an hour 
        - Custom scan - Choose files/locations 
    
    - Threat history 
        - Last scan - Windows Defender AV automatically scans device 
        - Quarantines threats - Isolated threats, prevented from running. Periodically removed
        - Allowed threats - Identified as threats but user allowed them to run 
    
- **Virus & Threat Protection** 
    - Manage settings
        - Real-time protection - Locates malware, stops it from installing or running 
        - Cloud-delivered protection - Provides increased and faster protection with access to cloud data 
        - Automatic sample submission - Sending sample files to MS helps protect you and others 
        - Controlled folder access - Protect files/folders to prevent unauthorised changes by unfriendly applications 
        - Exclusions - AV won't scan excluded items 
        - Notifications - AV will send notifications for critical information
    
    - Virus & Threat Protection Updates 
        - Check for updates - Manually check for updates 
    
    - Ransomware protection
        - Controlled folder access - Ransomware protection needs this to be enabled 

### ⚙️ Task 5: Firewall and Network Protection
**Concepts Covered**:
- **Firewall** 
    - Controls traffic entering and exiting ports 

- 3 Profiles:
    - Domain - Applied to networks where host system can authenticate to a Domain Controller (DC)
    - Private - User-assigned profile for private/home networks
    - Public - Public profile for public networks such as Wi-Fi hotspots

- Clicking on a profile provides the option to toggle firewall on/off
- Option to block all incoming connections 

### ⚙️ Task 6: App & Browser Control
**Concepts Covered**:
- Microsoft Defender SmartScreen 
- Protects against phishing, malware websites/applications, and downloading of potential malicious files
    - Check apps and files
        - Check for unrecognised apps and files from the web 
    
    - Exploit protection
        - Built into Win 10/11 to protect against attacks

### ⚙️ Task 7: Device security
**Concepts Covered**:
- Core isolation:
    - Memory Integrity: 
        - Prevents attacks from inserting malicious code into high-security processes 

- Security Processor:
    - Provides encryption via trusted platform module (TPM)

- Trusted Platform Module (TPM)
    - Provides hardware-based, security-related functions
    - TPM chip carries out cryptographic operations 
    - Physical security mechanisms make it tamper resistant 

### ⚙️ Task 8: BitLocker
**Concepts Covered**:
- **BitLocker Drive Encryption** 
- Data protection feature 
- Addresses threat of physical data theft or exposure from lost, stolen or inappropriately decommissioned computers 
- E.g. if the hard drive is removed and placed in another system 
- BitLocker offers the best protection on devices with TPM installed 


### ⚙️ Task 9: Volume Shadow Copy Service
**Concepts Covered**:
- **VSS**
- Created consistent shadow copy (snapshot/point-in-time copy) of data to be backed up 
- Volume Shadow Copies are stored on the System Volume Information folder on each drive that has protection enabled
- If VSS is enabled, you can:
    - Create a restore point 
    - Perform system restore
    - Configure restore settings 
    - Delete restore points
- Malware looks for these files and deletes them to prevent backups from ransomware


---
