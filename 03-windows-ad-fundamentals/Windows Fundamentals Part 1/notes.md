# 🏫 TryHackMe Room: Windows Fundamentals Part 1

> Category: Windows
> Difficulty: Easy
> Room URL: https://tryhackme.com/room/windowsfundamentalspartone

---

## 🗂️ Overview

- Explanation of Windows 
- User Interface 
---

## 📚 Learning Objectives

- Learn the differences between edition
- Understand the GUI
- Be able to navigate the GUI

---

## 🧾 Section Summaries

---

### ⚙️ Task 2: Windows Editions
**Concepts Covered**:
- What is Windows:
    - Operating System from Microsoft 
    - Dates back to 1985 
    - Most dominant home and corporate OS
    - Targeted by hackers & malware writers

- Versions:
    - XP
        - Long-running, popular 
    - Vista 
        - Overhaul of OS but quickly phased out
    - 7 
        - Popular but vendors had to make sure their software worked with it
    - 8.x 
        - Short Lived
    - 10 
        - Popular edition
    - 11  
        - Current edition

- Flavours:
    - Home 
    - Pro
    - Difference is pro has BitLocker Drive Encryption enabled

### ⚙️ Task 3: The Desktop (GUI)
**Concepts Covered**:
- Windows Desktop:
    - Graphical User Interface (GUI) 
    - Welcome screen when you log in
    - Login Screen required credentials

- Components:

    - Desktop
    - Start Menu
    - Search Box (Cortana)
    - Task View 
    - Taskbar
    - Toolbars 
    - Notification Area
    

    - Desktop:
        - Shortcuts to program, folders, files etc.
        - Organised in folders or scattered randomly
        
        - Context Menu:
            - Look and feel can be changed to suit your liking
            - Right-click opens a context menu  
            - Change icon size 
            - Copy/Paste
            - Create new items

        - Display Settings: 
            - Change screen's resolution and orientation
            - Make configurations to multi-screen setup
        
        - Personalize:
            - Change desktop background image 
            - Change fonts, themes, colour scheme, etc.

    - Start Menu:
        - Originally the word start was visible, replaced with a Windows Logo
        - Provides access to all apps/programs, files, utilities, etc 
        - Clicking logo opens the Start Menu

        - Sections:
            - Shortcuts for account/login sessions
                - Lock screen
                - Sign out
                - Documents 
                - Pictures 
                - Settings 

            Applications:
                - Recently added apps/programs 
                - Followed by installed apps/programs with start menu shortcuts enabled
                - Alphabetical Order

            - Tiles: 
                - Icons for specific apps/programs or utilities
                - Can be added by "Pin to start"

    - Taskbar: 
        - Open apps/programs, files, folders are shown in the taskbar 
        - Hovering provides a thumbnail and tooltip 
        - Tooltips used if multiple instances open at once
        - Unless pinned, closed items will disappear



---

### ⚙️ Task 4: The File System
**Concepts Covered**:
- **NTFS**:
    - New Technology File System
    - Previously **FAT**16/32 (File Allocation Table) and **HPFS** (High Performance File System)
    - FAT partitions used in USBs, MicroSDs, etc.

- Journaling:
    - In case of failure, FS can repair folders/files using log file info
    - Not possible with FAT

- Benefits:
    - Supports files > 4GB
    - Set permissions
    - Compression 
    - Encryption

| **Permission**         | **Meaning for Folders**                                                                                     | **Meaning for Files**                                                             |
|------------------------|-------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
| **Read**               | Permits viewing and listing of files and subfolders                                                         | Permits viewing or accessing of the file's contents                               |
| **Write**              | Permits adding of files and subfolders                                                                       | Permits writing to a file                                                          |
| **Read & Execute**     | Permits viewing and listing of files and subfolders as well as executing of files; inherited by files and folders | Permits viewing and accessing of the file's contents as well as executing of the file |
| **List Folder Contents** | Permits viewing and listing of files and subfolders as well as executing of files; inherited by folders only | N/A                                                                                |
| **Modify**             | Permits reading and writing of files and subfolders; allows deletion of the folder                          | Permits reading and writing of the file; allows deletion of the file              |
| **Full Control**       | Permits reading, writing, changing, and deleting of files and subfolders                                    | Permits reading, writing, changing and deleting of the file                       |


### ⚙️ Task 5: The Windows\System32 Folders
**Concepts Covered**:
- **Windows Folder** 
    - The folder that contains the Windows OS
    - Usually found at `C:\Windows` but any drive will work 
    - Can technically be in different folders too 

- **Environment Variables** 
    -  " Environment variables store information about the operating system environment. This information includes details such as the operating system path, the number of processors used by the operating system, and the location of temporary folders "

- **System32 Folder** 
    - Contains critical OS files 
    - Deletion of files/folders can break OS

### ⚙️ Task 6: User Accounts, Profiles, and Permissions
**Concepts Covered**:
- **Administrator Accounts** 
    - Can make system changes: 
        - Add/Delete Users
        - Modify groups 
        - Modify system settings 
        - Install programs 
    
- **Standard User Accounts**
    - Can only make changes to files/folder they own 
    - Can't make system changes 

**User Folders:
    - Each user profile has the same folders:
        - Desktop
        - Documents 
        - Downloads
        - Music 
        - Pictures

### ⚙️ Task 7: User Account Control
**Concepts Covered**:

### ⚙️ Task 8: Settings and the Control Panel
**Concepts Covered**:

### ⚙️ Task 9: Task Manager
**Concepts Covered**:

--- 
