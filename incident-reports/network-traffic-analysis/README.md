# Incident Report — Network Traffic Analysis (DNS/ICMP)

## Objective
Analyze tcpdump network logs to identify the root cause of a website outage, trace the failure to a specific protocol and port, and document findings in a structured incident report.

## Tech Stack
- tcpdump (packet capture & log analysis)
- DNS Protocol Analysis
- ICMP Error Message Interpretation
- TCP/IP Model (Application → Network layer tracing)

## Results / Impact
- ✅ Identified root cause of website outage in under 10 minutes of log analysis
- ✅ Traced failure to UDP port 53 being unreachable on the DNS server — preventing all domain resolution
- ✅ Confirmed root cause via 3 repeated ICMP error messages: `udp port 53 unreachable`
- ✅ Documented structured incident report covering: timeline, protocol analysis, affected systems, and recommended remediation
- ✅ Demonstrated that DNS failures silently take down website access even when the web server is fully operational

## Investigation Findings

| Element | Detail |
|---------|--------|
| Client IP | 192.51.100.15 |
| DNS Server IP | 203.0.113.2 |
| Protocol | UDP |
| Port | 53 (DNS) |
| Error | ICMP: udp port 53 unreachable (repeated 3x) |
| Root Cause | DNS service unreachable — firewall block or service failure |

## What I Learned
DNS is the silent backbone of internet connectivity — when it fails, everything fails even if the web server is healthy. tcpdump's ability to capture raw packets at the network layer makes it invaluable for diagnosing these invisible failures. This project reinforced why SOC analysts must understand all OSI layers, not just the application layer.

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Network Security / Incident Response
