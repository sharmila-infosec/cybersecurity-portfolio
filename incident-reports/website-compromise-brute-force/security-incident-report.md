# Security Incident Report — Website Compromise via Brute Force Attack

## Section 1: Network Protocols Identified

The network protocols identified during the investigation were DNS (Domain 
Name System) and HTTP (Hypertext Transfer Protocol). DNS was used to 
resolve the domain names yummyrecipesforme.com and greatrecipesforme.com 
into IP addresses. HTTP was used to establish web connections and transfer 
webpage data between the user's browser and the websites. The tcpdump log 
showed DNS queries followed by HTTP GET requests to both websites.

## Section 2: Incident Documentation

Multiple customers reported that yummyrecipesforme.com prompted them to 
download an executable file claiming to provide access to free recipes. 
After executing the file, users were redirected to greatrecipesforme.com 
and experienced reduced system performance.

The cybersecurity team created a sandbox environment and analyzed the 
network traffic using tcpdump. The packet capture showed a DNS request for 
yummyrecipesforme.com followed by an HTTP connection to the website. 
Shortly afterward, the browser initiated a download and then generated a 
DNS request for greatrecipesforme.com. The DNS server returned the IP 
address associated with the new domain, and the browser established an 
HTTP connection with that website.

Further investigation confirmed that the website had been compromised. A 
former employee gained unauthorized access to the web hosting 
administrative account through a brute force attack, successfully guessing 
the default administrator password after multiple login attempts. Once 
access was obtained, the attacker inserted malicious JavaScript into the 
website source code, prompting visitors to download an executable file. 
This file redirected users to greatrecipesforme.com, where malware was 
hosted. The attacker also changed the administrator password, locking out 
the website owner.

**Evidence used:**
- Customer complaints
- tcpdump network traffic logs
- Website source code analysis
- Malware file analysis

## Section 3: Remediation Recommendation

One effective security measure is implementing multi-factor authentication 
(MFA) for all administrative accounts. MFA requires users to provide an 
additional authentication factor beyond a password, such as a verification 
code generated on a mobile device. Even if an attacker successfully guesses 
or obtains a password, they would still need the second authentication 
factor to gain access. This significantly reduces the likelihood of 
successful brute force attacks and improves overall account security.

---

## Skills Demonstrated
- Network traffic analysis (DNS, HTTP)
- Malware analysis
- Incident documentation
- Root cause analysis
- Security remediation recommendations (MFA)
