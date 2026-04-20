# 🔐 SOC-Style Penetration Testing Report

## 📌 Project Overview
This repository contains a professional SOC-style external penetration testing assessment of a publicly accessible web application hosted on CDN infrastructure.

The assessment focuses on:
- Network exposure analysis
- Web application security posture
- TLS/SSL configuration review
- Information disclosure risks

---

## 🎯 Target
- Domain: houseofwellness.ae  
- Industry: Healthcare Web Application  
- Infrastructure: Wix CDN / Cloud-hosted environment  

---

## 🛠 Tools Used
- Nmap 7.95 (Port & service enumeration)
- Nikto v2.5.0 (Web vulnerability scanning)
- SSLyze (TLS/SSL analysis)
- WhatWeb (Technology fingerprinting)
- DNS tools (dig, nslookup)
- WHOIS lookup

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
- Missing web security headers
- Cookie misconfiguration (Secure / HttpOnly missing)
- Information leakage via CDN headers
- Legacy TLS cipher suites enabled
- Unverified open port observations

---

## 🧠 Conclusion
The target system is secure at baseline level but requires hardening to meet modern enterprise security standards.

No active exploitation vulnerabilities were identified.

---

## 📄 Full Report
See: `/reports/Professional_SOC_Pentest_Report.pdf`

---

## 👤 Author
Abdullah Rashid
