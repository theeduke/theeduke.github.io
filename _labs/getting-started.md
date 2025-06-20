---
layout: single
title: "Lab Challenge: Getting Started – Hack The Box Academy"
permalink: /labs/getting-started/
author_profile: true
---

## 🧪 Lab Challenge: Getting Started – Hack The Box Academy

**Problem Statement:**  
The task was to complete the "Getting Started" module on HackTheBox, focusing on foundational cybersecurity skills. This involved understanding Information Security (InfoSec) principles, performing penetration testing tasks such as establishing shells, enumerating services, exploiting vulnerabilities, escalating privileges, and transferring files, while submitting flags as proof of completion.

**Approach:**  
- **Organization:** Used Jupyter Notebook for structured note-taking, created checklists, templates, and a local vulnerability database to streamline workflows.  
- **VPN Connection:** Connected securely to HTB labs via client-based or SSL VPN, confirming success with “Initialization Sequence Completed.”  
- **Shell Establishment:** Set up reverse, bind, and web shells (Netcat, PHP) via exploitation (e.g., file upload).  
- **Service Enumeration:** Scanned with Nmap (`-sV`, `-sC`, `-p-`), used `smbclient`, `snmpwalk`, and Onesixtyone for deeper insight.  
- **Web Enumeration:** Used Gobuster, WhatWeb, inspected `robots.txt`, source code, and admin portals for creds.  
- **Exploitation:** Applied exploits with Searchsploit and Metasploit (e.g., Apache Tomcat, SimpleCMS), overcoming config issues when needed.  
- **Privilege Escalation:** Ran `LinEnum`, checked `sudo -l`, looked for SSH keys and kernel exploits to gain root.  
- **File Transfers:** Transferred files using `wget`, `curl`, `scp`, Python HTTP server, and Base64; verified integrity with `md5sum`.  
- **Flag Submission:** Retrieved `user.txt` and `root.txt` flags after successfully exploiting and escalating privileges.

**Tools Used:**  
- **Note-Taking:** Jupyter Notebook  
- **VPN:** HTB Client, SSL VPN  
- **Shells:** Netcat (`nc`), PHP scripts, Bash  
- **Terminal Multiplexer:** TMUX  
- **Text Editor:** Vim  
- **Network Scanning:** Nmap (`-sV`, `-sC`, `-p-`)  
- **Enumeration:** `smbclient`, `snmpwalk`, Onesixtyone  
- **Web Tools:** Gobuster, WhatWeb  
- **Exploitation:** Searchsploit, Metasploit Framework  
- **File Transfer:** `wget`, `curl`, `scp`, Base64, Python HTTP server  
- **Privilege Escalation:** LinEnum, `sudo`, SSH keys, kernel CVEs


**Key Lessons Learned:**  
- **Organization Enhances Efficiency:** Structured notes and templates reduce errors and improve workflow.  
- **Shell Versatility:** Each shell (reverse, bind, web) has situational strengths and weaknesses.  
- **Enumeration is Foundational:** Effective recon exposes exploitable misconfigurations.  
- **Exploitation Requires Adaptability:** Switching tools or techniques (e.g., when Metasploit fails) is critical.  
- **Privilege Escalation Strategies:** Combining manual review with automated tools boosts chances of success.  
- **File Transfer Security:** Integrity checks like `md5sum` ensure files aren't corrupted or tampered.  
- **Hands-On Practice:** Completing real-world labs bridges theory with application, strengthening skills and confidence.
