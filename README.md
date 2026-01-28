# Vulnerability Assessment & Penetration Testing (VAPT) – Learning Project

## Overview
This project is designed to build **theoretical and practical knowledge of Vulnerability Assessment and Penetration Testing (VAPT)** using **open-source tools** and **industry-recognized frameworks**.  
The goal is to understand how to assess system security, identify vulnerabilities, prioritize risks, and produce professional security reports **without using paid tools**.

---

## Objectives
- Learn structured security assessment methodologies
- Perform vulnerability scanning and penetration testing
- Understand compliance and security standards
- Apply risk assessment techniques
- Practice documentation and reporting skills
- Produce a comprehensive VAPT report in PDF format

---

## 1. Theoretical Knowledge

### 1.1 Understanding Security Assessment
**Objective:** Evaluate systems using standard frameworks and free tools.

**Key Concepts:**
- Security Assessment: Identifying weaknesses using frameworks like **NIST**
- Types of Security Testing:
  - **Vulnerability Assessment:** OpenVAS (open-source vulnerability scanner)
  - **Penetration Testing:** Kali Linux tools (Nmap, Metasploit)
  - **Compliance Testing:** CIS Benchmarks, security checklists

---

### 1.2 VAPT Methodology
**Objective:** Follow a structured and repeatable approach.

**Phases:**
1. **Planning**
   - Define scope and rules of engagement
   - Tools: Dradis CE
2. **Discovery**
   - Network scanning: Nmap
   - Web application scanning: OWASP ZAP
3. **Attack**
   - Exploitation: Metasploit Framework
4. **Reporting**
   - Use standard pentest report templates

**Learning Reference:**
- OWASP Web Security Testing Guide (WSTG)

---

### 1.3 Security Standards & Compliance
**Objective:** Align assessments with security regulations.

**Standards Covered:**
- GDPR
- HIPAA
- ISO/IEC 27001

**Learning Resource:**
- OWASP Top 10 (Web Application Risks)

---

### 1.4 Risk Assessment Basics
**Objective:** Prioritize vulnerabilities based on risk.

**Techniques:**
- CVSS Scoring (NVD CVSS Calculator)
- Risk Matrix (High / Medium / Low)
- Likelihood vs Impact analysis using Excel or Google Sheets

---

### 1.5 Common Vulnerabilities
**Objective:** Identify real-world security flaws.

**Examples:**
- Network Vulnerabilities:
  - Open ports
  - Misconfigurations (Nmap)
- Web Vulnerabilities:
  - SQL Injection
  - Cross-Site Scripting (XSS)

**Practice Labs:**
- Metasploitable 2 / 3
- OWASP Juice Shop
- VulnHub machines

---

### 1.6 Documentation Fundamentals
**Objective:** Create professional security reports.

**Tools:**
- Dradis CE (collaborative reporting)
- CherryTree (technical notes)
- Spreadsheets for vulnerability tracking
- Screenshots for evidence

**Templates:**
- Free report templates from GitHub

---

## 2. Practical Application

### 2.1 Setup Testing Environment
**Steps:**
1. Install Kali Linux
2. Download Metasploitable 3 from GitHub
3. Configure VirtualBox with Host-Only / NAT networking
4. Verify connectivity between VMs

---

### 2.2 Vulnerability Scanning
**Tools Used:**
- OpenVAS
- Nikto
---

## 2.3 Document Findings

**Objective:** Systematically record and organize discovered vulnerabilities.

### Information to Record
For every identified vulnerability, capture the following details:

| Field | Description |
|------|------------|
| Target IP Address | IP of the vulnerable system |
| Hostname | (If applicable) |
| Open Port | Port number (e.g., 22, 80, 443) |
| Service Name | Running service (e.g., SSH, Apache) |
| Vulnerability Name | Title of the vulnerability |
| Description | Brief explanation of the issue |
| Affected Software | Application/service name |
| Version | Vulnerable software version |
| CVE ID | Associated CVE (if available) |
| CVSS Score | Severity score |
| Risk Level | High / Medium / Low |
| Evidence | Screenshots or scan output |
| Recommended Fix | Patch or configuration change |

---

### Sample Vulnerability Tracking Table

| IP Address | Port | Service | Vulnerability | CVSS | Risk |
|-----------|------|--------|--------------|------|------|
| 192.168.56.101 | 80 | Apache | Outdated Apache Version | 7.5 | High |
| 192.168.56.101 | 21 | FTP | Anonymous Login Enabled | 5.3 | Medium |

---

### Tools Used
- **Excel / Google Sheets** – Vulnerability tracking
- **CherryTree** – Technical notes and evidence
- **Screenshots** – Proof of findings

---

## 2.4 Risk Assessment Practice

**Objective:** Prioritize vulnerabilities based on impact and likelihood.

### Step 1: CVSS Scoring
- Use the **NVD CVSS Calculator**
- Record:
  - Base Score
  - Attack Vector
  - Privileges Required
  - Impact on CIA (Confidentiality, Integrity, Availability)

---

### Step 2: Risk Matrix (3x3)

**Likelihood vs Impact Matrix**

| Impact \ Likelihood | Low | Medium | High |
|---------------------|-----|--------|------|
| **Low** | Low | Low | Medium |
| **Medium** | Low | Medium | High |
| **High** | Medium | High | Critical |

---

### Risk Classification Criteria

- **High Risk**
  - CVSS ≥ 7.0
  - Easily exploitable
  - Direct impact on system availability or data
- **Medium Risk**
  - CVSS 4.0 – 6.9
  - Requires authentication or user interaction
- **Low Risk**
  - CVSS ≤ 3.9
  - Limited impact

---

## 2.5 Reporting

**Final Deliverable:** Comprehensive Vulnerability Assessment & Penetration Testing Report (PDF)

---

### Report Structure

#### 1. Executive Summary
- Purpose of the assessment
- Scope of testing
- Overall security posture
- Key high-risk findings
- Business impact summary

---

#### 2. Assessment Methodology
- VAPT approach followed
- Tools and techniques used
- Testing limitations and assumptions

---

#### 3. Technical Findings
For each vulnerability:
- Vulnerability name
- Description
- Affected system
- CVSS score
- CVE reference
- Evidence (screenshots)
- Exploitation details (if applicable)

---

#### 4. Risk Analysis
- Risk matrix mapping
- Vulnerability prioritization
- Critical vs non-critical issues

---

#### 5. Remediation Recommendations
- Patching instructions
- Configuration hardening steps
- Security best practices
- References to vendor documentation

---

#### 6. Conclusion
- Overall assessment summary
- Security maturity level
- Next steps for improvement

---

### Report Format
- File Type: **PDF**
- Language: Clear, concise, and professional
- Audience: Technical & non-technical stakeholders

---

## Tools & Resources

### Operating System
- Kali Linux

### Scanning & Testing Tools
- OpenVAS
- Nmap
- Metasploit Framework
- OWASP ZAP
- Nikto

### Documentation Tools
- Dradis Community Edition
- CherryTree
- Google Sheets / Excel

### Standards & Frameworks
- OWASP Web Security Testing Guide (WSTG)
- OWASP Top 10
- NIST Security Framework
- CIS Benchmarks

---

## Ethical Disclaimer
All activities performed in this project are conducted in a **controlled lab environment** using **intentionally vulnerable systems**.  
Unauthorized testing on real-world systems is illegal and unethical.

---

## Submission Checklist
- [x] Kali Linux setup
- [x] Vulnerability scans completed
- [x] Findings documented
- [x] Risk assessment performed
- [x] Final PDF report generated

---

## Author
**Name:** Shaun Franklyn 
**Project:** VAPT Learning & Practice  
**Purpose:** Academic / Educational
