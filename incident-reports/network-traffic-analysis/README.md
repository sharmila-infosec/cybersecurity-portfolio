# Incident Report — Network Traffic Analysis (DNS/ICMP)

## Project Description

In this project, I analyzed network traffic logs captured using **tcpdump** to investigate a cybersecurity incident where users were unable to access a website. I identified the root cause of the outage by interpreting DNS and ICMP protocol behavior in the captured logs.

## Incident Summary

Users reported being unable to access **www.yummyrecipesforme.com**. Network traffic was captured and analyzed to determine why the website was unreachable.

## Investigation Findings

- DNS requests were sent via UDP from the client (`192.51.100.15`) to the DNS server (`203.0.113.2`) on **port 53**
- The DNS server returned repeated **ICMP error messages**: `udp port 53 unreachable`
- The same error occurred 3 times, confirming the DNS service was consistently failing

## Root Cause

UDP port 53 was unreachable on the DNS server, meaning DNS resolution failed and the website could not be accessed. Possible causes include:

- DNS service was down or misconfigured on the server
- A firewall rule was blocking inbound traffic to UDP port 53
- The DNS server was overwhelmed or unresponsive

## Skills Demonstrated

- Network Traffic Analysis
- tcpdump Log Interpretation
- DNS Protocol Analysis
- ICMP Error Message Analysis
- TCP/IP Model Understanding
- Cybersecurity Incident Documentation

## Tools Used

- tcpdump

## Protocols Analyzed

| Protocol | Port | Role in Incident |
|----------|------|-----------------|
| UDP | 53 | Used for DNS requests — was unreachable |
| DNS | 53 | Failed to resolve the domain name |
| ICMP | — | Returned error messages indicating port 53 was unreachable |

## Key Takeaways

- DNS failures can take down website access entirely even if the web server itself is functioning
- ICMP error messages are a critical diagnostic tool for identifying network-level failures
- tcpdump is a powerful command-line tool for capturing and analyzing real-time network traffic
- Documenting the 5 W's (Who, What, Where, When, Why) during investigation ensures thorough incident reporting

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Incident Response / Network Security
