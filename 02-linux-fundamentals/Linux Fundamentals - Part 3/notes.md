# 🏫 TryHackMe Room: Linux Fundamentals Part 3

> Category: Linux
> Difficulty: Easy
> Room URL: https://tryhackme.com/room/linuxfundamentalspart3

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

---

### ⚙️ Task 4: General/Useful Utilities  
**Concepts Covered**:

- `wget`:
    - Command-line utility to download files via HTTP/HTTPS
    - Works like a browser download
    ```bash
    wget https://example.com
    ```

- `scp`:
    - Securely transfers files over SSH
    - Uses `SOURCE → DESTINATION` format
    - Examples:
    ```bash
    # Local → Remote
    scp file.txt user@remote:/path/

    # Remote → Local
    scp user@remote:/path/file.txt . 
    ```

- Python HTTP Server:
    - Use `python3 -m http.server` to serve files from current directory
    - Can be accessed by other machines via `wget` or `curl`
    - Useful for quick, local file sharing

---

### ⚙️ Task 5: Processes 101  
**Concepts Covered**:

- **Processes**:
    - Every running program is a process
    - Managed by the kernel
    - Identified by a unique **PID** (Process ID)

- **Viewing Processes**:
    - `ps` shows running processes for the current session
    - `top` gives a real-time view of all system processes

- **Managing Processes**:
    - `kill [PID]` ends a process
    - Common signals:
        - `SIGTERM` – Graceful termination
        - `SIGKILL` – Forceful termination
        - `SIGSTOP` – Suspends the process

- **Namespaces**:
    - Used to isolate resources for groups of processes
    - Provides security and separation between processes

- **systemd and PID 0**:
    - PID 0 is the first process at boot (usually `systemd` in Ubuntu)
    - `systemd` starts and manages other processes as children

- **Starting Services on Boot**:
    - Use `systemctl`:
    ```bash
    systemctl start apache2
    systemctl enable apache2
    ```

- **Foreground vs Background Processes**:
    - Foreground: Runs interactively in terminal
    - Background: Appending `&` lets processes run without blocking terminal
    - Suspend with `Ctrl + Z`, resume with `fg`

---

### ⚙️ Task 6: Automation  
**Concepts Covered**:

- **Cron & Crontab**:
    - `cron` is a daemon that runs scheduled tasks
    - `crontab` is a file that defines scheduled jobs using a specific time format

- **Crontab Format**:
    ```
    MIN HOUR DOM MON DOW CMD
    ```
    | Field | Description                          |
    |-------|--------------------------------------|
    | MIN   | Minute (0–59)                        |
    | HOUR  | Hour (0–23)                          |
    | DOM   | Day of Month (1–31)                  |
    | MON   | Month (1–12)                         |
    | DOW   | Day of Week (0–7, 0 and 7 = Sunday)  |
    | CMD   | The command to run                   |

- **Wildcards**:
    - `*` is used as a wildcard for any value in a field

- **Example**:
    - Backup Documents folder every 12 hours:
    ```bash
    0 */12 * * * cp -R /home/cmnatic/Documents /var/backups/
    ```

- **Editing Crontabs**:
    - Use `crontab -e` to edit your user’s scheduled jobs

- **Helpful Resources**:
    - [Crontab Guru](https://crontab.guru/)
    - Crontab generators for easier formatting

---

### ⚙️ Task 7: Package Management  
**Concepts Covered**:

- **APT Repositories**:
    - Developers submit software to "apt" repositories
    - Approved packages become available to users
    - Supports open-source accessibility

- **Managing Repositories**:
    - Use `add-apt-repository` to add new repositories
    - Community and vendor repositories can be added
    - Can also manually add entries to `/etc/apt/sources.list.d/`

- **Adding GPG Keys**:
    - Ensure software authenticity
    - Example for Sublime Text:
    ```bash
    wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
    ```

- **Adding a Repository Manually**:
    1. Create a `.list` file in `/etc/apt/sources.list.d/`:
        ```bash
        sudo nano /etc/apt/sources.list.d/sublime-text.list
        ```
    2. Add repository info inside
    3. Update APT:
        ```bash
        sudo apt update
        ```
    4. Install the package:
        ```bash
        sudo apt install sublime-text
        ```

- **Removing Repositories/Packages**:
    - Remove via:
        ```bash
        sudo add-apt-repository --remove ppa:PPA_Name/ppa
        ```
    - Or manually delete the `.list` file
    - Then run:
        ```bash
        sudo apt remove sublime-text
        ```

---

### ⚙️ Task 8: Logging  
**Concepts Covered**:

- **Log Location**:
    - Most system/service logs are found in `/var/log`

- **Log Rotation**:
    - Logs are automatically rotated to manage space
    - Handled by utilities like `logrotate`

- **Service Logs**:
    - **Apache2**:
        - `access.log` – every request made to the web server
        - `error.log` – logs errors and issues
    - **fail2ban**:
        - Monitors brute force attempts and logs them
    - **UFW**:
        - Logs firewall-related events

- **System Logs**:
    - Capture:
        - OS performance
        - User actions (e.g., login attempts)
        - Kernel messages
    - Useful for monitoring system health, intrusion detection, and troubleshooting

---

## 🧠 Key Takeaways

- Terminal editors like Nano and Vim are essential for direct file editing
- Utilities like `wget`, `scp`, and Python HTTP servers help with file transfers
- Processes can be managed using `ps`, `top`, `kill`, and `systemctl`
- `cron` and `crontab` allow for automated scheduling of commands
- APT manages packages and repos; logs are vital for monitoring systems

---

## 🛠️ Tools/Commands Learned

| Tool/Command               | Purpose                                                  |
|----------------------------|----------------------------------------------------------|
| `nano`                     | Simple terminal-based text editor                        |
| `vim`                      | Advanced, customizable text editor                       |
| `wget`                     | Download files via HTTP/HTTPS                            |
| `scp`                      | Secure file transfer over SSH                            |
| `python3 -m http.server`   | Serve files over HTTP from current directory             |
| `ps`                       | View running processes                                   |
| `top`                      | Real-time process monitor                                |
| `kill`                     | Terminate processes by PID                               |
| `systemctl`                | Manage systemd services                                  |
| `fg`                       | Bring background process to foreground                   |
| `crontab -e`               | Edit the current user’s cron jobs                        |
| `apt`                      | Install, update, or remove software packages             |
| `add-apt-repository`       | Add (or remove) APT repositories                         |
| `apt-key add`              | Add trusted GPG keys for repositories                    |
| `logrotate`                | Manage automatic rotation of system logs                 |
