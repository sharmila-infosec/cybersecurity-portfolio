# Threat Intelligence — Pyramid of Pain

## Project Description

In this project, I analyzed a ransomware sample that was flagged as malicious by 53 out of 70 security vendors on VirusTotal. I then mapped the identified indicators of compromise (IOCs) to the **Pyramid of Pain** framework to evaluate how difficult each indicator would be for an attacker to change if defenders acted on them.

## Objectives

- Identify and classify IOCs from a VirusTotal malware report
- Map each indicator to its corresponding level in the Pyramid of Pain
- Understand which IOCs provide the highest defensive value
- Practice threat intelligence analysis using real-world tools

## Skills Demonstrated

- Threat Intelligence Analysis
- IOC Identification and Classification
- Pyramid of Pain Framework
- VirusTotal Analysis
- MITRE ATT&CK Awareness
- Malware Behavior Analysis

## Tools Used

- VirusTotal
- Pyramid of Pain Framework

## Key Findings

| Indicator Type | Example | Pyramid Level |
|---------------|---------|---------------|
| Hash Value | SHA-1 hash of malicious file | Trivial |
| IP Address | Contacted malicious IP | Easy |
| Domain Name | Contacted malicious domain | Simple |
| Network/Host Artifacts | Created .exe files | Annoying |
| Tools | Ransomware malware | Challenging |
| TTPs | File execution, persistence, file encryption | Tough |

## Key Takeaways

- Hash values are the easiest IOC for attackers to change and provide the least long-term value
- TTPs (Tactics, Techniques, and Procedures) are the hardest for attackers to change and provide the most defensive value
- VirusTotal confirmed the file was malicious based on 53/70 vendor detections and behavioral indicators
- Understanding the Pyramid of Pain helps security teams prioritize which IOCs to act on for maximum impact

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Threat Intelligence
