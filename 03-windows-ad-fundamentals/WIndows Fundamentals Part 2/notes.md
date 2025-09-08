# 🏫 TryHackMe Room: Windows Fundamentals Part 2

> Category: Windows
> Difficulty: Easy
> Room URL: https://tryhackme.com/room/windowsfundamentalsparttwo

---

## 🗂️ Overview

- Covers Windows utilities such as Resource Monitor and CMD
- Covers how to access the utilities 

---

## 📚 Learning Objectives

- Understand Utilities 
- Be able to navigate to the utilities 
- Understand usage 

---

## 🧾 Section Summaries


### ⚙️ Task 2: System Configuration
**Concepts Covered**:
- **MSConfig** is for advanced troubleshooting 
- Main purpose is to diagnose startup issues 
- Launch via start menu 

- 5 Main Tabs:
    - General 
    - Boot 
    - Services 
    - Startup 
    - Tools

- **General**
    - Select which devices and services are loaded upon boot 
        - Normal
        - Diagnostic
        - Selective
    
- **Boot**
    - Choose boot options for the OS 
        - Safe Boot 
        - No GUI Boot
    
- **Services**
    - Lists all running/stopped services
    - Services are backgrounded applications

- **Startup** 
    - Directs you to Task Manager
    - MSconfig is not used for managing startup services/programs

- **Tools** 
    - Utilities to configure the operating system 
    - Each tool has a brief description
    - To run a tool:
        - Launch via run prompt
        - Launch via command prompt
        - Click Launch button

### ⚙️ Task 3: Change UAC Settings
**Concepts Covered**:
- UAC settings can be changed or turned off (not recommended)
- Slider is used to choose setting and Microsoft provide their stance 
- 4 levels from "Always notify" to "Never notify"

### ⚙️ Task 4: Computer Management
**Concepts Covered**:
- `compmgmt`
- 3 Primary Sections: 
    - System Tools 
    - Storage 
    - Services and Applications

**System Tools** 
    - **Task Scheduler** :
        - Create and manage common tasks that the computer will run automatically 
        - Windows version of cronjobs

        - Tasks can:
            - Run applications or scripts
            - Be configured to run at any point like log on or log off
        
        - Tasks can be created under the Actions tab    

    - **Event Viewer**:
        - Allows us to view events that have occurred on the computer (like failed login)
        - Record of events can be used to understand the user activity
        - Can be used to diagnose problems (blue screens) or to investigate actions executed on the system

        - Three panes:
            - **Left**: 
                - Provides a hierarchical tree listing event log providers 
            
            - **Middle**: 
                - Displays summary of provider specific events 
            
            - **Right**:
                - Actions 
        
        - 5 Event types: 
            - **Error**:
                - Indicates loss of data or functionality 
                - If service fails to load, Error event logged
            
            - **Warning**:
                - Not currently significant but can indicate possible future problem 
                - Low disk space results in Warning event 
            
            - **Information**:
                - Success operation of an application, driver or service 
                - If a driver loads successfully, an Information Event can be logged
            
            - **Success Audit**: 
                - Audited successful security access attempt
                - Successful login attempt 

            - **Failure Audit**: 
                - Failed security access attempt 
                - Failed login
            
        - Standard Logs:
            - **Application**
                - Events logged by applications
            
            - **Security** 
                - Valid and invalid logon attempts 
                - CRUD of files and objects
            
            - **System**
                - Events logged by system components 
            
            - **CustomLog**
                - Events logged by application that create a custom log
    
    - **Shared Folders**:
        - List of shared and folders that others can connect too 
        - Default shares:
            - ADMIN$
            - C$
        
        - **Sessions** 
            - List of users who are currently connected to the shares

    - **Local Users and Groups**:
        - `lusrmgr.msc`
        - View local users and groups 
        - View their permissions

    - **Performance**:
        - Performance Monitor (perfmon)
        - Used to view performance data in real-time or from a log file 
        - Useful for troubleshooting performance issues on a system

    - **Device Manager**:
        - View and configure hardware
        - E.g. Disabling hardware attached to a computer

- **Storage**
    - **Disk Management**
        - Enables advanced storage tasks:
        - Setup a new drive 
        - Extend Partition 
        - Shrink Partition 
        - Assign or change a drive letter
    
    - **Services/Application**
        - View properties of services 
        - Enable/Disable Services 

### ⚙️ Task 5: System Information
**Concepts Covered**:
- 

### ⚙️ Task 6: Resource Monitor
**Concepts Covered**:
- Bullet points of key concepts

### ⚙️ Task 7: Command Prompt
**Concepts Covered**:
- Bullet points of key concepts

### ⚙️ Task 8: Registry Editor
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

