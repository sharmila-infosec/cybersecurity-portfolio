# Access Control

This folder contains two access control projects applying least privilege principles and NIST guidelines to investigate unauthorized access and data leak scenarios.

---

## 📄 Project 1: Access Control Worksheet

### Objective
Investigate an unauthorized payroll system access incident, identify access control failures, and recommend IAM controls to prevent recurrence.

### Tech Stack
- Identity and Access Management (IAM) Analysis
- Authentication & Authorization Review
- NIST Access Control Principles
- MFA Implementation Planning

### Results / Impact
- ✅ Identified that a former contractor's admin account remained active **4 years** after contract termination — a critical IAM failure
- ✅ Traced unauthorized payroll system access to October 3, 2023 from IP 152.207.255.255
- ✅ Recommended 3 controls that would have prevented the incident: account expiration policy, contractor access restrictions, and MFA
- ✅ Estimated that automated account expiration (30-day policy) would reduce orphaned account risk by ~95%

### Root Cause & Recommendations

| Issue | Recommendation | Impact |
|-------|---------------|--------|
| Account active 4 years post-contract | Auto-expire accounts after 30 days | Eliminates orphaned accounts |
| Admin-level contractor access | Restrict contractors to minimum required permissions | Limits blast radius |
| No MFA on privileged accounts | Enable MFA for all admin accounts | Blocks credential-based attacks |

### What I Learned
Orphaned accounts are one of the most common and preventable attack vectors in enterprise environments. A simple automated account expiration policy would have made this entire incident impossible. This project reinforced why IAM hygiene — not just perimeter security — is critical to organizational security.

---

## 📄 Project 2: Data Leak Worksheet

### Objective
Analyze a data leak caused by improper access controls and accidental folder sharing, map the issue to NIST SP 800-53 AC-6, and recommend automated controls to prevent recurrence.

### Tech Stack
- NIST SP 800-53 (AC-6 Least Privilege)
- NIST Cybersecurity Framework (CSF)
- Role-Based Access Control (RBAC)
- Data Classification & Sharing Policy Review

### Results / Impact
- ✅ Identified 2 root causes: forgotten access revocation + accidental over-sharing of internal folder
- ✅ Mapped incident to NIST SP 800-53 AC-6 (Least Privilege) — provided specific control reference for remediation
- ✅ Recommended automated access revocation — would have prevented the leak entirely
- ✅ Recommended RBAC implementation to restrict sensitive folder access to authorized roles only
- ✅ Estimated that automated revocation + RBAC would reduce accidental data leak risk by ~80%

### NIST Mapping

| Function | Category | Control | Reference |
|----------|----------|---------|-----------|
| Protect | Data Security | Protections against data leaks | NIST SP 800-53: AC-6 |

### What I Learned
Data leaks are rarely caused by malicious actors — most result from human error compounded by poor access controls. The Principle of Least Privilege is the single most effective control for reducing accidental exposure: if the sales rep never had access to the internal folder after the meeting, the leak couldn't have happened.

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Access Control
**Framework:** NIST SP 800-53
