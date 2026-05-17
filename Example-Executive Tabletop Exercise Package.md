# 🔐 Executive Tabletop Exercise Package
> Financial Institution Cybersecurity Program Portfolio  
> Scenario: Ransomware & Business Operations Disruption

---

# 📑 Table of Contents

- [Exercise Overview](#-exercise-overview)
- [Exercise Objectives](#-exercise-objectives)
- [Scenario Background](#-scenario-background)
- [Scenario Narrative](#-scenario-narrative)
- [Exercise Timeline & Injects](#-exercise-timeline--injects)
- [Participant Roles](#-participant-roles)
- [Evaluation Criteria](#-evaluation-criteria)
- [Example KPIs](#-example-kpis)
- [Lessons Learned Session](#-lessons-learned-session)
- [Post-Exercise Deliverables](#-post-exercise-deliverables)
- [Framework Alignment](#-framework-alignment)
- [Portfolio Purpose](#-portfolio-purpose)

---

# 📌 Exercise Overview

This tabletop exercise package is designed for executive leadership, cyber incident response teams, technology leadership, legal, communications, fraud operations, and business continuity stakeholders within a financial institution environment.

The exercise simulates a coordinated ransomware attack impacting critical banking systems, customer operations, third-party dependencies, and executive crisis-management decision-making.

The scenario is designed to evaluate:

- Executive decision-making
- Incident escalation procedures
- Cross-functional communication
- Business continuity readiness
- Regulatory response coordination
- Third-party risk management
- Media and customer communication strategies
- Human-risk and phishing escalation processes

---

# 🎯 Exercise Objectives

Participants will:

1. Validate incident response escalation procedures  
2. Assess executive crisis-management coordination  
3. Evaluate ransomware containment decision-making  
4. Review customer communication processes  
5. Test business continuity and disaster recovery alignment  
6. Validate regulatory notification workflows  
7. Evaluate fraud-risk escalation handling  
8. Assess third-party dependency management  
9. Review legal and compliance coordination  
10. Validate executive reporting and governance structures  

---

# 🏦 Scenario Background

## Organization Profile

A large regional financial institution with:

- Retail banking operations
- Commercial lending services
- Online banking platform
- Contact center operations
- Hybrid cloud infrastructure
- Third-party payment processing integrations

### Technology Stack

- Microsoft 365
- Entra ID
- Sentinel SIEM
- Endpoint Detection & Response (EDR)
- VPN infrastructure
- Core banking applications

---

# ⚠️ Scenario Narrative

## Day 1 — Initial Compromise

An employee within the finance department receives a phishing email appearing to originate from a trusted vendor.

The email contains:

- Urgent invoice payment request
- Spoofed domain
- Malicious attachment
- Credential harvesting link

The employee opens the attachment and enters credentials into a fake Microsoft 365 login portal.

Within hours:

- Threat actors establish persistence
- MFA fatigue attacks begin
- Multiple failed login attempts occur
- Privileged accounts are targeted

Security monitoring detects:

- Suspicious PowerShell execution
- Lateral movement behavior
- Privilege escalation activity
- Abnormal data access patterns

---

# 🚨 Exercise Timeline & Injects

## Inject 1 — SOC Detection

### 🕒 Time
8:15 AM

### 📌 Information Provided

The SOC identifies:

- Multiple endpoint alerts
- Credential abuse attempts
- Unusual administrative activity
- Indicators of ransomware staging

### 💬 Discussion Questions

- Who is notified first?
- What severity level is assigned?
- Does this trigger executive escalation?
- What systems require immediate containment?
- Are third parties engaged?

### ✅ Expected Actions

- Activate incident response procedures
- Escalate to leadership
- Initiate containment strategy
- Begin evidence preservation

---

## Inject 2 — Business Impact Escalation

### 🕒 Time
10:00 AM

### 📌 Information Provided

Employees report:

- File shares inaccessible
- Customer service ticket spikes
- VPN instability
- Banking application latency

A ransom note appears on multiple systems demanding cryptocurrency payment.

### 💬 Discussion Questions

- Who declares a crisis event?
- Does the institution activate BCP/DR?
- Are systems shut down proactively?
- How is fraud risk assessed?
- What is communicated internally?

### ✅ Expected Actions

- Executive crisis bridge activation
- Technology isolation procedures
- Business continuity activation
- Internal communications release
- Regulatory consultation initiation

---

## Inject 3 — Public & Customer Pressure

### 🕒 Time
12:30 PM

### 📌 Information Provided

Social media posts begin circulating claiming:

- Customer accounts inaccessible
- Fraudulent transactions occurring
- Mobile banking unavailable

Local media contacts corporate communications requesting a statement.

### 💬 Discussion Questions

- Who approves public statements?
- What legal review is required?
- What customer notification thresholds exist?
- How is reputational risk assessed?
- When is executive leadership informed?

### ✅ Expected Actions

- Activate communications response plan
- Coordinate legal/compliance review
- Prepare executive updates
- Draft customer messaging
- Monitor misinformation risks

---

## Inject 4 — Regulatory & Third-Party Escalation

### 🕒 Time
2:00 PM

### 📌 Information Provided

The institution receives:

- Regulator inquiries
- Third-party vendor alerts
- Cyber insurance notification requirements
- Law enforcement outreach

Indicators suggest customer data may have been exfiltrated.

### 💬 Discussion Questions

- What are the breach notification obligations?
- Which regulators require notification?
- How are vendors coordinated?
- Does the organization engage external IR firms?
- How are executives briefed?

### ✅ Expected Actions

- Regulatory notification coordination
- Legal escalation procedures
- Vendor-risk management activation
- External IR engagement
- Executive status reporting cadence

---

## Inject 5 — Recovery & Decision Point

### 🕒 Time
4:30 PM

### 📌 Information Provided

The threat actors:

- Demand payment within 24 hours
- Threaten public data release
- Continue encryption attempts

Backups appear partially affected.

### 💬 Discussion Questions

- Who approves ransom decisions?
- What legal restrictions exist?
- Are backups viable?
- What is the recovery priority?
- How are operational risks balanced?

### ✅ Expected Actions

- Recovery prioritization
- Executive decision documentation
- Legal and regulatory coordination
- Recovery communications strategy
- Post-incident planning

---

# 👥 Participant Roles

| Role | Responsibilities |
|---|---|
| Executive Leadership | Strategic decisions, business impact, governance |
| CISO | Incident oversight, cyber response coordination |
| SOC Team | Detection, containment, investigation |
| Infrastructure Team | Recovery and restoration |
| Legal | Regulatory guidance and legal review |
| Communications | Media and customer messaging |
| Fraud Operations | Fraud monitoring and escalation |
| Risk Management | Enterprise risk coordination |
| HR | Internal employee communications |
| Vendor Management | Third-party coordination |

---

# 📊 Evaluation Criteria

## Governance & Escalation

- Timeliness of escalation
- Leadership engagement effectiveness
- Executive communication cadence
- Documentation quality

## Technical Response

- Containment effectiveness
- Evidence preservation
- Recovery coordination
- Incident prioritization

## Business Operations

- BCP activation efficiency
- Customer-impact management
- Operational resilience
- Fraud mitigation coordination

## Communications

- Internal communications clarity
- Media response coordination
- Customer messaging quality
- Executive briefing effectiveness

## Regulatory Alignment

- Notification timing
- Documentation completeness
- Legal coordination
- Third-party oversight

---

# 📈 Example KPIs

| KPI | Target |
|---|---|
| Executive Escalation Time | < 30 minutes |
| Incident Severity Classification | < 15 minutes |
| Regulatory Notification Readiness | < 4 hours |
| Crisis Bridge Activation | < 20 minutes |
| Customer Communication Drafting | < 2 hours |
| Recovery Prioritization Completion | < 90 minutes |
| Internal Communications Release | < 60 minutes |

---

# 🧩 Lessons Learned Session

At exercise completion, facilitators should conduct a structured lessons-learned review.

## Discussion Areas

- Escalation gaps
- Technology weaknesses
- Communication breakdowns
- Vendor coordination issues
- Regulatory process improvements
- Executive decision bottlenecks
- Human-risk awareness opportunities

---

# 📋 Post-Exercise Deliverables

Recommended follow-up artifacts:

- After Action Report (AAR)
- Gap remediation plan
- Executive summary presentation
- Risk register updates
- Incident response playbook updates
- Awareness and training enhancements
- Third-party review actions

---

# 🛡️ Framework Alignment

This exercise aligns to:

- NIST CSF 2.0
- NIST 800-53
- FFIEC CAT
- Cyber Risk Institute (CRI) Profile
- ISO 27001
- PCI DSS
- GLBA Safeguards Rule
- SEC Cybersecurity Disclosure Guidance

---

# 📂 Portfolio Purpose

This tabletop exercise package demonstrates:

- Executive cybersecurity governance
- Incident response coordination
- Human-risk operational maturity
- Threat-informed awareness strategy
- Enterprise crisis management integration
- Financial-sector operational resilience
- Executive decision-making readiness
- Regulatory escalation preparedness

---
