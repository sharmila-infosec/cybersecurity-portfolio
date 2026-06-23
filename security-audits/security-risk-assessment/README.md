# Security Risk Assessment Report

## Project Description

In this project, I analyzed a network hardening scenario where an organization suffered a data breach due to several security vulnerabilities. I identified the key security risks, evaluated the causes, and recommended specific network hardening tools and methods to reduce the organization's attack surface and prevent future incidents.

## Scenario

A social media organization experienced a major data breach that exposed customers' personal information including names, addresses, and credit card numbers. After investigation, four key vulnerabilities were identified that contributed to the breach.

## Vulnerabilities Identified

1. Employees sharing passwords
2. Admin password for the database set to default
3. Firewall with no rules configured for filtering traffic
4. No MFA in use across the organization

## Skills Demonstrated

- Network Security Risk Assessment
- Security Hardening Recommendations
- Firewall Configuration Analysis
- Multi-Factor Authentication (MFA) Planning
- Password Policy Development
- Network Hardening Best Practices

## Recommended Hardening Methods

| Vulnerability | Recommended Control | Frequency |
|--------------|---------------------|-----------|
| Shared passwords | Enforce password policies; prohibit sharing | Immediate + ongoing |
| Default admin password | Change all default credentials immediately | Immediate |
| No firewall rules | Configure firewall rules to filter inbound/outbound traffic | Immediate + quarterly review |
| No MFA | Implement MFA for all user and admin accounts | Immediate |

## Key Recommendations

- **Password Policy:** Enforce minimum complexity, length requirements, and prohibit sharing; implement a centralized password manager
- **MFA:** Require multi-factor authentication for all accounts, especially privileged ones
- **Firewall Rules:** Define and enforce rules to block unauthorized traffic, limit exposure, and log all connections
- **Default Credential Policy:** Mandate immediate change of all default passwords upon system deployment

## Key Takeaways

- Default credentials and shared passwords are among the most easily exploited vulnerabilities
- MFA is one of the most effective controls for preventing unauthorized account access
- Firewall rule management is a foundational network security practice that requires regular review
- A layered approach to security hardening significantly reduces the overall attack surface

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Network Security / Risk Assessment
