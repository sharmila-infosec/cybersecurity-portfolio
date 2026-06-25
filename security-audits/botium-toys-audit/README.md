# Botium Toys Internal Security Audit

## Objective
Conduct a full internal security audit for a growing e-commerce company using the NIST CSF framework, identify critical compliance gaps, and deliver a prioritized remediation roadmap across PCI DSS, GDPR, and SOC standards.

## Tech Stack
- NIST Cybersecurity Framework (CSF)
- PCI DSS Compliance Assessment
- GDPR Compliance Review
- SOC 1 & 2 Controls Evaluation
- Controls Assessment Matrix

## Results / Impact
- ✅ Identified **3 critical compliance gaps** across PCI DSS, GDPR, and SOC frameworks
- ✅ Flagged **8 missing security controls** including least privilege, MFA, IDS, encryption, and disaster recovery
- ✅ Found that customer cardholder data was accessible to all employees — a direct PCI DSS violation
- ✅ Identified absence of GDPR breach notification plan — a high legal/financial risk for EU operations
- ✅ Delivered prioritized remediation roadmap: critical controls first → compliance gaps → physical security enhancements
- ✅ Physical security controls (locks, CCTV, fire detection) confirmed adequate — no action needed

## Critical Gaps Found

| Gap | Framework Violated | Risk Level |
|-----|-------------------|------------|
| No encryption for cardholder data | PCI DSS | Critical |
| All employees can access sensitive data | PCI DSS / Least Privilege | Critical |
| No GDPR breach notification plan | GDPR | Critical |
| No IDS deployed | NIST CSF | High |
| No disaster recovery plan | SOC / Business Continuity | High |
| No password policy enforced | NIST CSF | High |
| No separation of duties | SOC | Medium |
| Legacy systems unmanaged | NIST CSF | Medium |

## What I Learned
Security audits reveal risks that are invisible in day-to-day operations. Organizations often assume compliance because nothing has gone wrong yet — but a single unencrypted data breach or GDPR violation can cost millions. The NIST CSF provides a structured, repeatable approach to identifying these gaps before attackers or regulators find them first.

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Security Auditing & Compliance
**Frameworks:** NIST CSF | PCI DSS | GDPR | SOC
