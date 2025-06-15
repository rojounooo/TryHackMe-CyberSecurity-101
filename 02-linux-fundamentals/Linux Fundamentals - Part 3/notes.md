# 🏫 TryHackMe Room: Linux 

> Category: 
> Difficulty: 
> Room URL: https://tryhackme.com/room/

---

## 🗂️ Overview
- Day to Day utilities and applications 

---

## 📚 Learning Objectives
- Automation 
- Logging 
- Package Management


---

## 🧾 Section Summaries

---

### ⚙️ Task 3: Terminal Text Editors  
**Concepts Covered**:

- Storing Text in Files
    - Previously used `echo` and pipe operators (`>` and `>>`) to store text in files
    - Not efficient for working with multi-line files

- Terminal text editors provide better functionality for editing files
- Two editors introduced:
  - **Nano** (beginner-friendly)
  - **VIM** (advanced, powerful)

- Nano:
    - Nano launches in a full-screen terminal view
    - Use arrow keys to move between lines
    - Use `Enter` to start a new line
    - Easy to use and remember 
    - Shortcuts shown at bottom of screen 

- Vim:
    - Advanced text editor with a steeper learning curve
    - Powerful for experienced users
    - **Customizable** – Configure keyboard shortcuts to your preference
    - **Syntax Highlighting** – Helpful for coding
    - **Widely Compatible** – Available on all terminals (unlike nano)
    - **Learning Resources** – Many tutorials, cheatsheets, and guides available
    - TryHackMe offers a dedicated VIM room for learning


### ⚙️ Task 4: General/Useful Utilities
**Concepts Covered**:
- `wget`:
    - A command-line utility to download files via HTTP/HTTPS
    - Works similarly to downloading a file in a browser
    ```bash 
    Basic command: 
    wget https://example.com
    ```

- `scp`
    - Secure Transfer Protocol
    - Securely transfers files between computers over SSH
    - Offers authentication and encryption
    - Works using the `SOURCE` → `DESTINATION` model
    - Can transfer files from local to remote system or vice versa
    ```bash
    Local → Remote 
    scp localfile user@remote:/path/to/destination
    ```
    ```bash 
    Remote → Local 
    scp user@remote:/path/to/file localdestination
    ```

- Python HTTP Server
    - Ubuntu includes Python3 by default
    - Python's `http.server` module can be used to serve files over HTTP
    - Ideal for simple, quick file sharing on a local network
    - Serves files from current directory by default 
    - Directory can be changed using flags 
    - Clients can download files using:
        - `wget`
        - `curl`
    ```bash
    Basic Command 
    python3 -m http.server
    ```

### ⚙️ Task 5: Processes 101
**Concepts Covered**:


### ⚙️ Task : 
**Concepts Covered**:
- Processes:
    - Programs running on your machine
    - Managed by the kernel
    - Each process has a **PID** (Process ID)
    - PIDs increment based on the order the process starts (e.g., 60th process has PID 60)


### ⚙️ Task : 
**Concepts Covered**:

---

## 🧠 Key Takeaways

---

## 🛠️ Tools/Commands Learned

| Tool/Command | Purpose |
|--------------|---------|
| ``       | |

---

