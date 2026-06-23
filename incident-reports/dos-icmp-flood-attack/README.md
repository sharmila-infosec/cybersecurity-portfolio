# Incident Report — DoS ICMP Flood Attack (NIST CSF)

## Project Description

In this project, I analyzed a Denial of Service (DoS) attack using ICMP flood traffic that caused a network outage for a multimedia company. I applied the **NIST Cybersecurity Framework (CSF)** — working through all five functions (Identify, Protect, Detect, Respond, Recover) — to structure a comprehensive incident response and remediation plan.

## Incident Summary

A multimedia company experienced a network outage lasting approximately two hours. During this time, all internal network services were non-functional. Investigation revealed that the company was flooded with ICMP ping packets from a malicious actor, overwhelming the network and preventing legitimate traffic from flowing.

The attack was possible because the internal firewall had not been properly configured, allowing ICMP packets to enter without restriction.

## NIST CSF Response

| Function | Actions Taken |
|----------|--------------|
| **Identify** | Identified the ICMP flood as the attack vector; confirmed firewall misconfiguration allowed unrestricted ICMP traffic |
| **Protect** | Implemented a new firewall rule to limit the rate of incoming ICMP packets; deployed source IP address verification to detect spoofed IPs |
| **Detect** | Configured network monitoring software to detect abnormal ICMP traffic patterns; installed IDS/IPS to filter suspicious traffic |
| **Respond** | Blocked incoming ICMP flood traffic; took non-critical services offline; restored critical services first; notified management and documented the incident |
| **Recover** | Restored all network services; communicated recovery status to staff; scheduled a post-incident review to improve detection and response procedures |

## Skills Demonstrated

- NIST Cybersecurity Framework (CSF) Application
- DoS/DDoS Attack Identification
- ICMP Flood Attack Analysis
- Firewall Configuration and Rule Management
- IDS/IPS Deployment
- Incident Response Planning
- Network Recovery Procedures
- Incident Documentation

## Tools & Frameworks Used

- NIST Cybersecurity Framework (CSF)
- Firewall rule management
- IDS/IPS systems
- Network monitoring software

## Root Cause

The firewall lacked a rule to limit or block incoming ICMP traffic, allowing the attacker to flood the network unchecked.

## Recommendations

- Configure firewall rules to rate-limit ICMP packets and block suspicious sources
- Deploy source IP verification to detect and drop spoofed ICMP packets
- Implement IDS/IPS to detect abnormal ICMP traffic patterns automatically
- Conduct regular firewall audits to ensure rules are current and correctly configured

## Key Takeaways

- Firewall misconfigurations are a leading cause of successful DoS attacks
- The NIST CSF provides a structured, repeatable approach to incident response that covers prevention, detection, and recovery
- Network monitoring and IDS/IPS tools are essential for detecting DoS attacks early
- A well-documented incident response plan significantly reduces recovery time

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Incident Response / Network Security
**Framework:** NIST Cybersecurity Framework (CSF)
