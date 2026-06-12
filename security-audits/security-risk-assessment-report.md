# Security Risk Assessment Report

## Part 1: Hardening Methods Recommended

After reviewing the organization's vulnerabilities, the following network 
hardening methods are recommended:

1. **Multifactor Authentication (MFA)**
   - Implement MFA for all employee and administrator accounts.
   - MFA requires users to verify their identity using an additional 
     authentication factor, such as a code sent to a mobile device.

2. **Strong Password Policy**
   - Require employees to create strong, unique passwords and prohibit 
     password sharing.
   - Change the default database administrator password immediately and 
     enforce password complexity requirements.

3. **Firewall Rule Configuration**
   - Configure firewall rules to filter incoming and outgoing traffic.
   - Allow only authorized network traffic and block unnecessary ports 
     and connections.

## Part 2: Explanation of Recommendations

**Multifactor Authentication** is effective because it adds an additional 
layer of security beyond a password. Even if an attacker obtains a user's 
password, they would still need the second authentication factor to gain 
access. MFA should be enabled continuously and reviewed periodically.

**Strong Password Policy** is effective because it reduces the likelihood 
of attackers successfully guessing passwords through brute force attacks. 
Password sharing should be prohibited, and employees should receive regular 
security awareness training. Password policies should be enforced at all 
times and reviewed regularly.

**Firewall Rule Configuration** is effective because it helps control the 
traffic entering and leaving the network. Properly configured firewalls 
can block unauthorized access attempts and reduce exposure to network-based 
attacks. Firewall rules should be monitored continuously and reviewed 
whenever network changes occur.

Together, these hardening methods address the organization's identified 
vulnerabilities and significantly reduce the risk of future data breaches.

---

## Skills Demonstrated

- Security risk assessment
- Network hardening strategies
- Multifactor authentication implementation
- Password policy development
- Firewall configuration principles
