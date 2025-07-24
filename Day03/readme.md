#  💡 Day 03: ✨ Static & Dynamic Analysis ✨ and 💻 Linux Commands 💻



## 📑 Table of Contents
- [Static vs. Dynamic Analysis](#static-vs-dynamic-analysis)
- [Useful Linux Commands](#useful-linux-commands)
- [Understanding chmod](#understanding-chmod)
- [Villain Framework](#villain-framework)
- [References](#references)

---

## 🕵️ Static vs. Dynamic Analysis

| Aspect        | Static Analysis                           | Dynamic Analysis                          |
|---------------|------------------------------------------|-------------------------------------------|
| What          | Examines code without executing it        | Examines code while it's running          |
| Tools         | `lint`, `cppcheck`, `bandit`, `sonarqube`| `strace`, `ltrace`, debuggers, sandboxes  |
| Pros          | Early bug detection, fast                | Real-world behavior, runtime checks       |
| Cons          | May miss runtime issues                  | Harder to automate, can be slower         |
| Use Cases     | Code review, CI pipelines                | Malware analysis, fuzz testing            |

> **Tip:** Use both for comprehensive security and quality assurance.

---

## 💻 Useful Linux Commands

| Command       | Example                    | Purpose                             |
| ------------- | -------------------------- | ----------------------------------- |
| `ls`          | `ls`                       | Lists directory contents            |
| `cd`          | `cd /var/log`              | Changes directory                   |
| `pwd`         | `pwd`                      | Shows current directory path        |
| `mkdir`       | `mkdir test_dir`           | Creates a new directory             |
| `rmdir`       | `rmdir test_dir`           | Deletes an empty directory          |
| `touch`       | `touch file.txt`           | Creates a new empty file            |
| `rm`          | `rm file.txt`              | Removes a file                      |
| `cp`          | `cp file.txt /tmp/`        | Copies a file                       |
| `mv`          | `mv file.txt backup.txt`   | Moves or renames a file             |
| `man`         | `man ls`                   | Opens the manual page for a command |
| `echo`        | `echo "Hello World"`       | Prints a message to terminal        |
| `chmod`       | `chmod 755 script.sh`      | Changes file permissions            |
| `chown`       | `chown user:user file.txt` | Changes file ownership              |
| `ps`          | `ps aux`                   | Lists active processes              |
| `kill`        | `kill 1234`                | Terminates process by PID           |
| `top`         | `top`                      | Real-time system monitoring         |
| `df`          | `df -h`                    | Shows disk space usage              |
| `du`          | `du -sh /etc/`             | Shows directory size                |
| `cat`         | `cat file.txt`             | Displays file content               |
| `nano` / `vi` | `nano file.txt`            | Edits a file in terminal            |
| `clear`       | `clear`                    | Clears terminal screen              |
| `exit`        | `exit`                     | Logs out from terminal              |

---

## 🔐 Understanding chmod

File permissions in Linux control who can read, write, or execute a file. The `chmod` command changes these permissions.

### Permission Table

| Symbol | Number | Meaning      |
|--------|--------|--------------|
| r      | 4      | Read         |
| w      | 2      | Write        |
| x      | 1      | Execute      |
| -      | 0      | No permission|

<img width="794" height="397" alt="image" src="https://github.com/user-attachments/assets/3ead3fd6-05bb-4147-ba23-5de7e8a582d6" />

## Villain Framework

Villain is a powerful command-and-control (C2) framework designed for adversary emulation and red team operations.  
It allows attackers to manage multiple reverse shells with advanced features like relay, pivoting, and encrypted communications.
