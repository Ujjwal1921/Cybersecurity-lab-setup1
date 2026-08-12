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



### Learning Outcomes

* Host discovery
* Port scanning
* Service identification
* Basic enumeration
* Understanding network exposure

---

# 📡 3. Packet Analysis with Wireshark

Wireshark is used to capture and analyze network traffic.

The lab demonstrates:

* Packet capture
* TCP/IP analysis
* DNS traffic
* HTTP/HTTPS traffic
* TCP handshake
* Protocol identification

Useful filters:

```text
ip.addr == <LAB-IP>
```

```text
tcp
```

```text
dns
```

```text
http
```

---

# 🌐 4. Web Security Testing with Burp Suite

Burp Suite is used for authorized web application security testing.

The lab covers:

* HTTP requests and responses
* Proxy configuration
* Request interception
* HTTP headers
* Parameters
* Cookies
* Basic web security testing

All testing is performed against intentionally vulnerable or authorized applications.

---

# 💥 5. Metasploit Framework

Metasploit is used to understand vulnerability exploitation in a controlled lab.

The lab focuses on:

* Vulnerability research
* Exploit modules
* Payload concepts
* Sessions
* Post-exploitation concepts
* Security remediation

Example:

```bash
msfconsole
```

---

# 📊 6. Splunk SIEM Setup

Splunk is configured for security monitoring and log analysis.

The environment can include:

```text
Windows Machine
      │
      │ Logs
      ▼
Splunk Universal Forwarder
      │
      ▼
Splunk Enterprise
      │
      ▼
Search / Analysis / Detection
```

### Activities

* Installing Splunk
* Configuring Universal Forwarder
* Collecting logs
* Searching events
* Creating basic dashboards
* Detecting suspicious activity
* Investigating security events

---

# 🖥️ 7. Windows Security Monitoring

Windows logs are collected and analyzed to understand security events.

Important logs include:

* Windows Security Events
* System Events
* Application Events

Example security investigation areas:

* Failed login attempts
* Successful authentication
* Account activity
* Process activity
* Network-related events

---

# 🌐 8. Cisco Packet Tracer

Cisco Packet Tracer is used to understand network architecture and security fundamentals.

The lab covers:

* Routers
* Switches
* PCs
* IP addressing
* Subnetting
* VLAN concepts
* Routing
* Network troubleshooting
* Basic network security

---

# 🧪 Practical Exercises

The repository may contain practical exercises such as:

### Exercise 1 — Network Discovery

Identify active hosts in the authorized lab network.

### Exercise 2 — Port Scanning

Identify open ports and running services.

### Exercise 3 — Packet Capture

Capture and analyze network traffic using Wireshark.

### Exercise 4 — Web Traffic Analysis

Intercept authorized HTTP requests using Burp Suite.

### Exercise 5 — Vulnerability Assessment

Identify potential vulnerabilities in intentionally vulnerable lab systems.

### Exercise 6 — Log Analysis

Collect and analyze Windows security logs using Splunk.

### Exercise 7 — Threat Detection

Create basic searches to identify suspicious authentication activity.

### Exercise 8 — Network Troubleshooting

Analyze connectivity and routing issues using Packet Tracer.

---

# 📁 Repository Structure

```text
Cybersecurity-Setup-Lab/
│
├── README.md
│
├── Architecture/
│   ├── lab-architecture.png
│   └── network-diagram.png
│
├── Kali-Linux/
│   ├── setup.md
│   └── commands.md
│
├── Nmap/
│   ├── scanning.md
│   └── screenshots/
│
├── Wireshark/
│   ├── packet-analysis.md
│   └── screenshots/
│
├── Burp-Suite/
│   ├── setup.md
│   └── screenshots/
│
├── Metasploit/
│   ├── lab-notes.md
│   └── screenshots/
│
├── Splunk/
│   ├── installation.md
│   ├── configuration.md
│   ├── queries.md
│   └── screenshots/
│
├── Windows-Security/
│   ├── event-logs.md
│   └── screenshots/
│
├── Packet-Tracer/
│   ├── topology.pkt
│   └── documentation.md
│
└── Documentation/
    └── lab-report.md
```

---

# 📸 Screenshots

Screenshots can be added to document the setup and results.

Recommended screenshots:

* Kali Linux setup
* Network configuration
* Nmap scan
* Wireshark packet capture
* Burp Suite interface
* Metasploit console
* Splunk dashboard
* Windows Event Viewer
* Cisco Packet Tracer topology

Example:

```markdown
![Nmap Scan](Screenshots/nmap-scan.png)
```

---

# 📚 Skills Demonstrated

This project demonstrates practical knowledge of:

* Cybersecurity Fundamentals
* Network Security
* Linux
* Windows Security
* Network Scanning
* Vulnerability Assessment
* Packet Analysis
* Web Security
* SIEM
* Log Analysis
* Threat Detection
* Incident Investigation
* Network Troubleshooting
* Security Monitoring

---

# 🎓 Learning Outcomes

After completing this lab, I gained practical understanding of:

1. Building a cybersecurity lab environment.
2. Configuring security-focused virtual machines.
3. Performing authorized network reconnaissance.
4. Analyzing network packets.
5. Understanding web application traffic.
6. Working with security testing frameworks.
7. Collecting and analyzing security logs.
8. Understanding basic SIEM operations.
9. Investigating authentication and network events.
10. Applying cybersecurity concepts in a controlled environment.

---

# 🔐 Security & Ethics

This project is created strictly for **educational and authorized security testing**.

All scanning, exploitation, packet capture, and security testing should be performed only against systems that you own or have explicit permission to test.

Never use this lab or its techniques to access unauthorized systems.

---

# 🚀 Future Improvements

Planned improvements include:

* Adding Active Directory lab
* Adding Windows Server
* Integrating Sysmon
* Creating additional Splunk dashboards
* Adding Sigma detection rules
* Adding IDS/IPS monitoring
* Adding Wazuh
* Creating SOC investigation scenarios
* Adding incident-response exercises
* Automating lab deployment
* Adding vulnerability-management workflows

---

# 👨‍💻 Author

**Ujjwal Patidar**

B.Tech Computer Science Student

### Areas of Interest

* Cybersecurity
* Network Security
* SOC Operations
* Vulnerability Assessment
* SIEM & Log Analysis
* Network Engineering

---

## ⭐ Repository

If you find this project useful for learning cybersecurity, consider giving the repository a ⭐.

**Built for learning. Tested in a controlled lab. Secured by knowledge. 🔐**
