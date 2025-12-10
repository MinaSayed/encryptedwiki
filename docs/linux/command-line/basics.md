# Linux Command Line Guide

The Linux command line, also called the **shell**, allows you to interact with your system using text commands. The most common shell is **Bash** (`Bourne Again SHell`), but others like `zsh` and `fish` exist.

## Table of Contents

1. [Basic Commands](#basic-commands)  
2. [File and Directory Management](#file-and-directory-management)  
3. [File Viewing and Editing](#file-viewing-and-editing)  
4. [Permissions and Ownership](#permissions-and-ownership)  
5. [Process Management](#process-management)  
6. [Package Management](#package-management)  
7. [Networking Commands](#networking-commands)  
8. [Redirection and Pipes](#redirection-and-pipes)  
9. [Searching and Filtering](#searching-and-filtering)  
10. [Useful Shortcuts](#useful-shortcuts)  

---

## Basic Commands

| Command | Description | Example |
|---------|-------------|---------|
| `pwd` | Print current working directory | `pwd` → `/home/user` |
| `whoami` | Show current user | `whoami` → `user` |
| `date` | Show current date and time | `date` → `Wed Dec 10 05:00:00 UTC 2025` |
| `echo` | Print text to the terminal | `echo "Hello World"` |

---

## File and Directory Management

| Command | Description | Example |
|---------|-------------|---------|
| `ls` | List files and directories | `ls -l` (detailed listing) |
| `cd` | Change directory | `cd /etc` |
| `mkdir` | Create a directory | `mkdir my_folder` |
| `rmdir` | Remove empty directory | `rmdir my_folder` |
| `rm` | Remove files or directories | `rm file.txt` or `rm -r folder/` |
| `cp` | Copy files or directories | `cp file.txt /tmp/` |
| `mv` | Move or rename files | `mv old.txt new.txt` |

---

## File Viewing and Editing

| Command | Description | Example |
|---------|-------------|---------|
| `cat` | Display file contents | `cat file.txt` |
| `less` | View file contents page by page | `less file.txt` |
| `head` | View first lines | `head -n 10 file.txt` |
| `tail` | View last lines | `tail -n 10 file.txt` |
| `nano` | Simple text editor | `nano file.txt` |
| `vim` | Advanced text editor | `vim file.txt` |

---

## Permissions and Ownership

| Command | Description | Example |
|---------|-------------|---------|
| `chmod` | Change file permissions | `chmod 755 file.sh` |
| `chown` | Change file owner | `chown user:user file.txt` |
| `ls -l` | List files with permissions | `ls -l` → `-rw-r--r-- 1 user user 1024 Dec 10 05:00 file.txt` |

**Permissions Format:**  
`r = read, w = write, x = execute`  
Three sets: `user | group | others`

---

## Process Management

| Command | Description | Example |
|---------|-------------|---------|
| `ps` | List running processes | `ps aux` |
| `top` | Interactive process viewer | `top` |
| `htop` | Better interactive process viewer | `htop` (requires installation) |
| `kill` | Terminate a process | `kill 1234` |
| `killall` | Terminate process by name | `killall firefox` |

---

## Package Management

**Debian/Ubuntu (APT)**

```bash
sudo apt update          # Update repository info
sudo apt upgrade         # Upgrade installed packages
sudo apt install pkg     # Install a package
sudo apt remove pkg      # Remove a package
