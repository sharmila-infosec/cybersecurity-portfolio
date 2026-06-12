# Network Traffic Analysis — DNS/ICMP Incident Report

## Part 1: Summary of the Problem

The tcpdump log analysis revealed that DNS requests sent via UDP to port 53 
were not reaching the DNS server. The client repeatedly sent DNS queries 
for www.yummyrecipesforme.com, but received ICMP error responses stating 
"udp port 53 unreachable."

**Protocols identified:**
- UDP — used for outgoing DNS queries
- ICMP — used for the error responses
- DNS — the service affected (port 53)

## Part 2: Analysis and Root Cause

**Time of Incident:** 13:24:32 (1:24 PM)

**How the issue was discovered:**
Multiple users reported being unable to access www.yummyrecipesforme.com 
and received a "destination port unreachable" error. The analyst reproduced 
the issue and captured network traffic using tcpdump.

**Investigation actions:**
- Captured and reviewed network traffic logs using tcpdump
- Examined DNS requests sent from the client (192.51.100.15) to the DNS 
  server (203.0.113.2)
- Analyzed the ICMP error responses returned by the server

**Key findings:**
- DNS requests were sent using UDP port 53
- The DNS server IP address was 203.0.113.2
- ICMP responses repeatedly returned "udp port 53 unreachable"
- The DNS server was unable to process DNS requests
- Because DNS resolution failed, users could not access the website

**Suspected root cause:**
A DNS service outage or misconfiguration caused UDP port 53 on the DNS 
server to become unavailable. A firewall rule blocking DNS traffic to 
port 53 is also a possible cause.

---

## Skills Demonstrated
- Network traffic analysis
- tcpdump log interpretation
- DNS and ICMP protocol analysis
- TCP/IP model layer identification
- Cybersecurity incident documentation
