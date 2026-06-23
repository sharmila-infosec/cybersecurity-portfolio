# Access Control

This folder contains two access control projects completed as part of the Google Cybersecurity Professional Certificate. Both projects apply access control principles and NIST guidelines to investigate real-world security scenarios.

---

## 📄 Project 1: Access Control Worksheet

### Project Description

In this project, I investigated an unauthorized access incident where a former contractor's account accessed the payroll system four years after their contract ended. I identified the authorization issues and recommended controls to prevent similar incidents.

### Incident Details

- **Date of Incident:** October 3, 2023
- **User:** Robert Taylor Jr. (Legal/Administrator)
- **IP Address:** 152.207.255.255
- **Issue:** Former contractor's admin account remained active and accessed the payroll system in 2023 — four years after their contract ended in 2019

### Skills Demonstrated

- Access Control Analysis
- Authentication and Authorization Review
- Incident Investigation
- Principle of Least Privilege
- Multi-Factor Authentication (MFA)
- Identity and Access Management (IAM)

### Recommendations

- User accounts should automatically expire after 30 days of inactivity or contract end
- Contractors should have limited, role-based access to business resources
- Enable Multi-Factor Authentication (MFA) for all privileged accounts
- Conduct regular audits of active user accounts and permissions

### Key Takeaways

- Inactive accounts pose a serious insider threat risk if not properly deprovisioned
- Automated account expiration and regular privilege audits are critical controls
- MFA adds an important layer of protection even if credentials are compromised

---

## 📄 Project 2: Data Leak Worksheet

### Project Description

In this project, I analyzed a data leak caused by improper sharing of an internal folder during a sales team meeting. The leak resulted in confidential product information being posted publicly on social media by a business partner. I mapped the issue to **NIST SP 800-53 AC-6 (Least Privilege)** and recommended controls to prevent recurrence.

### Incident Summary

A sales manager shared an internal folder containing unreleased product information, customer analytics, and promotional materials with the team. The manager did not revoke access after the meeting. During a later video call, a sales representative accidentally shared the internal folder link (instead of just the promotional materials) with a business partner, who then posted it publicly on social media.

### Skills Demonstrated

- Data Leak Analysis
- NIST SP 800-53 (AC-6 Least Privilege)
- NIST Cybersecurity Framework (CSF)
- Access Control Policy Recommendations
- Role-Based Access Control (RBAC)
- Security Incident Documentation

### NIST Framework Mapping

| Function | Category | Subcategory | Reference |
|----------|----------|-------------|-----------|
| Protect | PR.DS: Data Security | PR.DS-5: Protections against data leaks | NIST SP 800-53: AC-6 |

### Recommendations

1. **Automatically revoke access** to shared folders after a defined period or when the task is complete
2. **Regularly audit user privileges** and enforce role-based access controls
3. **Train employees** on proper data sharing procedures and the risks of over-sharing

### Key Takeaways

- The Principle of Least Privilege (AC-6) is essential to preventing accidental data exposure
- Automated access revocation eliminates the risk of forgotten permissions
- Human error is a leading cause of data leaks — technical controls must support employee behavior

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Access Control
**Framework:** NIST SP 800-53
