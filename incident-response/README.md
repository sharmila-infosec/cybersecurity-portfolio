# Incident Response

This folder contains two SOC-level incident response projects completed as part of the Google Cybersecurity Professional Certificate.

---

## 📄 Project 1: Alert Ticket — Phishing with Malicious Attachment

### Objective
Triage a medium-severity phishing alert, verify the malicious attachment using VirusTotal, and make an escalation decision with documented findings.

### Tech Stack
- VirusTotal (IOC verification)
- IDS/IPS Alert System
- Incident Ticketing Workflow
- SHA-256 Hash Analysis

### Results / Impact
- ✅ Correctly identified and escalated a confirmed phishing attack with malicious .exe attachment
- ✅ Verified file hash against 70 security vendors — 53/70 flagged as malicious (75.7% detection rate)
- ✅ Reduced investigation time by applying structured triage: sender analysis → hash check → escalation
- ✅ Documented IOCs (file hash, sender domain, IP) enabling faster Tier 2 response

### Alert Details

| Field | Details |
|-------|---------|
| Ticket ID | A-2703 |
| Severity | Medium |
| File | bfsvc.exe |
| Hash | 54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b |
| Status | Escalated to Tier 2 |

### What I Learned
Structured triage checklists dramatically reduce time-to-escalation. Verifying file hashes with VirusTotal before escalating ensures Tier 2 analysts receive actionable, pre-validated findings rather than raw alerts — reducing unnecessary escalations and false positives.

---

## 📄 Project 2: Parking Lot USB Exercise

### Objective
Apply attacker mindset thinking to analyze a USB baiting scenario and recommend organizational controls to prevent removable media attacks.

### Tech Stack
- Threat Analysis Framework
- Social Engineering Risk Assessment
- Endpoint Security Policy Review

### Results / Impact
- ✅ Identified 3 distinct attack vectors from a single USB device (malware, phishing, data theft)
- ✅ Recommended 5 layered controls: employee training, autorun disabling, isolated scanning, endpoint protection, and file separation policy
- ✅ Demonstrated attacker mindset by mapping PII exposure to targeted social engineering scenarios

### What I Learned
Physical security threats are often underestimated in digital security planning. A single USB device can compromise an entire network — combining technical controls with employee awareness training is the most effective defense.

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Incident Response / SOC Operations
