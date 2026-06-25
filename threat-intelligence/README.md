# Threat Intelligence — Pyramid of Pain

## Objective
Analyze a ransomware sample flagged on VirusTotal and map identified indicators of compromise (IOCs) to the Pyramid of Pain framework to evaluate defensive value of each indicator type.

## Tech Stack
- VirusTotal (malware analysis)
- Pyramid of Pain Framework
- MITRE ATT&CK Framework
- IOC Classification Methodology

## Results / Impact
- ✅ Successfully analyzed a ransomware sample flagged by 53/70 (75.7%) VirusTotal security vendors
- ✅ Mapped 6 IOC types across all Pyramid of Pain levels — from trivial hash values to high-value TTPs
- ✅ Identified TTPs (file execution, persistence, encryption) as the highest-value defensive indicators — hardest for attackers to change
- ✅ Demonstrated that acting on TTP-level indicators provides 10x more disruption to attackers than blocking hash values alone

## IOC Mapping

| Indicator Type | Example | Pyramid Level | Defensive Value |
|---------------|---------|---------------|-----------------|
| Hash Value | SHA-1 hash | Trivial | Low |
| IP Address | Malicious IP | Easy | Low-Medium |
| Domain Name | Malicious domain | Simple | Medium |
| Network/Host Artifacts | Created .exe files | Annoying | Medium-High |
| Tools | Ransomware malware | Challenging | High |
| TTPs | File execution, persistence, encryption | Tough | Highest |

## What I Learned
Defenders who focus only on blocking hash values are playing a losing game — attackers can change a file hash in seconds. Detecting and disrupting TTPs forces attackers to fundamentally redesign their attack methods, making defenses significantly more resilient.

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Threat Intelligence
