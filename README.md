# Lab-1-Network-Reconnaissance-and-Service-Enumeration-with-Metasploitable-2
Network reconnaissance and service enumeration against Metasploitable 2 using Nmap, NSE scripts, and WhatWeb in an authorized lab environment.

## Overview

This laboratory exercise focused on performing network reconnaissance and service enumeration against the Metasploitable 2 virtual machine using Nmap and WhatWeb from a Kali Linux workstation. The objective was to identify active hosts, discover open ports, determine service versions, detect operating system information, enumerate network services, and fingerprint web technologies.

The exercise was conducted within an authorised and isolated laboratory environment for educational and cybersecurity training purposes.

---

## Lab Environment

| Component | Description |
|------------|------------|
| Assessment Workstation | Kali Linux |
| Target System | Metasploitable 2 |
| Environment | Virtual Lab |
| Initial Target IP | 10.15.203.233 |
| Updated Target IP | 10.15.203.91 |
| Scope | Metasploitable 2 Only |

### Note

The target system initially used the IP address **10.15.203.233** during Steps 1-9. Following a virtual machine restart, the target received a new DHCP-assigned address (**10.15.203.91**), which was used for Steps 10-30.

---

## Objectives

- Verify connectivity between Kali Linux and Metasploitable 2.
- Perform host discovery.
- Discover open TCP and UDP ports.
- Identify running services and service versions.
- Detect the target operating system.
- Enumerate HTTP, SMB, SSH, and FTP services.
- Fingerprint the target web application using WhatWeb.
- Build a comprehensive service inventory.

---

## Tools Used

- Nmap
- WhatWeb
- Curl
- Kali Linux
- Metasploitable 2

---

## Methodology

The assessment followed a structured reconnaissance process:

1. Target identification
2. Connectivity verification
3. Host discovery
4. TCP port scanning
5. Service version detection
6. Operating system detection
7. NSE script enumeration
8. UDP service discovery
9. HTTP service analysis
10. Web application fingerprinting
11. Service inventory creation

---

## Key Findings

### Open Services Discovered

- FTP (vsFTPd 2.3.4)
- SSH
- Telnet
- SMTP
- DNS
- HTTP
- SMB
- NetBIOS
- NFS
- MySQL
- VNC
- IRC
- Apache Tomcat
- Java RMI

### Web Technologies Identified

- Apache 2.2.8
- Ubuntu Linux
- PHP 5.2.4-2ubuntu5.10
- WebDAV Version 2
- Metasploitable2 - Linux

---

## Security Observations

- vsFTPd 2.3.4 is associated with historical security vulnerabilities.
- Telnet is enabled and transmits information in plaintext.
- SMBv1 is enabled and considered insecure.
