# 🏫 TryHackMe Room: Linux Fundamentals Part 2

> Category: Linux
> Difficulty: Easy
> Room URL: https://tryhackme.com/room/linuxfundamentalspart2

---

## 🗂️ Overview

- Fundamental skills to control remote machines

---

## 📚 Learning Objectives

- Unlocking the potential of your first few commands by introducing you to using flags and arguments
- Advancing your knowledge of the filesystem to perform some more useful commands such as copying and moving files
- Discovering how access to files and folders is managed and how we can determine our access.
- Running your first few scripts and executables!
---

## 🧾 Section Summaries

---

### ⚙️ Task 2: SSH
**Concepts Covered**:
- Protocol allowing remote access to a machine
- Syntax:
  ```bash
  ssh user@ip:port
  ```

### ⚙️ Task 3: Flags and Switches
**Concepts Covered**:
- Many commands allow arguments
- If no arguments are given, default behavior
- Manual page provides the flags and explanations for each

### ⚙️ Task 4: Filesystem Interaction Continued
**Concepts Covered**:
- `touch` creates file
- `mkdir` creates a folder 
- `cp` copy file or folder
- `mv` move file or folder
- `rm` remove file or folder
- `file` determine file type

### ⚙️ Task 5: Permissions 101
**Concepts Covered**:
- Not all users can access all files/folders
- A user can own a file but a group of users can access it
- `su` used to switch users 
    - Requires target user's username and password


### ⚙️ Task 6: Common Directories
**Concepts Covered**:
- /etc
    - **Etcetera** folder 
    - Stores system files used by the operating system
    - Stores **passwd** and **shadow** files

- /var
    - **Variable** data folder
    - Stored log files and data accessed/written by services or applications running on the system

- /root
    - Home for the **root** system user
    
-/tmp
    - **Temporary** folder
    - Stores data that needs to be accessed once or twice
    - Cleared out on system restart 
    - Any user can access by default so can be used to store scripts

### ⚙️ Task 7: Shell Operators
**Concepts Covered**:
- `&` run commands in the background
- `&&` combine commands
- `>` redirect output from one command to a file 
- `>>` append output of a command to a file

---

## 🧠 Key Takeaways

- Linux is so useful because it barely requires resources
- It's open source so can be freely edited 
- Commands are used in the terminal in place of a GUI

---

## 🛠️ Tools/Commands Learned

| Tool/Command | Purpose |
|--------------|---------|
| `echo`       | Outputs provided text |
| `whoami`      | Outputs current logged in user |
| `ls`      | Listing files and directories |
| `cd`      | Change directories |
| `cat`      | Output file contents |
| `pwd`      | Prints full path for current directory |
| `find`      | Find files based on name or extension |
| `grep`      | Filter based on provided pattern |
| `&`      | Background a command |
| `&&`      | Combine commands, n+1 command only works if n command was successful |
| `>`      | Redirects command output to a file (overwrites any content) |
| `>>`      | Appends command output to a file |
---

