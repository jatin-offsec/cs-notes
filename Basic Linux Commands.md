# 🐧 Introduction to Linux

## 📖 What is Linux?

Linux is a free and open-source operating system based on the Unix architecture. At its core is the **Linux Kernel**, which manages hardware resources and allows software to communicate with the computer.

Unlike proprietary operating systems, Linux is maintained by a global open-source community, making it highly secure, stable, and customizable. Today, Linux powers everything from personal computers and smartphones to servers, cloud platforms, embedded systems, and supercomputers.

---

# ⭐ Key Features

- Open-source and community-driven
- Highly secure and stable
- Multi-user operating system
- Multitasking support
- Portable across different hardware platforms
- Powerful command-line interface (CLI)
- Large collection of software packages
- Widely used in cloud computing and cybersecurity

---

# 🏗️ Linux Architecture

Linux consists of several layers working together.

```
+-----------------------+
|    User Applications  |
+-----------------------+
|         Shell         |
+-----------------------+
|     Linux Kernel      |
+-----------------------+
|      Hardware         |
+-----------------------+
```

### 1. Kernel

The **Kernel** is the heart of the Linux operating system.

It is responsible for:

- Process management
- Memory management
- Device communication
- File system management
- Hardware interaction

---

### 2. Shell

The **Shell** is the interface between the user and the operating system.

It allows users to execute commands, automate tasks, and manage the system efficiently.

Popular Linux shells include:

- Bash (Bourne Again Shell)
- Zsh (Z Shell)
- Fish Shell

---

### 3. File System

Linux organizes files using a hierarchical directory structure that starts from the **Root Directory (`/`)**.

Every file and folder exists somewhere under this root directory.

---

### 4. Applications

Applications are software programs installed on Linux to perform specific tasks.

Examples include:

- Firefox
- Apache Web Server
- VS Code
- Nano
- Vim

---

# 📦 Popular Linux Distributions

Different Linux distributions package the Linux kernel with additional software and package managers.

| Distribution | Description | Best For |
|--------------|-------------|-----------|
| 🟠 Ubuntu | Beginner-friendly Linux distribution with strong community support. | Desktop & Server |
| 🔴 Debian | Stable and reliable distribution with extensive package repositories. | Servers |
| 🔵 CentOS | Enterprise-focused Linux distribution derived from Red Hat. | Enterprise Infrastructure |
| 🐉 Kali Linux | Security-focused distribution designed for penetration testing and digital forensics. | Cybersecurity |
| 🎩 Fedora | Modern Linux distribution featuring the latest technologies. | Developers |
| 🟢 Arch Linux | Lightweight, customizable distribution for advanced users. | Power Users |

---

# 📂 Linux File System Structure

Linux uses a standardized directory hierarchy.

| Directory | Purpose |
|-----------|---------|
| `/` | Root directory of the file system |
| `/home` | Stores personal user files |
| `/root` | Home directory of the root user |
| `/etc` | System configuration files |
| `/usr` | Installed applications and utilities |
| `/var` | Variable files such as logs and databases |
| `/tmp` | Temporary files |
| `/bin` | Essential command-line programs |
| `/sbin` | System administration utilities |
| `/dev` | Device files |
| `/proc` | Process and kernel information |
| `/opt` | Optional third-party software |

---

# 💡 Why Learn Linux?

Linux is the preferred operating system for many technology fields because of its flexibility and reliability.

It is widely used in:

- Cybersecurity
- Ethical Hacking
- Penetration Testing
- Cloud Computing
- Web Hosting
- DevOps
- System Administration
- Embedded Systems
- Artificial Intelligence
- Supercomputing

---

# 🔐 Linux in Cybersecurity

Linux is the foundation of many cybersecurity tools and distributions, making it an essential skill for security professionals.

Popular security distributions include:

- Kali Linux
- Parrot Security OS
- BlackArch Linux

Common cybersecurity activities performed on Linux:

- Network Scanning
- Vulnerability Assessment
- Digital Forensics
- Malware Analysis
- Wireless Security Testing
- Reverse Engineering
- Incident Response

---

# 📌 Summary

Linux is a secure, open-source, Unix-like operating system used across desktops, servers, cloud platforms, and embedded devices. Its flexibility, stability, and extensive software ecosystem make it one of the most popular operating systems in the world. For cybersecurity professionals, Linux provides the foundation for penetration testing, digital forensics, and security research.

# 🐧 Linux Command Cheat Sheet

A comprehensive collection of commonly used Linux commands for file management, user administration, networking, package management, process control, and system monitoring.

---

# 📂 File & Directory Commands

| Command | Description | Example |
|----------|-------------|---------|
| `pwd` | Display the current working directory. | `pwd` |
| `ls` | List files and directories. | `ls -la` |
| `cd` | Change the current directory. | `cd /home/user` |
| `mkdir` | Create a new directory. | `mkdir projects` |
| `rmdir` | Remove an empty directory. | `rmdir temp` |
| `touch` | Create a new empty file. | `touch notes.txt` |
| `cp` | Copy files or directories. | `cp file.txt backup/` |
| `mv` | Move or rename files. | `mv file.txt newfile.txt` |
| `rm` | Remove files or directories. | `rm file.txt` |
| `rm -r` | Remove directories recursively. | `rm -r folder` |
| `tree` | Display directory structure. | `tree` |

---

# 📄 File Viewing Commands

| Command | Description | Example |
|----------|-------------|---------|
| `cat` | Display file contents. | `cat file.txt` |
| `less` | View large files page by page. | `less file.txt` |
| `more` | Display file content one page at a time. | `more file.txt` |
| `head` | Show the first lines of a file. | `head -10 file.txt` |
| `tail` | Show the last lines of a file. | `tail -20 file.txt` |
| `tail -f` | Monitor a log file in real time. | `tail -f /var/log/syslog` |

---

# 🔍 Search Commands

| Command | Description | Example |
|----------|-------------|---------|
| `find` | Search for files and directories. | `find /home -name "*.txt"` |
| `locate` | Quickly locate files. | `locate nginx.conf` |
| `which` | Show the location of a command. | `which python3` |
| `whereis` | Locate binaries and manuals. | `whereis ssh` |
| `grep` | Search text inside files. | `grep "root" file.txt` |

---

# 📦 File Compression

| Command | Description | Example |
|----------|-------------|---------|
| `tar` | Archive files. | `tar -cvf backup.tar folder/` |
| `tar -xvf` | Extract archive. | `tar -xvf backup.tar` |
| `gzip` | Compress a file. | `gzip file.txt` |
| `gunzip` | Decompress a file. | `gunzip file.txt.gz` |
| `zip` | Create ZIP archive. | `zip files.zip file1 file2` |
| `unzip` | Extract ZIP archive. | `unzip files.zip` |

---

# 👤 User Management

| Command | Description | Example |
|----------|-------------|---------|
| `whoami` | Show current user. | `whoami` |
| `id` | Display user information. | `id` |
| `useradd` | Create a user. | `sudo useradd student` |
| `passwd` | Set user password. | `sudo passwd student` |
| `usermod` | Modify user account. | `sudo usermod -aG sudo student` |
| `userdel` | Delete a user. | `sudo userdel student` |
| `groupadd` | Create a group. | `sudo groupadd developers` |
| `groups` | Display user groups. | `groups` |

---

# 🔐 File Permissions

| Command | Description | Example |
|----------|-------------|---------|
| `chmod` | Change file permissions. | `chmod 755 script.sh` |
| `chown` | Change file ownership. | `sudo chown user:user file.txt` |
| `chgrp` | Change file group. | `sudo chgrp developers file.txt` |
| `umask` | Display default permissions. | `umask` |

---

# ⚙️ Process Management

| Command | Description | Example |
|----------|-------------|---------|
| `ps` | Show running processes. | `ps aux` |
| `top` | Real-time process monitor. | `top` |
| `htop` | Interactive process viewer. | `htop` |
| `kill` | Stop a process. | `kill 1234` |
| `kill -9` | Force stop a process. | `kill -9 1234` |
| `pkill` | Kill process by name. | `pkill firefox` |
| `jobs` | List background jobs. | `jobs` |
| `bg` | Resume job in background. | `bg` |
| `fg` | Bring job to foreground. | `fg` |

---

# 🌐 Networking Commands

| Command | Description | Example |
|----------|-------------|---------|
| `ip addr` | Show IP addresses. | `ip addr show` |
| `ifconfig` | Display network interfaces (legacy). | `ifconfig` |
| `ping` | Test connectivity. | `ping google.com` |
| `netstat` | Show network connections. | `netstat -tuln` |
| `ss` | Display sockets. | `ss -tuln` |
| `traceroute` | Trace packet route. | `traceroute google.com` |
| `nslookup` | Query DNS records. | `nslookup google.com` |
| `dig` | DNS lookup tool. | `dig google.com` |
| `curl` | Transfer data via URL. | `curl https://example.com` |
| `wget` | Download files. | `wget https://example.com/file.zip` |

---

# 💾 Disk Management

| Command | Description | Example |
|----------|-------------|---------|
| `df -h` | Display disk usage. | `df -h` |
| `du -sh` | Show folder size. | `du -sh Downloads` |
| `lsblk` | List storage devices. | `lsblk` |
| `fdisk -l` | Display disk partitions. | `sudo fdisk -l` |
| `mount` | Mount filesystem. | `mount /dev/sdb1 /mnt` |
| `umount` | Unmount filesystem. | `umount /mnt` |

---

# 📦 Package Management (Debian/Ubuntu/Kali)

| Command | Description | Example |
|----------|-------------|---------|
| `sudo apt update` | Update package index. | `sudo apt update` |
| `sudo apt upgrade` | Upgrade installed packages. | `sudo apt upgrade` |
| `sudo apt install` | Install software. | `sudo apt install git` |
| `sudo apt remove` | Remove package. | `sudo apt remove nginx` |
| `sudo apt autoremove` | Remove unused packages. | `sudo apt autoremove` |
| `sudo apt search` | Search packages. | `sudo apt search python` |

---

# 📊 System Information

| Command | Description | Example |
|----------|-------------|---------|
| `uname -a` | Kernel information. | `uname -a` |
| `hostname` | Display hostname. | `hostname` |
| `hostnamectl` | Show system information. | `hostnamectl` |
| `uptime` | Show uptime. | `uptime` |
| `free -h` | Display RAM usage. | `free -h` |
| `lscpu` | CPU information. | `lscpu` |
| `lsusb` | USB devices. | `lsusb` |
| `lspci` | PCI devices. | `lspci` |

---

# 🔥 Firewall Commands

| Command | Description | Example |
|----------|-------------|---------|
| `sudo ufw enable` | Enable firewall. | `sudo ufw enable` |
| `sudo ufw disable` | Disable firewall. | `sudo ufw disable` |
| `sudo ufw status` | Check firewall status. | `sudo ufw status` |
| `sudo ufw allow 22` | Allow SSH port. | `sudo ufw allow 22` |

---

# 📜 Service Management

| Command | Description | Example |
|----------|-------------|---------|
| `systemctl status` | Check service status. | `systemctl status ssh` |
| `systemctl start` | Start a service. | `sudo systemctl start apache2` |
| `systemctl stop` | Stop a service. | `sudo systemctl stop apache2` |
| `systemctl restart` | Restart a service. | `sudo systemctl restart apache2` |
| `systemctl enable` | Enable service at boot. | `sudo systemctl enable ssh` |

---

# ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|-----------|--------|
| `Ctrl + C` | Stop running command |
| `Ctrl + Z` | Suspend current process |
| `Ctrl + D` | Logout/Exit terminal |
| `Ctrl + L` | Clear terminal |
| `Ctrl + R` | Search command history |
| `Tab` | Auto-complete command |
| `↑` / `↓` | Browse command history |

---

# 📌 Tips

- Use `man <command>` to open the manual page.
- Use `--help` to view command options.
- Prefix commands with `sudo` when administrative privileges are required.
- Keep your system updated using `sudo apt update && sudo apt upgrade`.

---

⭐ **This cheat sheet is intended for Linux beginners, system administrators, DevOps engineers, and cybersecurity professionals.**
