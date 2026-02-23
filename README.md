## 🔴 Attack Flow

```mermaid
flowchart TD
    A[Kali Linux Attacker] --> B[Reconnaissance]
    B --> C[Enumeration]
    C --> D[Exploitation]
    D --> E[Credential Harvesting]
    E --> F[Privilege Escalation]
    F --> G[Metasploitable Target]
```
## 🔍 Reconnaissance

### 🖥 Host Discovery
![Host Discovery](02-reconnaissance/host_discovery.png)

### 🚪 Port Scanning
![Port Scan 1](02-reconnaissance/port_scan_1.png)
![Port Scan 2](02-reconnaissance/port_scan_2.png)

## 🧠 Enumeration

### 📂 FTP Enumeration
- Banner Grabbing
- Version Identification

![FTP Banner](03-enumeration/ftp_enum/banner_grabbing.png)
![FTP Version](03-enumeration/ftp_enum/version_identification.png)

---
### 🔑 SSH Enumeration
- Service detection
- User validation attempts

![SSH Scan 1](03-enumeration/ssh_enum/Ubuntu-2026-02-21-14-49-34.png)
![SSH Scan 2](03-enumeration/ssh_enum/Ubuntu-2026-02-21-14-56-47.png)
![SSH Scan 3](03-enumeration/ssh_enum/Ubuntu-2026-02-21-14-59-05.png)
![SSH Scan 4](03-enumeration/ssh_enum/Ubuntu-2026-02-21-15-00-48.png)
![SSH Scan 5](03-enumeration/ssh_enum/Ubuntu-2026-02-21-15-12-41.png)

### 🌐 Web Enumeration
- Directory discovery
- Service probing
- Web application mapping

![Web Enum 1](03-enumeration/web_enum/Ubuntu-2026-02-20-19-53-06.png)
![Web Enum 2](03-enumeration/web_enum/Ubuntu-2026-02-20-19-55-41.png)
![Web Enum 3](03-enumeration/web_enum/Ubuntu-2026-02-20-19-56-57.png)
![Web Enum 4](03-enumeration/web_enum/Ubuntu-2026-02-20-19-58-58.png)
![Web Enum 5](03-enumeration/web_enum/Ubuntu-2026-02-20-20-01-22.png)
![Web Enum 6](03-enumeration/web_enum/Ubuntu-2026-02-20-20-02-58.png)
![Web Enum 7](03-enumeration/web_enum/Ubuntu-2026-02-20-20-07-05.png)
# Internal Network Compromise Simulation (Red Team Lab)

## Overview
This project simulates a real-world internal network attack performed in a controlled lab environment using Kali Linux and Metasploitable.

The objective was to demonstrate the full red team lifecycle:
Reconnaissance → Enumeration → Exploitation → Post-Exploitation 

---

## Lab Setup
- Attacker: Kali Linux
- Target: Metasploitable 2
- Environment: Virtual lab
- Network: Internal simulated network

---

## Attack Phases

### 1. Reconnaissance
- Host discovery
- Network scanning
- Port scanning

### 2. Enumeration
- FTP enumeration
- SSH enumeration
- Web service discovery

### 3. Exploitation
- Vulnerability exploitation
- Reverse shell access

### 4. Post Exploitation
- Credential harvesting
- Privilege escalation
- Persistence

---

## Tools Used
- Nmap
- Netcat
- Metasploit
- Hydra
- Wireshark


---

## Skills Demonstrated
- Network reconnaissance
- Service enumeration
- Exploitation techniques
- Credential harvesting
- Privilege escalation
- Red team workflow

---

## Disclaimer
This project was conducted in a controlled lab environment for learning and ethical cybersecurity purposes only.
