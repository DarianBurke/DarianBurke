# Hi there 👋 I'm Darian!

Building knowledge and experience through hands-on experimentation

---
## 🛠️ Projects

### 🖥️ [Windows VM Networking Lab](https://github.com/yourusername/windows-vm-network-lab)
## 📘 Overview
This project demonstrates how to set up and test network connectivity between two Windows 11 virtual machines using **Oracle VirtualBox**.  

The goal was to configure both **internet access** (using NAT) and **VM-to-VM communication** (using Host-Only networking), while fixing IP conflicts and firewall issues.

---

## 🎯 Objectives
- Set up two Windows 11 VMs with:
  - **Adapter 1 (NAT):** Internet access  
  - **Adapter 2 (Host-Only):** Private internal network
- Resolve duplicate IP address issues  
- Enable **ICMP (ping)** through Windows Firewall  
- Test communication between both VMs  

---

## 🧰 Tools Used
- Oracle VirtualBox  
- Windows 11  
- Command Prompt  
- Windows Firewall  

---

## ⚙️ Network Setup
| Adapter | Type | Purpose | Example IP Range |
|----------|------|----------|------------------|
| Adapter 1 | NAT | Internet Access | 10.0.2.x |
| Adapter 2 | Host-Only | VM-to-VM Communication | 192.168.56.x |

---

## 🧠 Troubleshooting Steps
1. **Problem:** Both VMs had the same IPv4 address.  
2. **Fix:**  
   - Enabled DHCP in VirtualBox Host-Only Network Manager.  
   - Ran the following commands:
     ```cmd
     netsh int ip reset
     ipconfig /release
     ipconfig /renew
     ```
3. **Enabled Ping:** Turned on `File and Printer Sharing (Echo Request - ICMPv4-In)` in Windows Firewall.

---

---

## 📚 Learning Goals
- Master Windows system administration
- Build homelab projects and share my progress
- Learn PowerShell, bash scripting, and basic automation
- Explore cybersecurity and ethical hacking labs

---

## 🧰 Tools & Tech
![VirtualBox](https://img.shields.io/badge/-VirtualBox-183A61?logo=virtualbox&logoColor=white&style=for-the-badge)
![Windows](https://img.shields.io/badge/-Windows-0078D6?logo=windows&logoColor=white&style=for-the-badge)
![Git](https://img.shields.io/badge/-Git-F05032?logo=git&logoColor=white&style=for-the-badge)
![PowerShell](https://img.shields.io/badge/-PowerShell-5391FE?logo=powershell&logoColor=white&style=for-the-badge)

---

## 📫 Contact Me
- [LinkedIn](https://linkedin.com/in/yourusername)  
- Email: darian_burke.tech@outlook.com

---

*Thanks for visiting! This profile is under active development as I build and share more of my learning journey.*
