# Incident Report — SYN Flood DoS Attack

## Project Description

In this project, I investigated a Denial of Service (DoS) attack targeting a travel agency's web server. I analyzed network logs to identify the attack type, explained how the TCP three-way handshake was exploited, and recommended mitigations to restore and protect service availability.

## Incident Summary

The web server of a travel agency became unresponsive, causing the website to go offline. Employees and customers were unable to access the site. Network log analysis revealed a large volume of TCP SYN packets flooding the server without completing the three-way handshake — a classic **SYN Flood DoS attack**.

## How the Attack Worked

The TCP three-way handshake normally works as follows:

| Step | Action |
|------|--------|
| 1 | Client sends **SYN** packet to server |
| 2 | Server responds with **SYN-ACK** |
| 3 | Client sends **ACK** to complete the connection |

In a SYN Flood attack:
- The attacker sends a massive volume of SYN packets
- The server responds with SYN-ACK and waits for the final ACK
- The attacker never sends the ACK, leaving connections half-open
- The server's connection table fills up and it can no longer accept legitimate connections

## Skills Demonstrated

- DoS/DDoS Attack Identification
- TCP/IP Protocol Analysis
- Network Log Analysis
- SYN Flood Attack Understanding
- Incident Response Documentation
- Network Security Hardening Recommendations

## Tools Used

- Network log analysis
- TCP/IP protocol knowledge

## Recommendations

- **Enable SYN cookies** on the web server to handle half-open connections without filling the connection table
- **Configure rate limiting** on the firewall to restrict the number of SYN packets from a single source
- **Deploy a Web Application Firewall (WAF)** to filter malicious traffic before it reaches the server
- **Use a load balancer** to distribute traffic and absorb volumetric attacks
- **Contact ISP** for upstream traffic filtering during active attacks

## Key Takeaways

- SYN Flood attacks exploit the TCP handshake process to exhaust server resources
- Even a single attacker can take down a web server with enough SYN packets
- Firewall rate limiting and SYN cookies are effective first-line defenses against SYN Flood attacks
- Network log analysis is essential for quickly identifying the type and source of a DoS attack

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Incident Response / Network Security
