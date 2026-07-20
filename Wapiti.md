# 🕷️ Wapiti - Web Application Vulnerability Scanner

## 📖 Overview

**Wapiti** is an open-source web application vulnerability scanner that performs **black-box security testing**. Instead of analyzing the application's source code, it interacts with the target website like a normal user and attempts to identify common security vulnerabilities by sending carefully crafted requests.

Wapiti is commonly used by penetration testers and security professionals to evaluate the security posture of web applications.

---

# ✨ Key Features

Wapiti can identify several common web application vulnerabilities, including:

- SQL Injection (SQLi)
- Cross-Site Scripting (XSS)
- Local File Inclusion (LFI)
- Remote File Inclusion (RFI)
- CRLF Injection
- Command Injection
- Directory Traversal
- Cross-Site Request Forgery (CSRF)
- Server-Side Request Forgery (SSRF)
- Open Redirect

### 📄 Report Formats

After completing a scan, Wapiti can export reports in multiple formats:

- HTML
- XML
- JSON
- TXT

---

# ⚙️ Installation

## Debian / Ubuntu

Update the package repository and install Wapiti.

```bash
sudo apt update
sudo apt install wapiti
```

---

## RHEL / CentOS

Install Python's package manager first, then install Wapiti using pip.

```bash
sudo yum install python3-pip
pip3 install wapiti3
```

---

## Install from GitHub Source

Clone the official repository and install the required dependencies.

```bash
git clone https://github.com/wapiti-scanner/wapiti.git
cd wapiti
pip3 install -r requirements.txt
```

---

# 🚀 Basic Usage

## Perform a Basic Scan

```bash
wapiti -u http://www.example.com
```

### Explanation

- `-u` → Specifies the target website URL.

This command starts a vulnerability scan using Wapiti's default settings.

---

# 📄 Generate a Report

```bash
wapiti -u http://www.example.com -f html -o /path/to/report.html
```

### Explanation

| Option | Description |
|----------|-------------|
| `-f` | Specifies the report format (HTML, JSON, XML, TXT). |
| `-o` | Defines the output location for the generated report. |

---

# 📢 Enable Verbose Output

```bash
wapiti -u http://www.example.com -v 2
```

### Explanation

| Level | Description |
|--------|-------------|
| `0` | Silent mode |
| `1` | Normal output |
| `2` | Detailed (Verbose) output |

Verbose mode provides additional information about each stage of the scan.

---

# 🎯 Attack Modules

Wapiti allows you to control which vulnerability modules are executed during a scan.

## Run Specific Modules

```bash
wapiti -u http://www.example.com --attack sql,xss
```

### Explanation

- `--attack` specifies the vulnerability checks to execute.

In this example, only:

- SQL Injection
- Cross-Site Scripting (XSS)

will be tested.

---

## Skip Specific Modules

```bash
wapiti -u http://www.example.com --skip xss,crlf
```

### Explanation

- `--skip` excludes selected vulnerability modules from the scan.

Here, XSS and CRLF testing are skipped.

---

# 🔐 Authentication Support

Many web applications require authentication before accessing protected pages.

Wapiti supports authenticated scans by submitting login credentials.

## Login Using POST Data

```bash
wapiti -u http://www.example.com --post-login "http://www.example.com/login.php" --data "username=admin&password=admin"
```

### Explanation

| Option | Description |
|----------|-------------|
| `--post-login` | URL of the login page |
| `--data` | Credentials or POST parameters submitted during login |

---

# 📋 Custom HTTP Headers

Custom headers and cookies can be included in scan requests.

```bash
wapiti -u http://www.example.com --header "User-Agent: CustomAgent" --cookie "sessionid=123456"
```

### Explanation

| Option | Description |
|----------|-------------|
| `--header` | Adds a custom HTTP header |
| `--cookie` | Sends session cookies with requests |

---

# 🌐 Proxy Support

Traffic can be routed through an HTTP proxy, which is useful when using tools such as Burp Suite.

```bash
wapiti -u http://www.example.com --proxy http://127.0.0.1:8080
```

### Explanation

- `--proxy` specifies the proxy server address.

---

# ⚡ Advanced Options

## Set Request Timeout

```bash
wapiti -u http://www.example.com --timeout 5
```

### Explanation

- `--timeout` defines the delay between requests (in seconds).

This can help avoid overwhelming the target application.

---

## Restrict Scan Scope

```bash
wapiti -u http://www.example.com --scope url --exclude "http://www.example.com/logout"
```

### Explanation

| Option | Description |
|----------|-------------|
| `--scope` | Restricts scanning to URLs within the target scope |
| `--exclude` | Prevents specified URLs from being scanned |

---

## Limit Crawling Depth

```bash
wapiti -u http://www.example.com --max-depth 3
```

### Explanation

- `--max-depth` limits how many levels of links Wapiti will follow.

Example:

```
Homepage
   │
   ├── Page 1
   │      │
   │      ├── Page 2
   │      │      │
   │      │      └── Page 3
```

With a depth of **3**, Wapiti stops after reaching the third level.

---

# 🧪 Example Scan

The following command demonstrates a complete scan using authentication, custom headers, selected attack modules, and HTML report generation.

```bash
wapiti -u http://www.example.com --post-login "http://www.example.com/login.php" --data "username=admin&password=admin" \
--header "User-Agent: WapitiScanner" --scope page --timeout 3 --attack sql,xss --format html -o /path/to/report.html
```

### What This Command Does

- Logs into the application.
- Sends a custom User-Agent header.
- Restricts the scan to individual pages.
- Adds a delay between requests.
- Executes SQL Injection and XSS modules.
- Generates an HTML report.

---

# 📌 Summary

Wapiti is a lightweight yet powerful web application vulnerability scanner designed for black-box security testing. It supports automated crawling, authentication, multiple vulnerability modules, customizable scanning options, proxy integration, and detailed reporting, making it a valuable tool for authorized web application security assessments.

---

## ⚖️ Disclaimer

This guide is intended for **educational purposes**, **security research**, and **authorized penetration testing** only. Always obtain proper authorization before scanning or testing any web application.
