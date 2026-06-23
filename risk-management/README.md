# Risk Management

This folder contains two risk management projects completed as part of the Google Cybersecurity Professional Certificate. Both projects apply structured frameworks to identify, assess, and prioritize security risks.

---

## 📄 Project 1: Risk Register

### Project Description

In this project, I built a risk register for a fictional coastal bank operating with 100 on-premise and 20 remote employees, serving 2,000+ individual and 200 commercial accounts. I identified key assets, described potential threats, and scored each risk by likelihood and severity to calculate a priority score.

### Skills Demonstrated

- Risk Assessment
- Risk Register Creation
- Likelihood and Severity Scoring
- Asset Identification
- Threat Analysis
- Financial Sector Security Awareness

### Risk Scoring Formula

**Priority = Likelihood × Severity** (each scored 1–3)

### Key Risks Identified

| Asset | Risk | Likelihood | Severity | Priority |
|-------|------|-----------|----------|----------|
| Funds | Business Email Compromise (BEC) | 3 | 3 | 9 (High) |
| User Database | Poorly encrypted customer data | 2 | 3 | 6 (Medium) |
| Financial Records | Publicly accessible backup server | 2 | 3 | 6 (Medium) |
| Bank Safe | Left unlocked | 1 | 2 | 2 (Low) |
| Supply Chain | Natural disaster disruption | 1 | 2 | 2 (Low) |

### Key Takeaways

- Business Email Compromise posed the highest risk due to high likelihood and catastrophic impact
- Encryption gaps and exposed backup servers represent significant data security risks
- Risk registers help organizations prioritize remediation based on impact vs. likelihood

---

## 📄 Project 2: PASTA Threat Model Worksheet

### Project Description

In this project, I applied the **PASTA (Process for Attack Simulation and Threat Analysis)** framework to a fictional sneaker marketplace mobile application. I worked through all seven PASTA stages to identify business objectives, technical scope, threats, vulnerabilities, and risk mitigations.

### Skills Demonstrated

- Threat Modeling (PASTA Framework)
- Application Security Analysis
- SQL Injection Identification
- Authentication Vulnerability Assessment
- Risk Mitigation Planning
- Principle of Least Privilege (PoLP)
- Multi-Factor Authentication (MFA)

### PASTA Stages Summary

| Stage | Summary |
|-------|---------|
| I. Business Objectives | Secure mobile app for buying/selling sneakers; protect customer data and payments |
| II. Technical Scope | Prioritized API security due to high-risk communication between app, users, and database |
| III. Application Decomposition | Mapped login flow: user → API → SQL database with encrypted connections |
| IV. Threat Analysis | Identified SQL injection attacks and phishing/credential theft as key threats |
| V. Vulnerability Analysis | Weak input validation and poor authentication/password management |
| VI. Attack Modeling | Mapped attack paths via attack tree diagram |
| VII. Risk & Impact | Recommended MFA, Least Privilege, AES/TLS encryption, and regular security audits |

### Key Takeaways

- The API layer was identified as the highest-risk component due to its role in all data communication
- SQL injection and credential theft were the top threats for this application
- Defense-in-depth controls (MFA, encryption, least privilege, audits) significantly reduce risk exposure

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Risk Management
