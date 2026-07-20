# 🚀 Installing and Running Kali Linux

There are multiple ways to use Kali Linux depending on your requirements. The most common method for beginners is running it inside a virtual machine.

---

# Method 1: Install Kali Linux on VirtualBox (Recommended)

## Step 1: Download Kali Linux

Visit the official Kali Linux website:

👉 https://www.kali.org/get-kali/

Download one of the following:

- VirtualBox Image (Recommended)
- VMware Image
- Installer ISO

---

## Step 2: Install VirtualBox

Download and install Oracle VirtualBox:

👉 https://www.virtualbox.org/wiki/Downloads

---

## Step 3: Import the Kali Linux Virtual Machine

1. Open VirtualBox.
2. Click **Machine → Add** (or **Import Appliance** if applicable).
3. Select the downloaded Kali Linux VM.
4. Allocate RAM (minimum 2 GB, recommended 4 GB or more).
5. Allocate CPU cores (2 or more recommended).
6. Click **Finish**.

---

## Step 4: Start Kali Linux

Select the virtual machine and click **Start**.

Default credentials (older images):

```
Username: kali
Password: kali
```

> **Note:** Newer versions require creating a user during installation.

---

# Method 2: Install Kali Linux Using ISO

### Download the Installer ISO

Download the latest installer from:

https://www.kali.org/get-kali/

---

### Create a Bootable USB

Use tools like:

- Rufus (Windows)
- Balena Etcher
- Ventoy

---

### Boot from USB

1. Restart your computer.
2. Enter the Boot Menu (F12, ESC, or F10 depending on your system).
3. Select the USB drive.
4. Choose **Graphical Install**.
5. Follow the installation wizard.

---

# Method 3: Install Kali Linux on VMware

1. Download VMware Workstation Player.
2. Download the Kali VMware image.
3. Open VMware.
4. Click **Open a Virtual Machine**.
5. Select the downloaded `.vmx` file.
6. Power on the virtual machine.

---

# Method 4: Install Kali Linux on Windows (WSL)

Open PowerShell as Administrator and run:

```powershell
wsl --install
```

Restart your computer.

Install Kali Linux:

```powershell
wsl --install -d kali-linux
```

Launch Kali:

```powershell
kali
```

---

# Update Kali Linux

After installation, update all packages:

```bash
sudo apt update
sudo apt full-upgrade -y
```

Clean unused packages:

```bash
sudo apt autoremove -y
```

---

# Install Additional Tools

Install a package:

```bash
sudo apt install <package-name>
```

Example:

```bash
sudo apt install git
```

---

# Check Kali Version

```bash
cat /etc/os-release
```

or

```bash
lsb_release -a
```

---

# Verify Internet Connection

```bash
ping google.com
```

---

# Shutdown Kali Linux

```bash
sudo poweroff
```

Restart:

```bash
sudo reboot
```

---

# Basic Terminal Commands

Update package list:

```bash
sudo apt update
```

Upgrade packages:

```bash
sudo apt upgrade
```

Current directory:

```bash
pwd
```

List files:

```bash
ls
```

Create a folder:

```bash
mkdir CyberNotes
```

Change directory:

```bash
cd CyberNotes
```

Clear terminal:

```bash
clear
```

---

# Recommended System Requirements

| Component | Recommended |
|-----------|-------------|
| CPU | Dual Core (64-bit) |
| RAM | 4 GB or higher |
| Storage | 40 GB+ |
| Virtualization | Enabled in BIOS |
| Internet | Required for updates |

---

## 📌 Notes

- Download Kali Linux only from the **official website**.
- Always keep your system updated with the latest security patches.
- Use Kali Linux only for **authorized security testing**, learning, and research.
- Virtual machines are recommended for beginners as they are safer and easier to manage.
