# Cybersecurity Incident Report — SYN Flood DoS Attack

## Section 1: Identify the Type of Attack

The web server was experiencing a TCP SYN Flood attack that caused it to 
become overloaded and unable to respond to legitimate user requests.

**Log findings:**
The network logs show a large number of TCP SYN packets coming from the IP 
address 203.0.113.0. The server initially responded to these requests, but 
the attacker continued sending SYN packets at a very high rate. As the 
attack continued, legitimate users started receiving timeout and connection 
reset errors. Eventually, the server stopped responding to normal traffic.

**Classification:**
This event is a Denial of Service (DoS) attack, specifically a SYN Flood 
attack. Since the attack originated from a single IP address, it is 
classified as a DoS attack rather than a Distributed Denial of Service 
(DDoS) attack.

## Section 2: How the Attack Causes the Website to Malfunction

**The TCP three-way handshake:**
1. The client sends a SYN packet to the server requesting a connection.
2. The server responds with a SYN-ACK packet to acknowledge the request.
3. The client sends an ACK packet back to the server, completing the 
   connection.

**Effect of a SYN flood:**
When a malicious actor sends thousands of SYN packets, the server attempts 
to respond to each request and reserves resources for incomplete 
connections. As the number of requests increases, the server's resources 
become exhausted, preventing it from handling legitimate traffic.

**Log analysis and server impact:**
The logs indicate that the attacker continuously sent SYN packets to the 
web server without establishing normal connections. This caused the server 
to become overwhelmed and unable to process legitimate user requests. As a 
result, employees and customers experienced connection timeouts, failed 
webpage requests, and website unavailability. This attack negatively 
impacted business operations because users could no longer access the 
company's sales webpage.

## Recommendations

To prevent similar attacks in the future, the organization should implement 
SYN flood protection, configure rate limiting on the firewall, deploy 
intrusion prevention systems (IPS), and continuously monitor network traffic 
for suspicious activity.

---

## Skills Demonstrated
- TCP/IP protocol analysis (three-way handshake)
- DoS/SYN flood attack identification
- Network log interpretation
- Security remediation recommendations (rate limiting, IPS, monitoring)
