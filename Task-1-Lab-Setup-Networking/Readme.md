# Task 1 – The Home Base: Lab Setup & Networking Fundamentals

## 📌 Overview

This project was completed as part of the **SoftNexis Cyber Security Internship Program**.

The objective of this task is to create a secure virtual laboratory environment for practicing cybersecurity concepts and to understand the fundamentals of computer networking. A controlled virtual lab enables safe security testing without affecting real-world systems.

---

# 🎯 Objectives

- Install virtualization software.
- Set up Kali Linux as the attacker machine.
- Set up Metasploitable 2 as the vulnerable target machine.
- Configure both virtual machines on the same private network.
- Verify communication between the virtual machines.
- Learn basic networking commands used in cybersecurity.

---

# 🛠 Tools & Technologies

- Oracle VirtualBox
- Kali Linux
- Metasploitable 2
- Linux Terminal
- TCP/IP Networking

---

# 📂 Lab Environment

| Machine | Purpose |
|----------|---------|
| Kali Linux | Attacker Machine |
| Metasploitable 2 | Vulnerable Target Machine |
| VirtualBox | Virtualization Platform |
| Internal Network | Secure Communication |

---

# ⚙ Installation Steps

## Step 1

Install Oracle VirtualBox.

Official Website:

https://www.virtualbox.org/

---

## Step 2

Download Kali Linux Virtual Machine.

Official Website:

https://www.kali.org/get-kali/

---

## Step 3

Download Metasploitable 2.

Official Website:

https://sourceforge.net/projects/metasploitable/

---

## Step 4

Import both virtual machines into VirtualBox.

---

## Step 5

Configure both VMs to use the same **Internal Network**.

Example:

Network Adapter → Attached To → Internal Network

---

# 🌐 Network Configuration

Example IP Address Assignment

Kali Linux

```
10.0.2.15
```

Metasploitable 2

```
10.0.2.15
```

Both machines were configured on the same virtual network for communication.

---

# 💻 Commands Used

## Display IP Address

```bash
ip addr
```

or

```bash
ifconfig
```

---

## Test Network Connectivity

```bash
ping -c 4 <Target-IP>
```

Example

```bash
ping -c 4 10.0.2.15
```

---

## Display Network Connections

```bash
netstat
```

---

# 📷 Screenshots

Include the following screenshots:

- Kali Linux IP Address
- Metasploitable 2 IP Address
- Successful Ping Response
- Network Configuration

---

# ✅ Expected Results

- Kali Linux installed successfully.
- Metasploitable 2 installed successfully.
- Both virtual machines connected through the same internal network.
- IP addresses successfully identified.
- Successful communication verified using ping.
- Basic networking commands executed successfully.

---

# 📖 Learning Outcomes

Through this task, the following concepts were learned:

- Virtualization
- Virtual Machines
- Network Configuration
- IP Addressing
- Internal Networks
- Linux Networking Commands
- Basic Cybersecurity Lab Setup

---

# 📚 Concepts Covered

- VirtualBox
- Kali Linux
- Metasploitable 2
- TCP/IP
- ICMP
- Ping
- Network Interfaces
- Internal Networking

---

# 🚀 Skills Gained

- Setting up a cybersecurity lab
- Virtual machine management
- Linux terminal usage
- Network troubleshooting
- Understanding IP addressing
- Verifying network communication

---

# 🎯 Conclusion

This task established a secure virtual cybersecurity laboratory using VirtualBox. Both Kali Linux and Metasploitable 2 were configured successfully on the same internal network, allowing secure communication and providing the foundation for future penetration testing and vulnerability assessment tasks.

---

## 👨‍💻 Developed By

Vishwajeet Harijan

---
