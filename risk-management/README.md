# Risk Management

This folder contains two risk management projects applying structured frameworks to identify, assess, and prioritize security risks.

---

## 📄 Project 1: Risk Register

### Objective
Build a prioritized risk register for a banking environment to help security teams focus remediation efforts on the highest-impact threats.

### Tech Stack
- Risk Scoring Matrix (Likelihood × Severity)
- Asset-Based Risk Assessment
- Financial Sector Threat Modeling

### Results / Impact
- ✅ Identified and scored 5 key risks across a banking environment with 120 employees and 2,200+ accounts
- ✅ Flagged Business Email Compromise (BEC) as the highest-priority risk (score: 9/9) due to high likelihood and catastrophic financial impact
- ✅ Identified 2 medium-priority data security risks (score: 6/9) — poorly encrypted customer database and publicly accessible backup server
- ✅ Prioritized remediation roadmap: BEC controls → encryption → access controls → physical security

### Risk Scoring Summary

| Asset | Risk | Priority Score |
|-------|------|---------------|
| Funds | Business Email Compromise | 9 (Critical) |
| User Database | Poor encryption | 6 (Medium) |
| Financial Records | Exposed backup server | 6 (Medium) |
| Bank Safe | Left unlocked | 2 (Low) |
| Supply Chain | Natural disaster | 2 (Low) |

### What I Learned
Risk registers force security teams to move beyond gut feelings and apply objective scoring. Quantifying risk by likelihood × severity ensures the most dangerous threats get addressed first — preventing alert fatigue from low-priority issues consuming limited security resources.

---

## 📄 Project 2: PASTA Threat Model Worksheet

### Objective
Apply the PASTA (Process for Attack Simulation and Threat Analysis) framework to a mobile application to identify threats, model attack paths, and recommend mitigations before deployment.

### Tech Stack
- PASTA Threat Modeling Framework (7 stages)
- SQL Injection Analysis
- Authentication Vulnerability Assessment
- Mobile Application Security (API security focus)

### Results / Impact
- ✅ Completed all 7 PASTA stages for a sneaker marketplace mobile application
- ✅ Identified the API layer as the highest-risk component — handles all user-database communication
- ✅ Modeled 5 attack vectors including SQL injection and credential theft
- ✅ Recommended 4 mitigations: MFA, Principle of Least Privilege, AES/TLS encryption, and regular security audits
- ✅ Reduced projected attack surface by recommending input validation controls to block SQL injection at source

### PASTA Stages Completed

| Stage | Key Output |
|-------|-----------|
| Business Objectives | Secure checkout, user privacy, reliable payments |
| Technical Scope | API identified as highest-risk component |
| App Decomposition | Login flow mapped: user → API → SQL database |
| Threat Analysis | SQL injection + credential theft identified |
| Vulnerability Analysis | Weak input validation + poor authentication |
| Attack Modeling | Attack tree diagram completed |
| Risk & Impact | MFA + PoLP + AES/TLS + audits recommended |

### What I Learned
Threat modeling before deployment is far cheaper than remediating breaches after. The PASTA framework's business-first approach ensures security recommendations are practical and aligned with real organizational priorities — not just theoretical security ideals.

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Risk Management
