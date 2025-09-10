# 🏫 TryHackMe Room: Active Directory Basics

> Category: Windows
> Difficulty: Easy
> Room URL: https://tryhackme.com/room/winadbasics

---

## 🗂️ Overview

Active Directory is a simplified method of managing devices and users in a corporate environment

---

## 📚 Learning Objectives

- Understand what Active Directory is
- Understand what an Active Directory Domain is
- Learn components go into an Active Directory Domain
- Understand Forests and Domain Trust

---

## 🧾 Section Summaries

### ⚙️ Task 2: Windows Domain
**Concepts Covered**:
- **AD** is used to manage multiple computers and users in a network without manual configuration of each computer 
- **Windows Domain**:
    - Group of users and computers under the administration of a given business
    - Server running the Active Directory services is known as a **Domain Controller** (**DC**)

- Advantages of a Windows Domain:
    - Centralised Identity Management - All users can be configured with minimum effort
    - Managing security policies - Security policies directly from AD and apply to users and computers across the network

- Real-world Example:
    - School/University networks 
    - When credentials are entered, they are sent to DC and authenticated through AD 
    - Credentials don't need to be stored on each machine


### ⚙️ Task 3: Active Directory
**Concepts Covered**:
- Core of any Windows Domain is the **Active Directory Domain Service** (**AD DS**) 
- Holds the information of all "objects" on the network 
- Objects include:
    - Users 
    - Groups 
    - Machines 
    - Printers 
    - Shares 
    - Etc 

- **Users**:
    - Known as **Security Principals**, can be authenticated by domain and assigned privileges over resources like files and printers
    - Users represent two types of entities: 
        - People:
            - Users will generally represent persons in the organisations like employees 
        - Services: 
            - Users can be defined to be used by services like IIS
            - Every service requires a user but service users are different from regular users 
            - Service users only have privileges needed to run their specific service

- **Machines**:
    - A machine object is created for every computer that joins the AD domain 
    - Also considered **Security Principals** and are assigned accounts 
    - Limited rights within domain 
    - 

### ⚙️ Task 4: Managing Users in AD
**Concepts Covered**:
- Bullet points of key concepts

### ⚙️ Task 5: Managing Computers in AD
**Concepts Covered**:
- Bullet points of key concepts

### ⚙️ Task 6: Group Policies
**Concepts Covered**:
- Bullet points of key concepts

### ⚙️ Task 7: Authentication Methods
**Concepts Covered**:
- Bullet points of key concepts

### ⚙️ Task 8: Trees, Forests and Trusts
**Concepts Covered**:
- Bullet points of key concepts

---

## 🛠️ Tools/Commands Learned

| Tool/Command | Purpose |
|--------------|---------|
| `nmap`       | Network scanning |
| `whois`      | Domain info lookup |

---

## 🔗 Additional Resources

- [Resource Name](URL) – Short description
