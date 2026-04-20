# 🔐 SOC-Style Penetration Testing Report

## 📌 Project Overview
This repository contains a professional SOC-style external penetration testing assessment of a publicly accessible web application hosted on CDN infrastructure.

The objective of this assessment was to evaluate the external attack surface, identify misconfigurations, analyze TLS security posture, and detect potential information disclosure risks using industry-standard cybersecurity tools.

---

## 🎯 Target
- Domain: houseofwellness.ae  
- Industry: Healthcare Web Application  
- Infrastructure: Wix CDN / Cloud-hosted environment  
- Assessment Type: External Black-Box Security Testing  

---

## 🛠 Tools Used & Their Role in This Case

### 🔍 Nmap 7.95
Used for:
- Network discovery
- Port scanning
- Service version detection
- Identifying exposed services (HTTP/HTTPS and potential unknown ports)

---

### 🌐 Nikto v2.5.0
Used for:
- Web server vulnerability scanning
- Detection of missing security headers
- Identification of insecure HTTP configurations
- Information disclosure checks

---

### 🔐 SSLyze
Used for:
- TLS/SSL configuration analysis
- Cipher suite evaluation
- Certificate validation
- Detection of legacy encryption (CBC usage, OCSP status, etc.)

---

### 🌍 WhatWeb
Used for:
- Web technology fingerprinting
- Identifying backend stack (Wix / CDN / server framework)
- Server header analysis

---

### 🧠 DNS Tools (dig / nslookup)
Used for:
- DNS resolution analysis
- IP mapping and infrastructure discovery
- CDN and load balancer identification

---

### 📜 WHOIS Lookup
Used for:
- Domain ownership identification
- Registrar information analysis
- Organizational attribution (UAE healthcare entity)

---

## 📊 Risk Summary

| Severity | Count |
|----------|------|
| Critical | 0 |
| High     | 0 |
| Medium   | 4 |
| Low      | 2 |

---

## ⚠ Key Findings
- Missing web security headers (CSP, X-Frame-Options, etc.)
- Cookie misconfiguration (Secure / HttpOnly / SameSite missing)
- Information leakage via CDN / server headers
- Legacy TLS 1.2 cipher suites (CBC mode still enabled)
- Unverified open port observations during reconnaissance phase

---

## 🧠 Conclusion
The target system demonstrates a secure baseline configuration with modern TLS implementation and CDN protection.

However, several medium-severity misconfigurations increase the overall attack surface, primarily through information disclosure and web security header weaknesses.

No active exploitation vulnerabilities were identified.

---

## 📄 Full Report
See: `/reports/Professional_SOC_Pentest_Report.pdf`

---

## 👤 Author
Abdullah Rashid
Cybersecurity Analyst | SOC / Pentesting Research Project
