# Internal Security Audit — Botium Toys

**Course:** Google Cybersecurity Certificate  
**Framework Used:** NIST CSF  
**Date:** June 2026  

---

## Scenario Summary
Botium Toys is a small U.S. toy company with growing online presence 
including EU customers. An internal IT audit was conducted to assess 
security posture, identify risks, and ensure compliance with PCI DSS 
and GDPR regulations.

---

## Controls Assessment Checklist

| Control | In Place |
|--------|----------|
| Least Privilege | ❌ No |
| Disaster Recovery Plans | ❌ No |
| Password Policies | ❌ No |
| Separation of Duties | ❌ No |
| Firewall | ✅ Yes |
| Intrusion Detection System (IDS) | ❌ No |
| Backups | ❌ No |
| Antivirus Software | ✅ Yes |
| Manual Monitoring for Legacy Systems | ❌ No |
| Encryption | ❌ No |
| Password Management System | ❌ No |
| Locks (offices, storefront, warehouse) | ✅ Yes |
| CCTV Surveillance | ✅ Yes |
| Fire Detection/Prevention | ✅ Yes |

---

## Compliance Checklist

### PCI DSS
| Best Practice | Status |
|--------------|--------|
| Only authorized users access credit card info | ❌ No |
| Credit card data stored in secure environment | ❌ No |
| Encryption for credit card transactions | ❌ No |
| Secure password management policies | ❌ No |

### GDPR
| Best Practice | Status |
|--------------|--------|
| EU customers data is kept private/secured | ❌ No |
| 72-hour breach notification plan exists | ✅ Yes |
| Data is properly classified and inventoried | ❌ No |
| Privacy policies documented and maintained | ✅ Yes |

### SOC Type 1 & Type 2
| Best Practice | Status |
|--------------|--------|
| User access policies are established | ❌ No |
| Sensitive data (PII/SPII) is confidential | ❌ No |
| Data integrity is validated | ✅ Yes |
| Data available to authorized individuals | ✅ Yes |

---

## Recommendations

1. **Implement Least Privilege and Separation of Duties** — Currently 
all employees have access to sensitive customer and credit card data. 
Access should be restricted so employees only access data necessary 
for their role, reducing insider threat risk and improving PCI DSS 
and SOC compliance.

2. **Establish Encryption** — No encryption is currently in place for 
stored or transmitted data. Encryption must be implemented immediately 
for all sensitive customer and credit card data to meet PCI DSS and 
GDPR requirements.

3. **Strengthen Password Policies and Implement a Password Management 
System** — Current password requirements are weak. Strong password 
policies and a centralized password management system should be 
enforced to protect against unauthorized access and meet PCI DSS 
standards.

4. **Create a Disaster Recovery Plan** — No disaster recovery plan 
exists. A formal plan must be developed to ensure business continuity 
in the event of a system failure, cyberattack, or natural disaster.

5. **Set Up Regular Backups** — There are currently no backups in 
place. Automated and regular data backups should be implemented to 
prevent permanent data loss during incidents.

6. **Install an Intrusion Detection System (IDS)** — No IDS exists 
to monitor for active threats. Installing an IDS will allow the IT 
team to detect and respond to suspicious network activity before it 
causes serious damage.

7. **Create a Monitoring and Maintenance Schedule for Legacy Systems** 
— Legacy systems are not being regularly monitored or maintained. A 
clear schedule and assigned responsibility should be established to 
reduce vulnerabilities in outdated systems.

8. **Classify and Inventory All Data Assets** — Data is not properly 
classified or inventoried. A full data classification system should 
be created, especially for EU customer data, to meet GDPR requirements 
and improve overall data management.

9. **Restrict Access to Credit Card Information** — Only authorized 
payment-processing staff should have access to customers credit card 
data. This is a direct PCI DSS requirement and significantly reduces 
the risk of financial data exposure.

10. **Enforce and Document Privacy Policies for EU Customers** — While 
a 72-hour breach notification plan exists, data privacy policies need 
to be fully enforced and documented across the organization to maintain 
full GDPR compliance and protect EU customer data.

---

## Skills Demonstrated
- Internal security auditing
- NIST CSF framework application
- Risk assessment analysis
- PCI DSS compliance evaluation
- GDPR compliance evaluation
- SOC controls evaluation
- Security recommendations and reporting
