# 🛡️ Cybersecurity Fundamentals

## 📖 Introduction

Cybersecurity is the discipline of protecting digital systems, networks, applications, and sensitive information from cyber threats, unauthorized access, and malicious activities. It combines technologies, policies, and best practices to ensure that information remains secure and available to legitimate users.

As organizations become increasingly dependent on digital infrastructure, cybersecurity has become an essential part of protecting personal data, business operations, and national security.

---

# 🎯 Objectives of Cybersecurity

Cybersecurity is built around three fundamental security principles known as the **CIA Triad**.

| Principle | Description | Example |
|-----------|-------------|---------|
| 🔒 Confidentiality | Prevents unauthorized users from accessing sensitive information. | Encrypting online banking transactions using HTTPS. |
| ✔️ Integrity | Ensures data remains accurate, authentic, and unchanged. | Using SHA-256 hashes to verify downloaded software. |
| 🌐 Availability | Guarantees that systems and data are accessible whenever authorized users need them. | Maintaining backup servers and redundant power supplies. |

---

# 🔐 Confidentiality

## What is Confidentiality?

Confidentiality ensures that sensitive information is only accessible to authorized individuals.

### Common Protection Methods

- Data Encryption
- Multi-Factor Authentication (MFA)
- Access Control Lists (ACL)
- User Authentication
- Role-Based Access Control (RBAC)

### Practical Examples

- Encrypting confidential emails using **PGP**.
- Using **HTTPS (SSL/TLS)** to protect website communication.
- Restricting employee access based on job roles.

---

# ✔️ Integrity

## What is Integrity?

Integrity guarantees that information remains accurate and has not been modified without authorization.

### Common Techniques

- Hash Functions
- Digital Signatures
- Checksums
- Data Validation

### Practical Examples

- Verifying downloaded files using **SHA-256** hashes.
- Signing software releases with digital certificates.
- Comparing checksums before and after data transfer.

---

# 🌐 Availability

## What is Availability?

Availability ensures that systems, applications, and information remain accessible whenever required.

### Common Techniques

- Data Backups
- RAID Storage
- Load Balancing
- Disaster Recovery Planning
- High Availability Infrastructure

### Practical Examples

- Using backup servers during hardware failure.
- Replicating databases across multiple locations.
- Implementing redundant network connections.

---

# ⚠️ Common Cyber Threats

Cyber threats are malicious activities designed to compromise confidentiality, integrity, or availability.

---

## 🦠 Malware

Malware is software intentionally created to damage or gain unauthorized access to systems.

### Types of Malware

| Malware | Description | Example |
|----------|-------------|---------|
| Virus | Attaches itself to legitimate files and spreads when executed. | ILOVEYOU Virus |
| Worm | Self-replicates across networks without user interaction. | WannaCry Worm |
| Ransomware | Encrypts files and demands payment for recovery. | CryptoLocker |

---

## 🎣 Phishing

Phishing is a social engineering attack where attackers impersonate trusted organizations to steal sensitive information.

### Common Types

- Email Phishing
- Spear Phishing
- SMS Phishing (Smishing)
- Voice Phishing (Vishing)

### Example

A fake banking email asking users to verify their login credentials.

---

## 🧠 Social Engineering

Social engineering exploits human psychology rather than technical vulnerabilities.

### Popular Techniques

| Technique | Description |
|-----------|-------------|
| Pretexting | Creating a fake identity or scenario to obtain confidential information. |
| Baiting | Offering an attractive reward to trick victims into compromising security. |
| Tailgating | Following an authorized person into a restricted area. |
| Impersonation | Pretending to be someone trustworthy to gain access. |

### Examples

- Fake IT support requesting passwords.
- Infected USB drives left in public places.

---

# 🚨 Security Vulnerabilities

A vulnerability is a weakness that attackers can exploit.

---

## CVE (Common Vulnerabilities and Exposures)

CVE is a globally recognized database of publicly disclosed software vulnerabilities.

### Example

**CVE-2017-0144 (EternalBlue)**

Used by the WannaCry ransomware to exploit Windows systems.

---

## Zero-Day Vulnerabilities

A Zero-Day vulnerability is a newly discovered flaw that has no available security patch.

### Characteristics

- Unknown to software vendors
- No immediate fix available
- Highly valuable to attackers
- Often targeted in advanced attacks

---

# 🏛️ Cybersecurity Frameworks

Security frameworks provide structured guidelines for protecting information systems.

---

## NIST Cybersecurity Framework

The NIST Framework organizes cybersecurity into five core functions.

| Function | Purpose |
|----------|----------|
| Identify | Understand assets, risks, and business environment. |
| Protect | Implement safeguards to reduce risk. |
| Detect | Identify cybersecurity incidents quickly. |
| Respond | Take action to contain and manage incidents. |
| Recover | Restore normal operations after an incident. |

### Example Activities

- Asset Inventory
- Access Control
- Intrusion Detection
- Incident Response
- Backup Restoration

---

## ISO/IEC 27001

ISO/IEC 27001 is an international standard for managing information security.

### Main Objectives

- Risk Assessment
- Security Policies
- Access Management
- Compliance
- Continuous Improvement

### Benefits

- Protects sensitive information
- Improves organizational security
- Supports regulatory compliance
- Enhances customer trust

---

## CIS Controls

The Center for Internet Security (CIS) Controls provide prioritized best practices for defending against cyber attacks.

### Key Controls

- Hardware Asset Inventory
- Software Asset Inventory
- Secure System Configuration
- Continuous Vulnerability Management
- Access Control Management
- Security Monitoring

### Benefits

- Reduces attack surface
- Improves visibility
- Strengthens endpoint security
- Enhances incident detection

---

# 📌 Summary

Cybersecurity is based on protecting the **Confidentiality**, **Integrity**, and **Availability** of information while defending against evolving cyber threats.

### Core Topics Covered

- 🔒 CIA Triad
- 🦠 Malware
- 🎣 Phishing
- 🧠 Social Engineering
- 🚨 Vulnerabilities
- 📚 CVE & Zero-Day
- 🏛️ NIST Framework
- 🌍 ISO/IEC 27001
- 🛡️ CIS Controls

---

## ⚖️ Disclaimer

This repository is intended for **educational purposes**, cybersecurity training, research, and authorized security testing only. Always ensure you have proper permission before performing any security assessment on systems or networks.
