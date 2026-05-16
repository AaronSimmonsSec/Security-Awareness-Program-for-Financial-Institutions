# Blue Team Incident Response Tabletop Exercise  
## Security Operations & Incident Response Scenario  
### Security Awareness Program for Financial Institutions

This page provides a technical tabletop exercise scenario designed specifically for Security Operations Center (SOC), Incident Response (IR), Threat Hunting, and Blue Team personnel within a financial institution environment.

The scenario simulates a realistic multi-stage cyberattack targeting enterprise systems, employee credentials, and sensitive financial data to evaluate detection, escalation, containment, analysis, communication, and recovery capabilities.

---

# Purpose

This exercise is designed to evaluate the operational effectiveness of:

- Security Operations Center (SOC) procedures
- Incident Response processes
- Blue Team coordination
- Threat detection capabilities
- Escalation discipline
- Cross-functional cyber response
- Executive communications
- Recovery readiness
- Human decision-making under pressure

---

# Exercise Overview

| Field | Description |
|---|---|
| Exercise Type | Technical Tabletop Exercise |
| Audience | SOC, IR, Threat Hunting, Engineering, Management |
| Threat Theme | Phishing → Credential Theft → Lateral Movement → Data Exfiltration |
| Difficulty | Intermediate to Advanced |
| Duration | 2–4 Hours |
| Environment | Financial Institution |
| Exercise Style | Discussion-Based with Technical Injects |

---

# Table of Contents

- [Scenario Objectives](#scenario-objectives)
- [Scenario Background](#scenario-background)
- [Attack Narrative](#attack-narrative)
- [Exercise Timeline](#exercise-timeline)
- [Technical Injects](#technical-injects)
- [Blue Team Discussion Questions](#blue-team-discussion-questions)
- [Expected Detection Opportunities](#expected-detection-opportunities)
- [MITRE ATT&CK Mapping](#mitre-attck-mapping)
- [NIST & CRI Framework Mapping](#nist--cri-framework-mapping)
- [Scoring and Evaluation](#scoring-and-evaluation)
- [After-Action Review](#after-action-review)

---

# Scenario Objectives

The exercise is intended to validate the organization’s ability to:

- Detect malicious activity across multiple security tools
- Escalate incidents appropriately
- Coordinate investigation activities
- Contain compromised systems and accounts
- Analyze indicators of compromise (IOCs)
- Communicate effectively across teams
- Make risk-based operational decisions
- Recover affected systems safely
- Document investigative findings accurately

---

# Scenario Background

A threat actor targets employees at a regional financial institution using a phishing campaign impersonating a trusted vendor relationship.

An employee receives an email containing a malicious authentication link designed to harvest credentials. Shortly after successful credential compromise, the attacker gains access to cloud services using valid credentials and begins establishing persistence.

The threat actor then attempts:

- Mailbox rule creation
- Privilege escalation
- Internal reconnaissance
- Lateral movement
- Access to file shares
- Potential customer data exfiltration

The Security Operations Center begins receiving multiple low-confidence alerts across various security tools.

The exercise begins at the point where analysts must determine whether the activity represents a legitimate security incident.

---

# Attack Narrative

## Phase 1 — Initial Access

The attacker sends a phishing email spoofing a third-party vendor.

The employee:

- Opens the message
- Clicks the embedded link
- Enters credentials into a fake authentication portal

---

## Phase 2 — Credential Abuse

Within minutes:

- Impossible travel alerts appear
- Failed MFA attempts occur
- A successful cloud login is detected from an unusual geography

The attacker begins accessing email and collaboration platforms.

---

## Phase 3 — Persistence & Reconnaissance

The attacker:

- Creates suspicious inbox forwarding rules
- Enumerates user accounts
- Accesses shared file repositories
- Attempts privilege escalation

---

## Phase 4 — Lateral Movement

Additional indicators appear:

- Remote PowerShell activity
- SMB share enumeration
- Authentication attempts against internal systems
- Endpoint detection alerts for suspicious command execution

---

## Phase 5 — Data Exfiltration Attempt

Potential indicators include:

- Large outbound file transfers
- Archive file creation
- Unusual cloud storage uploads
- Suspicious encrypted traffic

---

# Exercise Timeline

| Time | Inject | Expected Team Action |
|---|---|---|
| T+0 | Employee reports suspicious email | Triage and collect indicators |
| T+15 | Multiple failed MFA alerts appear | Investigate account compromise |
| T+30 | Successful login from unusual location | Validate impossible travel activity |
| T+45 | Suspicious mailbox forwarding rule created | Investigate persistence activity |
| T+60 | Endpoint alert for PowerShell execution | Begin endpoint investigation |
| T+90 | Multiple failed authentication attempts | Assess lateral movement |
| T+120 | Potential data exfiltration alert | Escalate incident severity |
| T+150 | Executive leadership requests status update | Provide operational briefing |

---

# Technical Injects

## Inject 1 — Phishing Email

### Simulated Indicators

- Suspicious sender domain
- External login portal
- Credential harvesting page
- Employee-reported phishing message

### Blue Team Considerations

- What evidence should be collected?
- How should the email be analyzed?
- Should enterprise blocking occur immediately?

---

## Inject 2 — Identity Compromise

### Simulated Indicators

- Impossible travel alert
- MFA fatigue attempts
- New sign-in location
- User-agent anomalies

### Blue Team Considerations

- What log sources should be reviewed?
- Should the account be disabled immediately?
- What additional accounts may be affected?

---

## Inject 3 — Endpoint Activity

### Simulated Indicators

- PowerShell execution
- Encoded command activity
- Registry persistence
- Endpoint telemetry alerts

### Blue Team Considerations

- What endpoint evidence is required?
- How should containment occur?
- What systems should be isolated?

---

## Inject 4 — Data Exfiltration

### Simulated Indicators

- Unusual outbound traffic
- Archive creation
- Cloud upload activity
- Large file transfers

### Blue Team Considerations

- Has sensitive data been accessed?
- What legal or regulatory obligations exist?
- When should executives or regulators be informed?

---

# Blue Team Discussion Questions

## Detection & Analysis

1. Which alerts would you prioritize first?
2. What evidence is needed before declaring an incident?
3. What tools or telemetry sources would you review?
4. How do you validate whether activity is malicious?

---

## Containment

1. When should accounts be disabled?
2. Should endpoints be isolated immediately?
3. What risks exist if containment is delayed?
4. How do you preserve forensic evidence while containing threats?

---

## Escalation & Communications

1. When should leadership be informed?
2. What information should be included in executive briefings?
3. When should Legal, Privacy, Fraud, or Compliance be engaged?
4. How should customer impact be assessed?

---

## Recovery

1. How should affected systems be restored?
2. What validation is required before returning systems to production?
3. What lessons learned should be documented?
4. What preventive controls should be improved afterward?

---

# Expected Detection Opportunities

| Security Control | Expected Detection |
|---|---|
| Email Security Gateway | Phishing detection |
| Identity Protection Platform | Impossible travel / MFA anomalies |
| SIEM | Correlation of authentication anomalies |
| Endpoint Detection & Response (EDR) | PowerShell and persistence activity |
| Network Monitoring | Data exfiltration indicators |
| Cloud Security Monitoring | Suspicious cloud access patterns |
| Threat Intelligence | IOC correlation |

---

# MITRE ATT&CK Mapping

| ATT&CK Tactic | Technique |
|---|---|
| Initial Access | Phishing |
| Credential Access | Credential Harvesting |
| Persistence | Mailbox Rule Creation |
| Discovery | Account Enumeration |
| Lateral Movement | Remote Services |
| Command and Control | Encrypted Channel |
| Exfiltration | Exfiltration Over Web Services |

---

# NIST & CRI Framework Mapping

---

## NIST Cybersecurity Framework (CSF)

| NIST Function | Alignment |
|---|---|
| Identify | Threat identification and risk analysis |
| Protect | Awareness and access control validation |
| Detect | Monitoring, alerting, and telemetry analysis |
| Respond | Incident response coordination and communications |
| Recover | Recovery planning and operational restoration |

---

## NIST SP 800-53 Mapping

| Control | Description |
|---|---|
| IR-2 | Incident Response Training |
| IR-3 | Incident Response Testing |
| IR-4 | Incident Handling |
| IR-5 | Incident Monitoring |
| IR-8 | Incident Response Plan |
| SI-4 | System Monitoring |
| AU-6 | Audit Review and Analysis |
| CA-7 | Continuous Monitoring |

---

## Cyber Risk Institute (CRI) Mapping

| CRI Domain | Exercise Alignment |
|---|---|
| Cybersecurity Incident Management | Validates escalation and response coordination |
| Situational Awareness | Reinforces detection and operational visibility |
| Cybersecurity Controls | Tests detective and preventive control effectiveness |
| Cyber Risk Management & Oversight | Supports governance and reporting maturity |
| Incident Resilience & Recovery | Exercises operational resilience and restoration |

---

# Scoring and Evaluation

## Maturity Scale

| Score | Rating | Description |
|---|---|---|
| 5 | Optimized | Rapid, coordinated, and mature response |
| 4 | Managed | Effective response with minor gaps |
| 3 | Defined | Repeatable but inconsistent execution |
| 2 | Developing | Informal or partially effective response |
| 1 | Initial | Significant operational weaknesses |

---

## Evaluation Categories

| Category | Evaluation Focus |
|---|---|
| Detection | Speed and accuracy of identification |
| Analysis | Quality of investigation and evidence handling |
| Escalation | Appropriate incident declaration and communications |
| Containment | Timeliness and effectiveness of response actions |
| Coordination | Cross-team collaboration |
| Recovery | Restoration and validation processes |
| Documentation | Accuracy of notes, timelines, and findings |
| Lessons Learned | Identification of remediation opportunities |

---

# Sample Findings

| Finding | Risk Level | Recommendation |
|---|---|---|
| Analysts delayed escalation awaiting additional evidence | High | Define escalation thresholds more clearly |
| EDR alerts were not correlated with identity alerts | Medium | Improve SIEM correlation rules |
| Executive communications lacked consistency | Medium | Develop executive cyber incident templates |
| Endpoint isolation procedures worked effectively | Low | Document as operational strength |

---

# After-Action Review

Each exercise should produce:

- Executive summary
- Technical findings
- Timeline of events
- Investigation observations
- Escalation analysis
- Detection gaps
- Recommended control improvements
- Assigned remediation owners
- Completion timelines

---

# Strategic Value

This exercise demonstrates operational cyber defense maturity by validating:

- SOC readiness
- Incident response effectiveness
- Threat detection capability
- Blue Team coordination
- Security monitoring processes
- Executive reporting readiness
- Financial sector cyber resilience

The exercise also provides measurable evidence for:

- Internal Audit
- Regulatory reviews
- NIST maturity assessments
- CRI profile alignment
- FFIEC examinations
- Security operations program maturity

---
# Blue Team Incident Response Tabletop Exercise

A realistic multi-stage cyberattack scenario designed for SOC analysts, incident responders, and Blue Team personnel within a financial institution environment. Includes MITRE ATT&CK mapping, NIST/CRI alignment, scoring models, technical injects, and after-action reporting structure.
```
