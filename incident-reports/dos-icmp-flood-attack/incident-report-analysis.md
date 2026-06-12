# Incident Report Analysis — DoS ICMP Flood Attack

## Summary

The organization experienced a Denial of Service (DoS) attack that disrupted 
internal network operations for approximately two hours. The attack was 
caused by a flood of incoming ICMP packets that overwhelmed network 
resources and prevented legitimate users from accessing network services. 
Investigation revealed that the attacker exploited an unconfigured firewall, 
which allowed excessive ICMP traffic to enter the network. The incident 
response team mitigated the attack by blocking incoming ICMP traffic, 
temporarily shutting down non-critical services, and restoring critical 
services. The security team later implemented firewall rate limiting, source 
IP verification, network monitoring software, and an IDS/IPS solution to 
reduce the risk of similar attacks in the future.

## Identify

The attack was identified as a Denial of Service (DoS) attack using ICMP 
flood traffic. The primary systems affected were the organization's internal 
network infrastructure, network services, and resources that depended on 
network connectivity. The root cause was an improperly configured firewall 
that failed to restrict incoming ICMP traffic, allowing the attacker to 
overwhelm network resources and disrupt business operations.

## Protect

To strengthen security, the organization should maintain firewall rules that 
limit ICMP traffic and regularly review firewall configurations. Source IP 
verification should remain enabled to identify spoofed packets. The company 
should establish a formal network hardening policy, perform regular security 
audits, apply configuration management procedures, and provide security 
awareness training for IT personnel responsible for firewall administration. 
Additional protections should include network segmentation and periodic 
vulnerability assessments.

## Detect

The organization should use continuous network monitoring software to 
identify abnormal traffic patterns and unusual spikes in ICMP traffic. IDS 
and IPS technologies should be configured to alert security personnel when 
suspicious traffic exceeds established thresholds. Firewall logs, network 
traffic analysis tools, and a SIEM solution should be used to collect and 
correlate security events. Regular monitoring of network performance 
metrics will help identify potential attacks before they significantly 
affect operations.

## Respond

If a similar attack occurs, the incident response team should immediately 
activate the incident response plan, identify affected systems, and contain 
the attack by filtering or blocking malicious traffic. Non-essential services 
may be temporarily isolated to preserve critical business operations. 
Security personnel should collect firewall logs, IDS/IPS alerts, and network 
traffic data for forensic analysis. Communication procedures should ensure 
that management, IT staff, and affected stakeholders receive timely updates. 
After the incident, the team should conduct a lessons-learned review and 
update response procedures as necessary.

## Recover

The organization should restore normal network operations by verifying that 
malicious traffic has been eliminated and confirming that all critical 
services are functioning correctly. System configurations should be reviewed 
and validated before returning services to production. Recovery efforts 
should include restoring any affected services, validating network 
performance, reviewing security controls, and documenting recovery actions. 
Backup configurations and disaster recovery procedures should be tested 
regularly to ensure rapid restoration during future incidents.

## Reflections/Notes

This incident demonstrated the importance of proper firewall configuration, 
continuous monitoring, and layered security controls. Applying the NIST 
Cybersecurity Framework helped identify security gaps and develop a 
structured approach for protecting, detecting, responding to, and recovering 
from cybersecurity incidents. Future security efforts should focus on 
proactive monitoring, regular audits, and continuous improvement of network 
defenses.

---

## Skills Demonstrated
- DoS attack analysis
- NIST Cybersecurity Framework application
- Firewall configuration review
- Incident response (Identify, Protect, Detect, Respond, Recover)
- Network hardening recommendations
