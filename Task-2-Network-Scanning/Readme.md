# Task 2 – Seeing the Unseen: Network Scanning & Enumeration

## 📌 Overview

This project was completed as part of the **SoftNexis Cyber Security Internship Program**.

The objective of this task is to understand network reconnaissance and service enumeration using **Nmap**, one of the most powerful network scanning tools. By scanning a target system, we can discover active hosts, identify open ports, detect running services, and gather valuable information about the target's attack surface.

---

# 🎯 Objectives

- Understand the fundamentals of network scanning.
- Learn how to identify live hosts on a network.
- Discover open TCP ports on a target machine.
- Identify running services and service versions.
- Perform operating system detection.
- Understand the importance of enumeration in penetration testing.

---

# 🛠 Tools & Technologies

- Kali Linux
- Metasploitable 2
- Nmap (Network Mapper)
- VirtualBox
- Linux Terminal

---

# 📂 Lab Environment

| Machine | Purpose |
|----------|---------|
| Kali Linux | Attacker Machine |
| Metasploitable 2 | Vulnerable Target Machine |
| Nmap | Network Scanning Tool |
| VirtualBox | Virtualization Platform |
| Internal Network | Secure Communication |

---

# ⚙ Prerequisites

Before starting this task:

- Oracle VirtualBox installed
- Kali Linux virtual machine configured
- Metasploitable 2 virtual machine configured
- Both virtual machines connected to the same Internal Network
- Network connectivity verified using the `ping` command

---

# 🌐 Target Information

Example Target IP Address

```
10.0.2.15
```

> Replace the IP address above with your actual Metasploitable 2 IP if it is different.

---

# 💻 Commands Used

## 1. Basic Network Scan

```bash
nmap 10.0.2.15
```

Purpose:

- Detect open ports
- Identify running services

---

## 2. Aggressive Scan

```bash
nmap -A 10.0.2.15
```

Purpose:

- Operating System Detection
- Service Version Detection
- Default Script Scanning
- Traceroute

---

## 3. Full Port Scan

```bash
nmap -p- 10.0.2.15
```

Purpose:

- Scan all 65535 TCP ports
- Discover hidden or uncommon services

---

## 4. Service Version Detection

```bash
nmap -sV 10.0.2.15
```

Purpose:

- Detect software versions running on open ports

---

## 5. Operating System Detection

```bash
nmap -O 10.0.2.15
```

Purpose:

- Identify the target operating system

---

# 📊 Sample Scan Results

| Port | State | Service | Version |
|------|-------|----------|---------|
| 21 | Open | FTP | vsftpd 2.3.4 |
| 22 | Open | SSH | OpenSSH 4.7p1 |
| 23 | Open | Telnet | Linux Telnet |
| 25 | Open | SMTP | Postfix SMTP |
| 80 | Open | HTTP | Apache HTTP Server |
| 139 | Open | NetBIOS | Samba |
| 445 | Open | SMB | Samba |
| 3306 | Open | MySQL | MySQL Database |

---

# 🔍 Enumeration Findings

The scan successfully identified several running services on the target machine, including:

- FTP Server
- SSH Server
- Telnet Service
- SMTP Mail Server
- Apache Web Server
- Samba File Sharing Service
- MySQL Database Server

These services represent potential entry points that can be further analyzed during penetration testing.

---

# 📷 Screenshots

Include the following screenshots:

- Basic Nmap Scan (`nmap <IP>`)
- Aggressive Scan (`nmap -A <IP>`)
- Full Port Scan (`nmap -p- <IP>`)
- Enumeration Results
- Open Ports List

---

# ✅ Expected Results

- Target machine discovered successfully.
- Open ports identified.
- Running services detected.
- Service versions identified.
- Operating system information obtained.
- Network enumeration completed successfully.

---

# 📖 Learning Outcomes

Through this task, the following concepts were learned:

- Network Reconnaissance
- Port Scanning
- Service Enumeration
- Operating System Detection
- Attack Surface Identification
- TCP/IP Networking
- Nmap Command Usage

---

# 📚 Concepts Covered

- Nmap
- Enumeration
- TCP Ports
- Network Services
- OS Detection
- Service Version Detection
- Reconnaissance
- Vulnerability Assessment Basics

---

# 🚀 Skills Gained

- Performing network reconnaissance
- Identifying open ports
- Detecting running services
- Using advanced Nmap commands
- Understanding attack surfaces
- Interpreting scan results
- Preparing targets for vulnerability assessment

---

# 🎯 Conclusion

This task introduced the fundamentals of network scanning and enumeration using Nmap. By scanning the Metasploitable 2 virtual machine, various open ports, active services, and operating system details were successfully identified. These findings demonstrate how reconnaissance is a critical first step in penetration testing and cybersecurity assessments, helping security professionals understand the target environment before performing further analysis.

---

## 👨‍💻 Developed By

Vishwajeet Harijan

---
