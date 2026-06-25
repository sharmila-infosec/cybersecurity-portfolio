# Incident Report — SYN Flood DoS Attack

## Objective
Investigate a Denial of Service attack on a travel agency web server, identify the attack type by analyzing TCP handshake anomalies in network logs, and recommend mitigations to restore and protect service availability.

## Tech Stack
- Network Log Analysis
- TCP/IP Protocol Analysis (Three-Way Handshake)
- SYN Flood Attack Pattern Recognition
- Firewall Rule Design
- DoS Mitigation Strategies

## Results / Impact
- ✅ Identified SYN Flood DoS attack as root cause of complete web server outage
- ✅ Analyzed TCP handshake anomalies — confirmed thousands of half-open connections exhausting server resources
- ✅ Recommended SYN cookies as primary mitigation — eliminates half-open connection table overflow without blocking legitimate traffic
- ✅ Recommended rate limiting to reduce attack bandwidth by ~80% at the firewall level
- ✅ Documented full incident report with attack timeline, technical analysis, and layered mitigation plan

## How the Attack Worked

| Step | Normal TCP | SYN Flood Attack |
|------|-----------|-----------------|
| 1 | Client sends SYN | Attacker sends thousands of SYNs |
| 2 | Server sends SYN-ACK | Server sends thousands of SYN-ACKs |
| 3 | Client sends ACK ✅ | Attacker never sends ACK ❌ |
| Result | Connection established | Server fills with half-open connections → crashes |

## Mitigations Recommended

| Control | Impact |
|---------|--------|
| SYN Cookies | Eliminates half-open connection table overflow |
| Firewall Rate Limiting | Reduces attack volume by ~80% |
| Web Application Firewall (WAF) | Filters malicious traffic upstream |
| Load Balancer | Distributes and absorbs volumetric traffic |
| ISP-Level Filtering | Blocks traffic before reaching the network |

## What I Learned
SYN Flood attacks are devastatingly simple yet highly effective — a single attacker can take down a web server by exploiting a fundamental TCP design assumption. Defense requires multiple layers: rate limiting at the firewall, SYN cookies at the OS level, and upstream ISP filtering for large-scale attacks.

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Incident Response / Network Security
