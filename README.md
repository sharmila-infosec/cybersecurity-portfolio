# 👋 Cybersecurity Portfolio

**Name:** Sharmila Pathakamudi
**Course:** Google Cybersecurity Certificate
**GitHub:** sharmila-infosec
**Email:** sharmila.careers.2213@gmail.com

---

## 🙋 About Me

I am an aspiring Cybersecurity and SOC Analyst with a Master of Science in Information Technology Management from Campbellsville University. I have completed the Google Cybersecurity Professional Certificate (9 courses) and a Security Operations Center (SOC) Bootcamp by ThinkCloudly. This portfolio showcases hands-on projects covering threat detection, incident response, risk management, network security, access control, and Python scripting.

---

## 📂 Portfolio Structure

| Folder | Domain | Projects |
|--------|--------|----------|
| [security-audits](#-security-audits) | Security Auditing | Botium Toys Audit, Security Risk Assessment |
| [incident-reports](#-incident-reports) | Incident Response | DNS/ICMP, Brute Force, SYN Flood, ICMP Flood |
| [incident-response](#-incident-response) | SOC / Triage | Alert Ticket, USB Baiting Exercise |
| [threat-intelligence](#-threat-intelligence) | Threat Intelligence | Pyramid of Pain |
| [risk-management](#-risk-management) | Risk Management | Risk Register, PASTA Worksheet |
| [access-control](#-access-control) | Access Control | Access Control Worksheet, Data Leak Worksheet |
| [network-security](#-network-security) | Network Security | Wireshark vs tcpdump Diagram |
| [python-scripting](#-python-scripting) | Python Automation | Algorithm for File Updates in Python |
| [apply-filters-to-sql-queries](#-sql--linux) | SQL | Apply Filters to SQL Queries |
| [file-permissions-in-linux](#-sql--linux) | Linux | File Permissions in Linux |
| [home-asset-inventory](#-asset-management) | Asset Management | Home Asset Inventory |
| [incident-handler-journal](#-incident-handler-journal) | SOC Documentation | Incident Handler's Journal |
| [security-governance](#-security-governance) | Security Governance | Security Organization Worksheet |

---

## 🔍 Security Audits

Internal security audits using industry frameworks like NIST CSF, PCI DSS, and GDPR to identify risks and recommend controls.

| Project | Description | Skills |
|---------|-------------|--------|
| [Botium Toys Internal Security Audit](security-audits/botium-toys-audit/botium-toys-audit.md) | Conducted a full internal IT audit for a fictitious toy company, assessing controls and compliance gaps across PCI DSS, GDPR, and SOC standards | Risk Assessment, NIST CSF, PCI DSS, GDPR, SOC |
| [Security Risk Assessment Report](security-audits/security-risk-assessment/security-risk-assessment-report.md) | Recommended hardening methods including MFA, password policies, and firewall configurations to reduce organizational security risk | Risk Assessment, Network Hardening, Access Control |

---

## 🚨 Incident Reports

Network-level incident investigations using packet analysis, log review, and the NIST Cybersecurity Framework.

| Project | Description | Skills |
|---------|-------------|--------|
| [Network Traffic Analysis — DNS/ICMP](incident-reports/network-traffic-analysis/network-traffic-analysis.md) | Analyzed tcpdump logs to identify a DNS/UDP port 53 failure causing a website outage | tcpdump, DNS, ICMP, TCP/IP |
| [Website Compromise — Brute Force Attack](incident-reports/website-compromise-brute-force/security-incident-report.md) | Investigated a brute-force attack that led to malware distribution via a malicious redirect | Incident Response, Malware Analysis, DNS/HTTP |
| [SYN Flood DoS Attack](incident-reports/syn-flood-dos-attack/cybersecurity-incident-report-2.md) | Identified a TCP SYN flood DoS attack causing website downtime; analyzed the TCP handshake and recommended mitigations | TCP/IP, DoS Identification, Network Log Analysis |
| [DoS ICMP Flood Attack](incident-reports/dos-icmp-flood-attack/incident-report-analysis.md) | Applied the NIST CSF (Identify, Protect, Detect, Respond, Recover) to analyze an ICMP flood DoS attack | NIST CSF, Firewall Configuration, Incident Response |

---

## 🛡️ Incident Response

SOC-level triage and response activities including alert handling and physical security threat analysis.

| Project | Description | Skills |
|---------|-------------|--------|
| [Alert Ticket — Phishing with Malicious Attachment](incident-response/Alert_ticket_.pdf) | Triaged a medium-severity phishing alert where an employee received a malicious .exe attachment; verified file hash using VirusTotal and escalated to Tier 2 | Alert Triage, VirusTotal, IOC Analysis, Phishing Detection |
| [Parking Lot USB Exercise](incident-response/Parking_lot_USB_exercise_.pdf) | Analyzed a USB baiting scenario, identifying PII risks, attacker mindset, and organizational controls to prevent removable media attacks | Threat Analysis, Social Engineering, Risk Mitigation |

---

## 🔎 Threat Intelligence

Mapping threat indicators to adversary behavior using the Pyramid of Pain framework.

| Project | Description | Skills |
|---------|-------------|--------|
| [Pyramid of Pain](threat-intelligence/Pyramid_of_Pain_.pdf) | Analyzed a ransomware sample flagged by 53/70 VirusTotal vendors; mapped indicators (hash, IP, domain, TTPs) to the Pyramid of Pain framework | VirusTotal, IOC Analysis, MITRE ATT&CK, Threat Intelligence |

---

## ⚠️ Risk Management

Identifying, assessing, and prioritizing security risks using structured frameworks and threat modeling.

| Project | Description | Skills |
|---------|-------------|--------|
| [Risk Register](risk-management/Risk_register_.pdf) | Built a risk register for a coastal bank, scoring assets by likelihood and severity to prioritize security risks including BEC, data leaks, and theft | Risk Assessment, Risk Scoring, Asset Management |
| [PASTA Threat Model Worksheet](risk-management/PASTA_worksheet.pdf) | Applied the PASTA (Process for Attack Simulation and Threat Analysis) framework to a sneaker marketplace mobile app, identifying SQL injection and credential theft threats | Threat Modeling, PASTA, SQL Injection, MFA, Least Privilege |

---

## 🔐 Access Control

Applying access control principles and NIST guidelines to investigate unauthorized access and data leaks.

| Project | Description | Skills |
|---------|-------------|--------|
| [Access Control Worksheet](access-control/Access_control_worksheet_.pdf) | Investigated an unauthorized payroll system access by a former contractor whose account remained active 4 years post-contract; recommended MFA and account expiration policies | Access Control, Authentication, MFA, Least Privilege |
| [Data Leak Worksheet](access-control/Activity_Template__Data_leak_worksheet_.pdf) | Analyzed a data leak caused by improper folder sharing; mapped controls to NIST SP 800-53 AC-6 (Least Privilege) and recommended automated access revocation | NIST SP 800-53, Least Privilege, Data Protection, NIST CSF |

---

## 🌐 Network Security

Comparing network analysis tools and visualizing how they support SOC operations.

| Project | Description | Skills |
|---------|-------------|--------|
| [Wireshark vs tcpdump Diagram](network-security/Diagram_template_.pdf) | Created a comparison diagram of Wireshark and tcpdump, highlighting their similarities and differences for packet capture and network troubleshooting | Wireshark, tcpdump, Network Analysis, Packet Capture |

---

## 🐍 Python Scripting

Automating security administration tasks using Python.

| Project | Description | Skills |
|---------|-------------|--------|
| [Algorithm for File Updates in Python](python-scripting/Algorithm_for_file_updates_in_Python_.pdf) | Wrote a Python algorithm to automatically update an IP address allow list by reading a file, removing unauthorized IPs, and writing the updated list back to disk | Python, File I/O, Automation, Security Administration |

---

## 🗄️ SQL & Linux

Hands-on work with SQL queries and Linux file permissions for security operations.

| Project | Description | Skills |
|---------|-------------|--------|
| [Apply Filters to SQL Queries](apply-filters-to-sql-queries/README.md) | Used SQL with AND, OR, NOT, and LIKE operators to filter login attempts and employee data for security investigations | SQL, Log Analysis, Security Investigations |
| [File Permissions in Linux](file-permissions-in-linux/README.md) | Managed file and directory permissions in Linux using chmod to enforce least privilege across the file system | Linux, chmod, File Permissions, Least Privilege |

---

## 🏠 Asset Management

Identifying and classifying assets to support security planning.

| Project | Description | Skills |
|---------|-------------|--------|
| [Home Asset Inventory](home-asset-inventory/README.md) | Created a home network asset inventory classifying devices by ownership, location, and sensitivity level | Asset Classification, Risk Awareness, Inventory Management |

---

## 📓 Incident Handler Journal

A running journal documenting incident handling activities and SOC workflows across multiple scenarios.

| Project | Description | Skills |
|---------|-------------|--------|
| [Incident Handler's Journal](incident-handler-journal/README.md) | Documented multiple cybersecurity incidents including ransomware attacks and phishing investigations following SOC procedures | Incident Documentation, SOC Operations, Post-Mortem Analysis |

---

## 🏛️ Security Governance

Exploring professional cybersecurity organizations and aligning career interests with industry bodies.

| Project | Description | Skills |
|---------|-------------|--------|
| [Security Organization Worksheet](security-governance/Security_organization_worksheet_.pdf) | Researched and compared Cloud Security Alliance (CSA), OWASP, and ISC2 to align professional development with career goals in cloud security and incident response | Security Governance, Professional Development, Cloud Security |

---

## 🛠️ Skills

**Security Operations**
- Alert Triage (Tier 1 & 2)
- Incident Response & Documentation
- IOC Analysis & Threat Intelligence
- MITRE ATT&CK Framework
- NIST Cybersecurity Framework (CSF)
- NIST SP 800-53

**Network Security**
- Wireshark & tcpdump
- TCP/IP Protocol Analysis
- DNS, ICMP, HTTP Analysis
- DoS/DDoS Attack Identification
- Firewall Configuration

**Risk & Compliance**
- Risk Assessment & Risk Registers
- Threat Modeling (PASTA)
- Security Auditing
- PCI DSS, GDPR, SOC Compliance
- Least Privilege & Access Control

**Tools & Technologies**
- SIEM (Google Chronicle, Splunk basics)
- VirusTotal
- Linux (chmod, file permissions)
- SQL (filters, joins)
- Python (file I/O, automation)

---

## 📜 Certifications

| Certification | Issuer | Date |
|---------------|--------|------|
| Google Cybersecurity Professional Certificate | Google / Coursera | June 2026 |
| SOC Bootcamp Certificate | ThinkCloudly | May 2026 |

---

## 🎓 Education

**Master of Science in Information Technology Management**
Campbellsville University, Kentucky — May 2025

