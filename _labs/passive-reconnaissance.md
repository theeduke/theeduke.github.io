---
layout: single
title: "Lab Challenge: Passive Reconnaissance – TryHackMe"
permalink: /labs/passive-reconnaissance/
author_profile: true
read_time: true
---

## 🧪 Lab Challenge: Passive Reconnaissance – TryHackMe

**Problem Statement:**  
The objective was to complete the Passive Reconnaissance module, focusing on gathering publicly available information about a target without direct interaction. This involved using command-line tools (`whois`, `nslookup`, `dig`) and online services (DNSDumpster, Shodan.io) to collect domain, DNS, and server information, and answering specific questions to demonstrate proficiency.

**Approach:**  
- **WHOIS Queries:** Queried domain registration data for `tryhackme.com`, including registrar, registration date, and name servers.  
- **DNS Queries:** Used `nslookup` and `dig` to gather A, MX, and TXT records from public DNS servers (e.g., Cloudflare's `1.1.1.1`).  
- **DNSDumpster:** Mapped DNS structure and discovered subdomains through DNSDumpster’s visual and tabular data.  
- **Shodan.io:** Analyzed global server exposure, identifying commonly exposed services and trends (Apache, nginx) by country and port.  
- **Question Resolution:** Accurately answered module-based questions by validating all outputs across multiple tools and services.

**Tools Used:**

**Command-Line Tools:**  
- `whois`: For WHOIS record details like registrar, registration dates  
- `nslookup`: For querying DNS records (A, TXT, MX)  
- `dig`: For DNS lookups using specific servers (e.g., `dig @1.1.1.1 MX tryhackme.com`)  

**Online Services:**  
- [DNSDumpster](https://dnsdumpster.com): For DNS map visualizations and subdomain discovery  
- [Shodan.io](https://www.shodan.io): For identifying exposed internet-facing services and trends  

**DNS Servers Used:**  
- Cloudflare DNS: `1.1.1.1`  
- Google DNS: `8.8.8.8`  
- Quad9 DNS: `9.9.9.9`  

**Key Lessons Learned:**  
- **Passive Reconnaissance Power:** You can gain a wealth of information without touching the target's infrastructure.  
- **Tool Specificity:** `whois` is best for registrar/domain data; `dig`/`nslookup` are better for DNS records.  
- **Online Tools Enhance Visibility:** DNSDumpster helps with subdomain discovery; Shodan gives global service intelligence.  
- **Query Syntax Matters:** Correct use of tools (`nslookup -type=TXT`, `dig MX`) is essential for precision.  
- **Global Context Matters:** Shodan provided useful insight into service popularity by country and common open ports.  
- **Low Detection Risk:** Passive methods are stealthy and ideal for initial recon phases before active engagement.

