---
layout: single
title: "Lab Challenge: Web Applications – Hack The Box Academy"
permalink: /labs/web-applications/
author_profile: true
---

## 🧪 Lab Challenge: Web Applications – Hack The Box Academy

**Problem Statement:**  
Understand and exploit the structural and security elements of modern web applications, including frontend and backend vulnerabilities.

**Approach:**  
- Explored the difference between native applications vs web apps  
- Investigated web infrastructure models and architectural segmentation  
- Broke down front-end technologies (HTML, CSS, JS) and how they're vulnerable  
- Identified security flaws like **HTML Injection**, **XSS**, and **CSRF**  
- Studied backend architecture including servers, databases, and APIs  
- Used real-world CVEs (e.g., [CVE-2014-6271](https://nvd.nist.gov/vuln/detail/cve-2014-6271)) to demonstrate backend vulnerabilities

**Tools Used:**  
- Browser Developer Tools  
- OWASP Cheat Sheet Series  
- Public CVE directories (e.g. NIST)  
- Web-based emulators

**Screenshots:**  
![Module Completion](assets/images/webapp_module_complete.png)

**Key Lessons Learned:**  
- **Web apps are multilayered**: Understanding both frontend and backend components is essential for holistic security.  
- **User input must always be sanitized**: Attacks like HTML injection and XSS are common when inputs are not filtered properly.  
- **Session and token vulnerabilities**: CSRF and XSS can manipulate authenticated sessions if CSRF tokens and validation aren't enforced.  
- **Real-world examples matter**: Understanding CVEs like Shellshock demonstrates how misconfigurations become exploits.

**Platform Link:**  
[HTB Web Applications Module](https://academy.hackthebox.com/achievement/1920307/75)
