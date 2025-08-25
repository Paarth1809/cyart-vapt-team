# Week 2 – VAPT Training & Practical Application

This repository documents the **Week 2 tasks** of our Vulnerability Assessment and Penetration Testing (VAPT) training.  
It contains both **theoretical knowledge** and **hands-on practical labs**.

---

## 📘 Theoretical Knowledge

### 1. Vulnerability Scanning Techniques
**What to Learn:**
- **Scan Types:** Network (e.g., Nmap port scans), Application (e.g., Nikto), Authenticated vs. Unauthenticated.
- **Vulnerability Scoring:** Use CVSS v4.0 (e.g., CVSS 8.8 = High). Example: Apache Struts CVE-2017-5638 = Critical.
- **False Positives:** Validate results manually (e.g., confirm open ports).
- **Key Objective:** Configure and validate scans for accurate risk assessment.

**How to Learn:**
- Study OWASP Testing Guide for web scanning.  
- Review NIST SP 800-115 for scanning methods.  
- Analyze WannaCry CVSS mapping.  

---

### 2. Penetration Testing Techniques
**Core Concepts:**
- **Phases:** Reconnaissance, Scanning, Exploitation, Post-Exploitation, Reporting.  
- **Methodologies:** PTES, OWASP WSTG. Example: PTES for scoping web tests.  
- **Ethics:** Always test with authorization and within scope.

**How to Learn:**
- Explore PTES for detailed methodology.  
- Study OWASP WSTG for web pentesting.  
- Review SANS pentest case studies.  

---

### 3. Exploit Development Basics
**Core Concepts:**
- **Exploit Types:** Buffer Overflows, SQL Injection, XSS.  
- **Exploit Writing:** Create basic exploits (e.g., Python buffer overflow).  
- **Mitigations:** Understand ASLR, WAFs, patching.  
- **Objective:** Safely develop and test exploits.

**How to Learn:**
- Study Exploit-DB PoCs.  
- Use TCM Security exploit guides.  
- Try buffer overflow labs on TryHackMe.  

---

## 🛠 Practical Application

### 1. Vulnerability Scanning Lab
**Tools:** Nmap, OpenVAS, Nikto  

**Steps:**
1. Scanned Metasploitable2 VM with Nmap:
   ```bash
   nmap -sV 192.168.1.100
