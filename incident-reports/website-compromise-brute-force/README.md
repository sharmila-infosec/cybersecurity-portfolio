# Incident Report — Website Compromise via Brute Force Attack

## Project Description

In this project, I investigated a website security incident where a brute force attack led to unauthorized access, malware injection, and malicious redirection of website visitors. I analyzed the attack timeline, identified the methods used, and recommended controls to prevent recurrence.

## Incident Summary

A former employee used a brute force attack to gain access to the admin panel of **yummyrecipesforme.com** using the default admin password. After gaining access, the attacker embedded malicious JavaScript into the website's source code that prompted visitors to download a file. The file redirected users to a fake version of the site and installed malware on their systems.

## Attack Timeline

1. Former employee launched a brute force attack against the admin panel
2. Default admin password was successfully guessed
3. Attacker embedded malicious JavaScript into the website source code
4. Visitors were prompted to download an "update" file
5. The downloaded file redirected users to a fraudulent website (`greatrecipesforme.com`)
6. Malware was installed on visitor devices
7. Incident was reported by multiple customers

## Skills Demonstrated

- Incident Response
- Brute Force Attack Analysis
- Malware Behavior Analysis
- DNS and HTTP Traffic Analysis
- Web Application Security
- MFA Recommendations
- Security Incident Documentation

## Tools Used

- tcpdump (network traffic analysis)
- DNS and HTTP log analysis

## Root Causes

- Admin panel used a **default password** that was not changed
- **No MFA** was configured on the admin account
- **No account lockout policy** to block repeated login attempts

## Recommendations

- Enforce strong, unique passwords and prohibit default credentials
- Implement Multi-Factor Authentication (MFA) on all admin accounts
- Configure account lockout policies after a defined number of failed login attempts
- Perform regular security scans to detect unauthorized changes to website source code
- Monitor DNS traffic for unexpected redirections

## Key Takeaways

- Default passwords are one of the most common and preventable attack vectors
- Brute force attacks are highly effective against accounts with weak or default credentials
- MFA and account lockout policies are essential controls for protecting admin interfaces
- Malicious JavaScript injections can silently compromise thousands of users before detection

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Incident Response / Web Application Security
