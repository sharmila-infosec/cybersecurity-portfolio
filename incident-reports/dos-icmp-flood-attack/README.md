# Incident Report — DoS ICMP Flood Attack (NIST CSF)

## Objective
Apply the complete NIST Cybersecurity Framework (all 5 functions) to analyze an ICMP flood DoS attack that caused a 2-hour network outage, and build a comprehensive incident response and recovery plan.

## Tech Stack
- NIST Cybersecurity Framework (CSF) — all 5 functions
- ICMP Flood Attack Analysis
- Firewall Rule Configuration
- IDS/IPS Deployment
- Network Monitoring Tools

## Results / Impact
- ✅ Applied all 5 NIST CSF functions to structure a complete incident response — Identify → Protect → Detect → Respond → Recover
- ✅ Identified firewall misconfiguration as root cause — unrestricted ICMP traffic allowed attacker to flood the network
- ✅ Restored all critical network services within the 2-hour outage window through structured response
- ✅ Implemented new firewall rule to rate-limit ICMP packets — prevents recurrence of same attack vector
- ✅ Deployed source IP verification to detect and drop spoofed ICMP packets going forward
- ✅ Recommended IDS/IPS deployment to automatically detect abnormal ICMP traffic patterns

## NIST CSF Response Summary

| Function | Actions Taken | Outcome |
|----------|--------------|---------|
| **Identify** | Identified ICMP flood + firewall misconfiguration | Root cause confirmed |
| **Protect** | New firewall rule limiting ICMP rate + IP verification | Attack vector closed |
| **Detect** | Network monitoring + IDS/IPS deployed | Early warning system active |
| **Respond** | Blocked flood, took non-critical services offline, restored critical first | Outage minimized |
| **Recover** | Restored all services, communicated status, post-incident review scheduled | Full recovery achieved |

## What I Learned
The NIST CSF transforms chaotic incident response into a structured, repeatable process. Without a framework, teams react — with it, they respond. The most important lesson: a single unconfigured firewall rule caused a 2-hour outage. Regular firewall audits and the principle of default-deny would have prevented this entirely.

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Incident Response / Network Security
**Framework:** NIST Cybersecurity Framework (CSF)
