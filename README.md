# 🔐 Cybersecurity Setup Lab

A hands-on **Cybersecurity Lab Environment** designed for learning and practicing fundamental cybersecurity concepts, network security, vulnerability assessment, monitoring, and security testing.

This project demonstrates the setup and configuration of a practical cybersecurity environment using tools such as **Kali Linux, Windows, Wireshark, Nmap, Burp Suite, Splunk, Metasploit, and Cisco Packet Tracer**.

---
## 📌 Project Overview

The **Cybersecurity Setup Lab** is a hands-on virtual laboratory environment designed for learning and practicing cybersecurity concepts in a controlled and isolated environment.

This project uses **Oracle VirtualBox** to create the virtual lab environment and **Kali Linux** as the primary cybersecurity platform.


## 🎯 Project Objective

The main objective of this lab is to create a controlled environment where cybersecurity concepts can be practically implemented and tested.

The lab helps in understanding:

* Network security fundamentals
* Vulnerability assessment
* Network scanning and enumeration
* Packet analysis
* Web application security testing
* Log monitoring and analysis
* Threat detection
* Incident investigation
* Security tools and techniques
* Basic SOC operations

> ⚠️ **Disclaimer:** This lab is intended only for educational purposes and authorized security testing. Do not use these techniques against systems, networks, or applications without permission.

---

## 🎯 Purpose of the Lab

The main purpose of this lab is to build a practical cybersecurity environment where different security tools and techniques can be tested safely.

This lab focuses on:

- Network Security
- Vulnerability Assessment
- Network Scanning
- Packet Analysis
- Web Security Testing
- SIEM Monitoring
- Log Analysis
- Threat Detection
- Security Investigation
- Linux and Windows Security

## 🏗️ Lab Architecture

The cybersecurity lab can contain multiple virtual machines and security tools.

### Example Environment

```text
                    ┌─────────────────────┐
                    │      Host PC        │
                    │   Windows / Linux   │
                    └──────────┬──────────┘
                               │
                        Virtual Network
                               │
              ┌────────────────┴────────────────┐
              │                                 │
      ┌───────▼────────┐                ┌───────▼────────┐
      │   Kali Linux   │                │ Windows VM     │
      │                │                │                │
      │ Nmap           │                │ Event Logs     │
      │ Wireshark      │                │ Security Logs  │
      │ Burp Suite     │                │ Test Machine   │
      │ Metasploit     │                │                │
      └───────┬────────┘                └───────┬────────┘
              │                                 │
              └──────────────┬──────────────────┘
                             │
                     ┌───────▼────────┐
                     │     Splunk     │
                     │ SIEM / Logs    │
                     │ Monitoring     │
                     └────────────────┘
```

---
## ⚙️ Lab Configuration

The Cybersecurity Lab is configured using **Oracle VirtualBox** and **Kali Linux** in a controlled virtual environment.

### 💻 Host Machine

| Component | Configuration |
|---|---|
| Host Operating System | Windows |
| Virtualization Platform | Oracle VirtualBox |
| Security Operating System | Kali Linux |
| Network Type | NAT Network |
| Network Address | 10.10.10.0/24 |

### 🖥️ Kali Linux VM

| Component | Configuration |
|---|---|
| Operating System | Kali Linux |
| Network Adapter | NAT Network |
| IP Address | 10.10.10.10 |
| Network | 10.10.10.0/24 |

### 🌐 Network Configuration

The Kali Linux virtual machine is connected to a dedicated NAT Network created in VirtualBox.


### 🛠️ Lab Setup Procedure

## Step 1: Install 7-Zip

7-Zip is installed on the host machine to extract compressed files such as `.7z`, `.zip`, and other archive formats.

### Tool: 7-zip

---

## Step 2: Install VirtualBox

Oracle VirtualBox is installed to create and manage the virtual machines required for the cybersecurity lab.

---

## Step 3: Create the NAT Network

A dedicated NAT Network is created in VirtualBox to provide network connectivity for the cybersecurity lab.
### NAT Network Configuration

## Step 4: Import Kali Linux

The Kali Linux virtual machine is imported into Oracle VirtualBox after extracting the downloaded Kali Linux files.

### Procedure

1. Extract the downloaded Kali Linux archive using **7-Zip**.
2. Open **Oracle VirtualBox**.
3. Click **File → Import Appliance**.
4. Browse to the extracted Kali Linux appliance file.
5. Select the Kali Linux appliance.
6. Review the virtual machine configuration.
7. Select the required storage location.
8. Click **Import**.
9. Wait for the import process to complete.
10. Verify that the Kali Linux virtual machine appears in VirtualBox Manager.
    
![Kali Linux Import](<img width="1714" height="872" alt="Screenshot 2026-08-12 142746" src="https://github.com/user-attachments/assets/2a1ab653-d8e7-4c67-a30a-6fe052959fe3" />
)
### Purpose

Kali Linux is used as the primary cybersecurity platform for performing network analysis, security testing, and other authorized cybersecurity lab activities.

---

## Step 5: Configure the Kali Linux Network

The Kali Linux virtual machine is configured to use the NAT Network created in Step 3.

### Network Configuration

```text
IP Address: 10.10.10.20
Netmask: /24
Gateway: 10.10.10.10
DNS Server: 8.8.8.8
```

![Kali Linux Network Configuration](![Uploading Screenshot 2026-08-12 143039.png…]()
)

## Step 6: Create a Clean VM Snapshot

After completing the Kali Linux installation and network configuration, a clean snapshot of the virtual machine is created.

### Purpose

The main purpose of creating a clean snapshot is to maintain a stable restore point for the cybersecurity lab.

During future lab exercises, different security tools, configurations, and testing activities may modify the virtual machine. If any unwanted changes, configuration errors, or software issues occur, the virtual machine can be restored to this clean snapshot.

---

---
## 📚 What I Learned

Through this Cybersecurity Setup Lab, I learned how to build and configure a basic virtual cybersecurity environment using Oracle VirtualBox and Kali Linux.

### Key Learning Outcomes

- Learned how to install and use **7-Zip** to extract virtual machine files.
- Learned how to install and configure **Oracle VirtualBox**.
- Learned how to create and configure a **NAT Network** in VirtualBox.
- Learned how to import a **Kali Linux virtual machine** into VirtualBox.
- Learned how to configure the **Kali Linux network adapter**.
- Learned how to check IP addresses and network configuration using Linux commands.
- Learned how to verify network connectivity from Kali Linux.
- Learned how to create a **clean VM snapshot**.
- Learned how snapshots can be used to restore a virtual machine to a stable state.
- Gained practical experience in building a **controlled and isolated cybersecurity lab environment**.
- Understood the importance of maintaining a clean and repeatable lab environment before performing security testing.

### Overall Learning

This lab helped me understand the basic process of setting up a virtual cybersecurity environment and prepared the lab for further practical activities such as network scanning, vulnerability assessment, packet analysis, and security testing.

---

# 🔐 Security & Ethics

This project is created strictly for **educational and authorized security testing**.

All scanning, exploitation, packet capture, and security testing should be performed only against systems that you own or have explicit permission to test.

Never use this lab or its techniques to access unauthorized systems.

---
## 🛠️ Tools and Resources

The following tools and resources were used to build and configure the Cybersecurity Setup Lab.

### 💻 Virtualization & System Tools

- **7-Zip** – https://7-zip.org/download.html 
- **Oracle VirtualBox** – https://virtualbox.org/wiki/Downloads 
- **Kali Linux** –  https://kali.org/get-kali 

---

# 👨‍💻 Author

**Ujjwal Patidar**
CyberSecurity B082
LinkedIn: https://www.linkedin.com/in/ujjwal-patidar-752114298

## ⭐ Repository

If you find this project useful for learning cybersecurity, consider giving the repository a ⭐.

**Built for learning. Tested in a controlled lab. Secured by knowledge. 🔐**

### 📌 Project Objective
**Program Name:** Cybersecurity at Networkwalks |**Week:** 01 | **Project:** Cybersecurity & Pentesting Lab Setup |**Repository:** Github
