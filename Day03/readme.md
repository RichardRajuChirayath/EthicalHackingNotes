# 🛡️ Day 03: Static & Dynamic Analysis, Linux Commands, and Villain Framework

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

| Command      | Description                          | Example Usage                       |
|--------------|--------------------------------------|-------------------------------------|
| `ls`         | List directory contents              | `ls -la`                            |
| `cd`         | Change directory                     | `cd /home/user/Documents`           |
| `pwd`        | Print working directory              | `pwd`                               |
| `cp`         | Copy files/directories               | `cp file.txt /tmp/`                 |
| `mv`         | Move/rename files                    | `mv old.txt new.txt`                |
| `rm`         | Remove files/directories             | `rm -rf unwanted_folder`            |
| `cat`        | Concatenate & display file content   | `cat notes.txt`                     |
| `grep`       | Search text using patterns           | `grep "password" file.txt`          |
| `chmod`      | Change file permissions              | `chmod 755 script.sh`               |
| `ps`         | Show running processes               | `ps aux | grep python`              |
| `top`        | Real-time process monitoring         | `top`                               |
| `history`    | Show command history                 | `history | grep ssh`                |

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

### Permission Structure

- Owner
- Group
- Others

### Example

```bash
chmod 755 filename
# 7 = 4+2+1 (rwx) for owner
# 5 = 4+1   (r-x) for group
# 5 = 4+1   (r-x) for others
