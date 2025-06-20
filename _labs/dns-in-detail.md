---
title: "Lab Challenge: DNS in Detail – TryHackMe"
layout: single
permalink: /labs/dns-in-detail/
author_profile: true
read_time: true
---

## 🧪 Lab Challenge: DNS in Detail – TryHackMe

**Problem Statement:**  
The DNS in Detail module focused on understanding the Domain Name System (DNS), its hierarchy, record types, and request process. The objective was to explore DNS concepts, use the `nslookup` command to query DNS records (A, CNAME, MX, TXT), and answer questions to demonstrate proficiency, retrieving flags and specific values as proof of completion.

**Approach:**  
- **DNS Hierarchy:** Reviewed structure from root to top-level domains (TLDs) and second-level domains. Noted rules such as subdomain character limits and valid characters.  
- **Record Types:** Learned purposes of major DNS records:  
  - `A` (IPv4 mapping),  
  - `AAAA` (IPv6),  
  - `CNAME` (canonical names),  
  - `MX` (mail routing),  
  - `TXT` (custom metadata like verification flags).  
- **DNS Request Flow:** Traced the journey of a DNS query through local cache, recursive DNS servers, root servers, and authoritative name servers. Examined the role of TTL in caching efficiency.  
- **Practical Queries:** Used `nslookup` to query `website.thm`:  
  - Retrieved the `CNAME` for `shop.website.thm`  
  - Queried `TXT` records to extract flags  
  - Identified the `MX` record and priority  
  - Found the `A` record for `www.website.thm` to get its IP  
- **Question Resolution:** Answered theoretical questions on subdomain limits and character constraints, and verified results from DNS queries for record accuracy.

**Tools Used:**  
- **Command-Line Tool:**  
  - `nslookup`: To retrieve `A`, `CNAME`, `MX`, `TXT` records  
- **DNS Servers:**  
  - Queried via local resolver (`127.0.0.53` on Linux)  
  - Aware of public resolvers: Cloudflare (`1.1.1.1`), Google (`8.8.8.8`), Quad9 (`9.9.9.9`)  
- **Environment:**  
  - Linux terminal for running queries and validating output

**Key Lessons Learned:**  
- **DNS Hierarchy Clarity:** Understanding domain structure (root → TLD → SLD) helps in mapping internet resources accurately.  
- **Record Type Versatility:** Each record serves a specialized purpose in routing, hosting, or metadata representation.  
- **Request Flow Efficiency:** DNS uses layered caching to reduce response times; TTL is crucial for managing cache refresh cycles.  
- **Practical Query Skills:** Accurate command syntax (`nslookup --type=MX website.thm`) is vital to extract correct results.  
- **Attention to Detail:** Interpreting fields like MX priority and TXT values requires careful review of raw outputs.  
- **Internet Fundamentals:** DNS is foundational to almost all internet communication, and its enumeration is key in cybersecurity reconnaissance.

