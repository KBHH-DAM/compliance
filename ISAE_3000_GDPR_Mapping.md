# ISAE 3000 Type 1 Controls → GDPR Cyberday Mapping

**Prepared for:** Elumi  
**Framework:** ISAE 3000 Type 1 Audit for GDPR Compliance  
**Primary Reference:** General Data Protection Regulation (GDPR)  
**Supporting Framework:** SOC 2, ISO 27001, ISO 27701  
**Date:** 2026-10-02

---

## Overview: ISAE 3000 Audit Scope

ISAE 3000 is the assurance standard used to audit **GDPR compliance** for data processors. This mapping connects each ISAE 3000 control to the specific **GDPR Articles** that define the requirements being assessed.

**GDPR Cyberday Coverage:**
- **42 total requirements** mapped across 5 sections
- **Controller and Processor Obligations** (Art 24-39): 16 requirements
- **Data Subject Rights** (Art 12-23): 12 requirements  
- **Principles** (Art 5-11): 7 requirements
- **Third-Country Transfers** (Art 44-49): 6 requirements
- **Penalties** (Art 83): 1 requirement

---

## A – Controller Instructions

### A.1 Processing Instructions & Procedure Review
**ISAE Requirement:** Written procedures requiring documented controller instructions; annual assessments

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 1: Processing only on instructions from controller
  - Para 3(a): Documented instructions required
  - Para 3(b): Ensure processor doesn't process for own purposes
- **Art 5 - Principles** (Principles)
  - Para 2(d): Accountability principle (maintain records of instructions)

**Secondary References:**
- SOC 2: CC3.1, CC5.3, CC7.1 (objectives, policies, configuration changes)
- ISO 27001: A.5.1 (policies for information security)
- ISO 27701: A.2.2 (controller-processor relationship)

**Evidence to Gather:**
- Documented controller instruction procedures
- Records of annual review of instructions
- Evidence of compliance with Art 28(3)(a) written instructions requirement
- Processing instructions registry/register

---

### A.2 Compliance with Processing Agreements
**ISAE Requirement:** Data processor only processes per controller instructions; DPA alignment

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 1: Processing only on documented instructions
  - Para 3: Content of data processing agreement
- **Art 5 - Principles** (Principles)
  - Para 1(a): Lawfulness, fairness, transparency
  - Para 2(a): Accountability in processing activities
- **Art 6 - Lawfulness of processing** (Principles)
  - Instructions must be lawful

**Secondary References:**
- SOC 2: P5.1 (consistency of processing with objectives), CC2.1 (quality of information)
- ISO 27001: A.5.1 (policy documentation)

**Evidence to Gather:**
- Processing activities register (mapped to DPA instructions)
- Sample data processing agreements
- Activity/processing logs showing instruction compliance
- Records demonstrating lawful processing basis

---

### A.3 Reporting Potentially Unlawful Instructions
**ISAE Requirement:** Data processor assesses and reports instructions violating GDPR/EU law to controller

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Implied in processor obligation to ensure lawful processing
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1: Processor responsible for security measures
  - Para 1(b): Ensuring only authorized access
- **Art 33 - Notification of breach** (Controller and processor)
  - Processor responsibility to notify controller

**Secondary References:**
- SOC 2: CC3.3 (fraud consideration), CC2.3 (external communication)
- ISO 27701: A.2.2 (processor obligations)
- NIS2 Directive: Incident escalation procedures

**Evidence to Gather:**
- Procedure for assessing lawfulness of instructions
- Case records of unlawful instructions (if any) with controller notifications
- Confirmation of zero unlawful cases (if none occurred)
- Escalation procedure documentation

---

## B – Technical and Physical Security Measures

### B.1 Safeguards Implementation & Review
**ISAE Requirement:** Written procedures for implementing agreed safeguards; annual assessments

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1: Technical and organizational measures required
  - Para 2: Processor implements measures appropriate to risk
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(c): Agreement on security measures
- **Art 30 - Records of processing activities** (Controller and processor)
  - Document security measures implemented

**Secondary References:**
- SOC 2: CC5.1, CC6.1c, CC4.1 (control activities, asset security, monitoring)
- ISO 27001: A.5, A.12 (organizational and operational controls)
- ISO 27017: A.2.1 (cloud-specific safeguards)

**Evidence to Gather:**
- Security measures implementation procedure (aligned to Art 32)
- Evidence of latest procedure review
- DPA Annex II security requirements
- Implementation evidence (configurations, audit reports, screenshots)

---

### B.2 Risk Assessment & Technical Measures
**ISAE Requirement:** Risk assessment performed; technical measures implemented based on risk assessment

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1: Measures appropriate to the risk
  - Para 2: Basis = risk assessment
- **Art 35 - Data protection impact assessment** (Controller and processor)
  - Risk assessment and evaluation of impacts
  - Required before high-risk processing

**Secondary References:**
- SOC 2: CC3.2, CC5.1, CC5.2 (risk identification, control activities)
- DORA: Risk assessment framework
- NIST CSF 2.0: Identify & Protect functions
- ISO 27001: A.12 (operational controls based on risk)

**Evidence to Gather:**
- Latest dated risk assessment (per Art 32)
- Risk assessment methodology documentation
- Risk approval by management
- Evidence of technical measures implementation
- DPA security requirements and mapping to risk assessment

---

### B.3 Antivirus Protection & Updates
**ISAE Requirement:** Antivirus software installed and regularly updated on systems processing personal data

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(a): Pseudonymization and encryption
  - Para 1(b): Ability to restore availability and access
  - Para 2: Measures appropriate to risk
- **Art 28 - Data processor** (Controller and processor)
  - Processor ensures appropriate security level

**Secondary References:**
- SOC 2: CC6.1c, CC7.2 (technical security, system monitoring)
- CIS 18 Controls: Control 10 (malware defenses)
- ISO 27001: A.12.2 (malware protection)
- NIST CSF 2.0: Detect function

**Evidence to Gather:**
- Inventory of systems processing personal data
- Antivirus/endpoint protection coverage report
- Patch update status (last 90 days)
- Update schedule or automated update evidence

---

### B.4 Firewall Protection for External Access
**ISAE Requirement:** External access to systems protected through secured firewall

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(a): Encryption and pseudonymization
  - Para 1(b): Ability to ensure ongoing confidentiality, integrity, availability
  - Para 2: Appropriate to risk and nature of personal data
- **Art 28 - Data processor** (Controller and processor)
  - Ensure security measures in place

**Secondary References:**
- SOC 2: CC6.2, CC7.1 (logical access, configuration management)
- CIS 18 Controls: Control 1 (asset inventory)
- ISO 27001: A.13.1 (network security)
- NIST CSF 2.0: Protect function

**Evidence to Gather:**
- Network diagram showing external access routes and firewall placement
- Current firewall configuration/rules export
- Firewall configuration standard/policy
- Evidence of firewall maintenance and updates

---

### B.5 Network Segmentation
**ISAE Requirement:** Internal networks segmented to restrict access to systems processing personal data

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(b): Ability to ensure ongoing confidentiality and integrity
  - Para 2: Appropriate to risk
- **Art 5 - Principles** (Principles)
  - Para 1(f): Integrity and confidentiality

**Secondary References:**
- SOC 2: CC6.1a, CC6.2b (asset identification, logical access)
- CIS 18 Controls: Control 1, 3 (asset management, network architecture)
- ISO 27001: A.13.1 (network segregation)
- NIST CSF 2.0: Protect function

**Evidence to Gather:**
- Network segmentation diagram
- VLAN/firewall configuration showing restricted access
- List of permitted inter-segment connections
- Evidence of segment maintenance/review

---

### B.6 Access Control for Personal Data
**ISAE Requirement:** Access to personal data limited to users with work-related need; periodic review

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(b): Ability to ensure confidentiality and integrity
  - Para 2: Appropriate to risk and nature of processing
- **Art 28 - Data processor** (Controller and processor)
  - Ensure only authorized persons access personal data
- **Art 5 - Principles** (Principles)
  - Para 1(f): Integrity and confidentiality principle
  - Para 2(a): Accountability (demonstrate compliance)

**Secondary References:**
- SOC 2: CC6.2 (prior to issuing credentials, periodic review)
- ISO 27001: A.9 (access control)
- ISO 27701: A.3.1 (data processing limitation)

**Evidence to Gather:**
- Access control procedure with authorization process
- Access approval requirements and business justification documentation
- Current user access listing for systems with personal data
- Sample access approvals with business justifications
- Latest periodic access review records with change management
- Deactivation records for employees with access

---

### B.7 System Monitoring & Alerts
**ISAE Requirement:** System monitoring established with alarm features; investigation and escalation

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(c): Ability to restore availability (implies incident detection)
  - Para 1(g): Regular testing of measures
  - Para 2: Appropriate to risk
- **Art 33 - Notification of breach** (Controller and processor)
  - Processor must detect and notify controller of breaches
- **Art 28 - Data processor** (Controller and processor)
  - Processor ensures security measures in place
- **Art 30 - Records of processing activities** (Controller and processor)
  - Document security measures (including monitoring)

**Secondary References:**
- SOC 2: CC7.2, CC7.3, CC7.4 (monitoring, security events evaluation)
- CIS 18 Controls: Control 8 (audit logging)
- ISO 27001: A.12.4 (event logging and monitoring)
- NIST CSF 2.0: Detect function

**Evidence to Gather:**
- Monitoring configuration and alert overview for systems with personal data
- Alert rules and thresholds
- Investigation procedure for detected events
- Sample investigation records (3 selected alerts)
- Controller notification records (if applicable)

---

### B.8 Encryption for Internet/Email Transfers
**ISAE Requirement:** Effective encryption applied when transmitting sensitive/confidential personal data

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(a): Encryption of personal data
  - Para 1(b): Ability to ensure ongoing confidentiality
  - Para 2: Measures appropriate to risk and nature of data
- **Art 5 - Principles** (Principles)
  - Para 1(f): Integrity and confidentiality

**Secondary References:**
- SOC 2: CC6.1c, C1.2 (technical security, confidentiality protection)
- ISO 27001: A.10.1 (cryptography)
- ISO 27017: Cloud-specific encryption controls

**Evidence to Gather:**
- Procedure/user guidance for encrypted transfers
- Configuration or screenshots of encryption technologies used
- Redacted transfer example showing encryption
- Overview of any unencrypted transfers (or confirmation none exist)
- Encryption standard documentation

---

### B.9 Logging of User & Security Events
**ISAE Requirement:** Logging of admin activities, security incidents, changes to logging, rights changes, failed logins

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(g): Regular testing of measures (implies ongoing monitoring/logging)
  - Para 2: Appropriate to risk and processing type
- **Art 33 - Notification of breach** (Controller and processor)
  - Requires detection capability (logs support detection)
- **Art 28 - Data processor** (Controller and processor)
  - Document and maintain security measures
- **Art 30 - Records of processing activities** (Controller and processor)
  - Records of security measures

**Secondary References:**
- SOC 2: CC7.2, CC7.3, CC6.2c (monitoring, event evaluation, privileged access)
- CIS 18 Controls: Control 8 (audit logging)
- ISO 27001: A.12.4 (event logging, monitoring, protected logs)
- NIST CSF 2.0: Detect function

**Evidence to Gather:**
- Logging standard/policy covering:
  - Privileged user activities
  - Security event logging
  - Changes to logging configuration
  - Changes to user rights
  - Failed login attempts
- Current logging configuration for systems with personal data
- Representative redacted log extracts
- Log protection and retention settings documentation

---

### B.10 Pseudonymization/Anonymization in Dev/Test
**ISAE Requirement:** Personal data in development/testing pseudonymized/anonymized or under documented controller agreement

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(a): Pseudonymization of personal data
  - Para 2: Appropriate to risk
- **Art 25 - Data protection by design and by default** (Controller and processor)
  - Implement technical and organizational measures (including pseudonymization)
  - Minimize personal data processing
- **Art 5 - Principles** (Principles)
  - Para 1(c): Data minimization
  - Para 1(e): Storage limitation
  - Para 1(f): Integrity and confidentiality

**Secondary References:**
- SOC 2: PI1.2 (system inputs)
- ISO 27701: Data minimization, pseudonymization
- ISO 27001: A.5 (organizational controls on data handling)

**Evidence to Gather:**
- Procedure for using personal data in development/testing environments
- Inventory of development and test databases
- Data extracts/configuration evidence for 3 selected databases showing:
  - Pseudonymization mechanism OR anonymization proof
  - Data minimization practices
- If identifiable data used: documented controller agreement/instruction
  - For 3 databases: DPA/instructions and approval evidence

---

### B.11 Vulnerability Scans & Penetration Testing
**ISAE Requirement:** Technical measures tested regularly through vulnerability scans and pen tests; weaknesses addressed

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(g): Regular testing of measures
  - Para 2: Appropriate to risk and nature of processing
- **Art 25 - Data protection by design and by default** (Controller and processor)
  - Implement technical measures (includes testing/validation)
- **Art 28 - Data processor** (Controller and processor)
  - Ensure appropriate security level

**Secondary References:**
- SOC 2: CC4.1, CC7.2 (control evaluation, system monitoring)
- CIS 18 Controls: Control 5 (vulnerability management)
- ISO 27001: A.14.2 (vulnerability management)
- NIST CSF 2.0: Identify, Detect functions

**Evidence to Gather:**
- Testing schedule (documented)
- Latest vulnerability scan report:
  - Scope defined
  - Date performed
  - Internal or external testing noted
  - Findings documented
- Latest penetration test report (same documentation)
- Finding tracker/remediation log
- Recent remediation or risk acceptance record
- Controller communication (if relevant findings found)

---

### B.12 Change & Patch Management
**ISAE Requirement:** System changes and patches controlled per procedure; includes security patches

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1: Ongoing security measures
  - Para 1(g): Regular testing (implies ongoing updates/changes)
  - Para 2: Appropriate to risk
- **Art 25 - Data protection by design and by default** (Controller and processor)
  - Implement technical measures
  - Keep measures up to date
- **Art 28 - Data processor** (Controller and processor)
  - Maintain security measures

**Secondary References:**
- SOC 2: CC8.1, CC7.1 (change management, configuration changes)
- CIS 18 Controls: Control 6 (asset management)
- ISO 27001: A.14.1 (information security change management)
- NIST CSF 2.0: Protect function

**Evidence to Gather:**
- Documented change and patch management procedure
- Current patch-status report showing:
  - Systems with personal data
  - Patch application status
  - Critical/security patch coverage
- Selected approved change tickets or deployment records
- Evidence of patch testing before deployment
- Patch schedule/automation evidence

---

### B.13 User Access Management & Periodic Review
**ISAE Requirement:** Formalized procedure for granting/removing access; regular review with business need justification

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(b): Ability to ensure confidentiality and integrity
  - Para 2: Appropriate to risk
  - Ongoing management of access rights
- **Art 28 - Data processor** (Controller and processor)
  - Ensure only authorized persons access personal data
- **Art 5 - Principles** (Principles)
  - Para 1(f): Integrity and confidentiality
  - Para 2(a): Accountability (demonstrate compliance)

**Secondary References:**
- SOC 2: CC6.2, CC4.1, CC7.3 (access credentials, control evaluation, event removal)
- ISO 27001: A.9.2 (user access management)
- ISO 27701: A.3.1 (data processing limitation)

**Evidence to Gather:**
- Access management procedure covering:
  - Access authorization process
  - Periodic review requirements
  - Offboarding/deactivation
- Current user access listing for systems with personal data
- For 3 selected employees:
  - Access request/approval records
  - Business justification for access grant
  - Current assigned privileges
- Latest periodic access review (documented):
  - Review date
  - Participants
  - Results/changes made
- Employee departure/deactivation records (if applicable)

---

### B.14 Two-Factor Authentication for High-Risk Processing
**ISAE Requirement:** Two-factor authentication required and active for high-risk systems/accounts

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(b): Ability to ensure confidentiality and integrity
  - Para 2: Measures appropriate to risk (high-risk = stronger MFA)
- **Art 5 - Principles** (Principles)
  - Para 1(f): Integrity and confidentiality
- **Art 25 - Data protection by design** (Controller and processor)
  - Implement technical measures appropriate to risk

**Secondary References:**
- SOC 2: CC6.2, CC6.1c (multi-factor authentication for sensitive access)
- CIS 18 Controls: Control 2 (access control, MFA)
- ISO 27001: A.9.4 (privileged access rights)
- NIST CSF 2.0: Protect function

**Evidence to Gather:**
- Risk assessment identifying high-risk systems/accounts for personal data
- Procedure/policy requiring MFA for high-risk access
- System settings or screenshots showing MFA enforcement
- Configuration evidence for critical systems
- VPN/remote access guidance (if applicable)

---

### B.15 Physical Access Safeguards
**ISAE Requirement:** Physical access controls restrict access to authorized persons only at premises/data centers with personal data

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1: Physical and technical measures
  - Para 1(b): Ability to ensure ongoing confidentiality and integrity
  - Para 2: Appropriate to risk and nature of processing
- **Art 5 - Principles** (Principles)
  - Para 1(f): Integrity and confidentiality
- **Art 28 - Data processor** (Controller and processor)
  - Ensure appropriate security level

**Secondary References:**
- SOC 2: CC6.1a, CC6.3 (asset identification, physical access)
- CIS 18 Controls: Control 1 (physical asset management)
- ISO 27001: A.11.1 (physical security perimeter)
- NIST CSF 2.0: Protect function

**Evidence to Gather:**
- Physical access procedure covering:
  - Badge/key issuance
  - Access authorization
  - Deactivation on departure
- Current list of authorized persons
- Latest access review (date, results)
- Selected access record (audit trail)
- Third-party facility control report (if data center is outsourced)
- Visitor policy/log (if applicable)

---

## C – Organisational Measures

### C.1 Information Security Policy & Management Approval
**ISAE Requirement:** Written information security policy approved by management, communicated to stakeholders, based on risk assessment; annual review

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 2: Appropriate security measures based on risk
- **Art 25 - Data protection by design and by default** (Controller and processor)
  - Implement technical and organizational measures
  - Document security measures
- **Art 28 - Data processor** (Controller and processor)
  - Para 3: Data processing agreement must specify security measures
- **Art 30 - Records of processing activities** (Controller and processor)
  - Document security measures implemented

**Secondary References:**
- SOC 2: CC1.1, CC2.2, CC3.2 (management commitment, communication, risk-based)
- ISO 27001: A.5.1 (information security policies)
- ISO 27701: Policy development for privacy controls

**Evidence to Gather:**
- Current information security policy covering:
  - GDPR compliance requirements
  - Security measures and controls
  - Data processor responsibilities
- Dated management approval/review (within past 12 months)
- Evidence of communication to staff:
  - Intranet screenshot
  - Distribution record
  - Acknowledgment log
- Policy aligned to risk assessment

---

### C.2 Policy Compliance with Data Processing Agreements
**ISAE Requirement:** Management verifies policy doesn't conflict with DPAs; policy covers security commitments in contracts

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(c): Agreement must specify technical and organizational measures
  - Para 4: Processor remains bound by GDPR even after contract ends
- **Art 32 - Security of processing** (Controller and processor)
  - Measures must align with controller agreements
- **Art 5 - Principles** (Principles)
  - Para 2(a): Accountability (demonstrate alignment)

**Secondary References:**
- SOC 2: CC2.1, CC5.2 (quality of information, control activities)
- ISO 27001: A.5.1 (policy integration)
- ISO 27701: A.2.2 (controller-processor agreement alignment)

**Evidence to Gather:**
- Management assessment/mapping document showing:
  - Policy requirements
  - DPA security clauses
  - Alignment evidence
- For 3 selected DPAs:
  - Security clauses/Annex II
  - Evidence policy addresses each clause
  - Documentation of any gaps resolved
- Approval by management

---

### C.3 Employee Screening During Recruitment
**ISAE Requirement:** Employees screened per procedure during recruitment; includes references, criminal records, diplomas per DPA requirements

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(c): Processor must ensure security level including personnel selection
  - Para 4: Processor bound by GDPR confidentiality
  - Implied: Personnel must be suitable/vetted
- **Art 5 - Principles** (Principles)
  - Para 2(a): Accountability (demonstrate suitable personnel)
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1: Organizational measures including personnel selection

**Secondary References:**
- SOC 2: CC1.2, CC1.3 (board oversight, established responsibilities)
- ISO 27001: A.6.1 (personnel screening)
- ISO 27701: A.2.1 (employee selection and confidentiality)

**Evidence to Gather:**
- Employee screening procedure covering:
  - References checks
  - Criminal record verification (as required)
  - Qualifications/diplomas
- Overview of DPA screening requirements
- For 3 DPAs: mapping showing how procedure addresses requirements
- For 3 selected employees:
  - Redacted screening checklist
  - Date of screening
  - Outcome (passed/reference verified)
- If < 3 hires: all available with count noted

---

### C.4 Employee Confidentiality & Information Security Induction
**ISAE Requirement:** Employees sign confidentiality agreements; receive induction on information security policy and data processing procedures

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 3: Persons must be bound by confidentiality
  - Para 4: Processor bound by GDPR confidentiality obligations
  - Persons authorized must understand GDPR
- **Art 29 - Processing under authority** (Controller and processor)
  - Persons authorized to process must commit to confidentiality
- **Art 5 - Principles** (Principles)
  - Para 1(f): Integrity and confidentiality
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(c): Ability to restore confidentiality and integrity

**Secondary References:**
- SOC 2: CC1.1, CC2.2 (management commitment, staff communication)
- ISO 27001: A.6.2 (information security awareness and training)
- ISO 27701: A.2.1 (employee confidentiality and awareness)

**Evidence to Gather:**
- Onboarding/induction procedure covering:
  - Confidentiality agreement requirement
  - Information security policy review
  - GDPR and data processing procedures
- List of employees appointed
- For 3 new hires:
  - Signed confidentiality agreement
  - Dated induction record with evidence of:
    - Policy acknowledgment
    - GDPR briefing
    - Processing procedures review
- If < 3 hires: all available with count noted

---

### C.5 Employee Offboarding: Access Removal & Asset Return
**ISAE Requirement:** Formalized process to ensure access deactivated/terminated upon departure; assets returned

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(g): Confidentiality obligations extend to termination
  - Implied: Access must be removed to maintain confidentiality
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(b): Ability to ensure confidentiality and integrity
  - Para 2: Measures appropriate to risk
  - Requires removal of access on departure
- **Art 5 - Principles** (Principles)
  - Para 1(f): Confidentiality throughout employment and after

**Secondary References:**
- SOC 2: CC6.2, CC6.2c (access removal upon termination)
- ISO 27001: A.6.3 (return of assets)
- ISO 27701: A.2.1 (termination procedures)

**Evidence to Gather:**
- Offboarding procedure covering:
  - Access deactivation
  - System credential removal
  - Asset return process
  - Timeline for completion
- List of employees who departed
- For recent departing employee(s):
  - Completed offboarding checklist
  - Access deactivation ticket with date
  - Asset return confirmation (if applicable)

---

### C.6 Continuation of Confidentiality Obligations Post-Departure
**ISAE Requirement:** Departing employees reminded confidentiality obligations continue after departure

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(g): Confidentiality obligations after termination
  - Para 4: Processor remains bound by confidentiality after contract ends
  - Persons must understand ongoing obligations
- **Art 29 - Processing under authority** (Controller and processor)
  - Authorization continues to bind persons after departure
- **Art 5 - Principles** (Principles)
  - Para 1(f): Confidentiality obligation is perpetual

**Secondary References:**
- SOC 2: CC1.1, CC2.3 (commitment, external communication)
- ISO 27001: A.6.2 (ongoing awareness)
- ISO 27701: A.2.1 (continuing confidentiality)

**Evidence to Gather:**
- Standard departure notice/exit interview documentation
- Offboarding instruction covering continuing confidentiality
- For recent departing employee:
  - Signed confidentiality agreement (original)
  - Dated reminder/acknowledgment of ongoing obligation

---

### C.7 Security Awareness Training
**ISAE Requirement:** Regular security awareness training provided to employees on IT security and data processing security

**Primary GDPR References (Cyberday):**
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(c): Ongoing confidentiality, integrity, availability
  - Para 2: Measures appropriate to risk include personnel awareness
  - Implied: Staff must understand security requirements
- **Art 28 - Data processor** (Controller and processor)
  - Para 3: Ensure appropriate security level
  - Personnel must understand data processing obligations
- **Art 5 - Principles** (Principles)
  - Para 1(f): Confidentiality - requires staff awareness
  - Para 2(a): Accountability (demonstrate staff competence)

**Secondary References:**
- SOC 2: CC1.1, CC2.2, PI2.2 (management commitment, staff communication, privacy training)
- ISO 27001: A.6.2 (information security awareness and training)
- CIS 18 Controls: Control 17 (security awareness and training)
- NIST CSF 2.0: Govern function

**Evidence to Gather:**
- Latest training material/curriculum covering:
  - General IT security
  - GDPR requirements
  - Personal data protection obligations
  - Date of material
- Attendance/completion records for staff with personal data access:
  - Names of attendees
  - Dates of training
  - Topic coverage
- Follow-up records for employees with missing training:
  - Rescheduled training dates
  - Completion records

---

## D – Return and Deletion of Personal Data

### D.1 Storage & Deletion Procedures & Annual Review
**ISAE Requirement:** Written procedures for storing and deleting personal data per controller agreement; annual review

**Primary GDPR References (Cyberday):**
- **Art 5 - Principles** (Principles)
  - Para 1(e): Storage limitation (only store as long as necessary)
  - Para 2(a): Accountability (document retention/deletion policy)
- **Art 17 - Right to erasure** (Data subject rights)
  - Para 3: Processor must delete data upon controller request
  - Implies: Deletion procedures required
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(g): Delete or return data after processing ends
  - Para 3(e): Assist controller with deletion obligations
- **Art 30 - Records of processing activities** (Controller and processor)
  - Document deletion procedures and schedules

**Secondary References:**
- SOC 2: D1.1, D2.2 (data objectives, retention)
- ISO 27701: Data retention and deletion controls
- ISO 27001: A.8.3 (retention of information)

**Evidence to Gather:**
- Current storage and deletion procedure covering:
  - Storage location and duration
  - Retention periods by data category
  - Deletion process and triggers
  - Compliance with Art 5(1)(e)
- Dated record of latest procedure review/update
- Evidence of alignment with controller instructions
- Evidence of implementation

---

### D.2 Retention Periods & Deletion Routines per Agreement
**ISAE Requirement:** Retention periods and deletion routines defined in agreement; verified compliance for 2+ processing activities

**Primary GDPR References (Cyberday):**
- **Art 5 - Principles** (Principles)
  - Para 1(e): Storage limitation (only necessary duration)
  - Para 2(a): Accountability (demonstrate compliance)
- **Art 17 - Right to erasure** (Data subject rights)
  - Para 3: Processor must delete upon request per agreement
  - Processor must have deletion capability
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(g): Deletion or return after processing
  - Agreement must specify retention periods
- **Art 6 - Lawfulness of processing** (Principles)
  - Retention period must align with lawful basis

**Secondary References:**
- SOC 2: D2.1, D2.2 (retention per objectives)
- ISO 27701: Retention and deletion controls
- NIST CSF 2.0: Govern function (data lifecycle)

**Evidence to Gather:**
- Controller instructions or DPA specifying:
  - Retention periods by data category
  - Deletion triggers
  - Lawful basis for retention
- Retention schedule document
- Deletion procedure
- For 2 selected processing activities:
  - System/database configuration showing storage period
  - Evidence data is not retained beyond agreed period
  - Records/reports of storage status
- For 2 selected processing activities:
  - Deletion logs/tickets showing completed deletion
  - Dates of deletion aligned to retention policy
  - Evidence of permanent deletion
- If < 2 available: all with count noted

---

### D.3 Return or Deletion Upon Termination
**ISAE Requirement:** Data returned to controller and/or deleted per agreement upon processing termination; no unlawful retention

**Primary GDPR References (Cyberday):**
- **Art 17 - Right to erasure** (Data subject rights)
  - Para 3: Processor must delete data
  - Controller can request erasure
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(g): **Key requirement**: Upon termination of services:
    - Return personal data to controller, OR
    - Delete personal data (unless EU/member state law requires retention)
- **Art 5 - Principles** (Principles)
  - Para 1(e): Storage limitation (no retention after purpose ends)
  - Para 2(a): Accountability (document termination procedures)

**Secondary References:**
- SOC 2: D2.3 (removal of personal data)
- ISO 27701: Data return and destruction
- ISO 27001: A.8.3 (retention and disposal)

**Evidence to Gather:**
- Termination procedure covering:
  - Trigger events (contract end, data subject request)
  - Return process (delivery to controller)
  - Deletion process (confirmed destruction)
  - Lawful retention exceptions (if any)
  - Timeline for completion
- Most recent terminated arrangement:
  - Related contract/DPA
  - Termination date
  - Return receipt OR deletion record
  - Evidence of lawful retention (if retained)
- If no arrangements terminated: written confirmation

---

## E – Storage and Processing Locations

### E.1 Storage & Processing Procedure Aligned with DPA
**ISAE Requirement:** Written procedure requiring personal data stored per controller agreement; annual review; compliance verified for 3 activities

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(c): DPA must specify location and type of processing
  - Processor must only process per instructions
  - Location is part of controller's instructions
- **Art 5 - Principles** (Principles)
  - Para 1(a): Lawfulness (storage location per contract)
  - Para 2(a): Accountability (document storage location)
- **Art 30 - Records of processing activities** (Controller and processor)
  - Document processing locations
- **Art 32 - Security of processing** (Controller and processor)
  - Para 2: Security measures appropriate to location/risk

**Secondary References:**
- SOC 2: D2.2, CC2.1 (processing consistency, information quality)
- ISO 27017: Cloud region and jurisdiction controls
- ISO 27001: A.8.1 (on-site and off-site storage)

**Evidence to Gather:**
- Storage and processing procedure covering:
  - Approved storage locations
  - Compliance with DPA requirements
  - Data residency requirements
  - Cloud vs on-premise
- Dated evidence of latest procedure review
- Overview of processing activities with locations
- For 3 selected processing activities:
  - Relevant DPA/instructions specifying location
  - System configuration showing actual storage location
  - Data flow documentation showing storage path
  - Cloud region/data center documentation (if applicable)

---

### E.2 Actual Processing/Storage Locations Match Approved Locations
**ISAE Requirement:** Actual processing/storage locations correspond to controller-approved locations; verified for 3 activities

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(c): Processing must follow controller instructions on location
  - Para 1: Processing only per instructions
  - Processor accountable for location compliance
- **Chapter V - Transfers to third countries** (Transfers of personal data)
  - Articles 44-49: If processing in third country, specific safeguards required
- **Art 5 - Principles** (Principles)
  - Para 1(a): Lawfulness (must comply with controller's location requirements)
  - Para 2(a): Accountability (demonstrate location compliance)
- **Art 6 - Lawfulness of processing** (Principles)
  - Location must be lawful (no unauthorized transfers)

**Secondary References:**
- SOC 2: D2.1, CC7.1 (retention per objectives, configuration monitoring)
- ISO 27017: Cloud region controls and compliance
- DORA: Geographical concentration of resources
- ISO 27701: Cross-border transfer controls

**Evidence to Gather:**
- Processing activity register or location inventory showing:
  - Each processing activity
  - Approved storage locations
  - Cloud regions (if applicable)
  - Service providers involved
- For 3 selected processing activities:
  - DPA/controller approval specifying location
  - System configuration showing actual location:
    - Database server location
    - Cloud region (if AWS/Azure/GCP)
    - Data center location
  - Data flow documentation
  - Network configuration showing data routing
- Current evidence of location compliance
  - Screenshots of cloud console (showing region)
  - Service provider certifications (data location)
  - Network diagrams

---

## F – Use of Sub-Processors

### F.1 Sub-Processor Appointment Procedure & Annual Review
**ISAE Requirement:** Written procedures for engaging sub-processors; includes DPA requirements; annual review

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 2: Processor must NOT engage sub-processor without:
    - Prior specific or general authorization from controller
    - Written contract imposing data protection obligations
  - Para 3(e): Agreement must specify authorization conditions
  - Processor accountable for sub-processor compliance
- **Art 30 - Records of processing activities** (Controller and processor)
  - Document sub-processor arrangements
- **Art 5 - Principles** (Principles)
  - Para 2(a): Accountability (document sub-processor governance)

**Secondary References:**
- SOC 2: CC5.3, CC9.2 (policy establishment, partner risk management)
- ISO 27001: A.14.2 (supplier relationships)
- ISO 27701: A.2.2 (sub-processor agreements)
- DORA: Third-party risk management

**Evidence to Gather:**
- Sub-processor appointment procedure covering:
  - Authorization process (specific vs. general)
  - Assessment criteria (security, reliability)
  - Contract/DPA requirements per Art 28(4)
  - Notification to controller per Art 28(2)(h)
  - Objection/change management process
- DPA template for sub-processors ensuring Art 28(4) compliance
- Dated record of latest procedure review/update

---

### F.2 Sub-Processor Authorization & Register
**ISAE Requirement:** Only approved sub-processors used; verified authorizations for 2+ selected

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 2: Only use sub-processors with controller authorization:
    - Specific authorization for named sub-processors OR
    - General authorization for categories
  - Para 3(e): Authorization conditions in DPA
- **Art 30 - Records of processing activities** (Controller and processor)
  - Maintain register of sub-processors
- **Art 5 - Principles** (Principles)
  - Para 2(a): Accountability (maintain authorization records)

**Secondary References:**
- SOC 2: CC9.2, CC5.2 (partner management, authorized activities)
- ISO 27001: A.14.2 (supplier information management)

**Evidence to Gather:**
- Current sub-processor register containing:
  - Sub-processor name
  - Services provided
  - Affected controllers/processing activities
  - Authorization status (specific or general)
  - Date of authorization
- For 2 selected sub-processors:
  - Written DPA or controller approval:
    - Specific authorization (named sub-processor) OR
    - General authorization (category/country)
  - Evidence of controller acceptance/notification
  - Evidence of Art 28(4) obligations in contract
- If < 2 sub-processors used: all available with evidence

---

### F.3 Sub-Processor Change Notification & Approval
**ISAE Requirement:** Controllers notified/asked to approve changes to sub-processors; objection procedures in place

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 2(h): **Key requirement**: Processor must:
    - Inform controller of any intended changes concerning addition/replacement of sub-processor
    - Give controller opportunity to object (if general authorization)
    - Not use sub-processor if controller objects
  - Para 3(e): Conditions for authorization in DPA
- **Art 5 - Principles** (Principles)
  - Para 2(a): Accountability (document notifications)

**Secondary References:**
- SOC 2: CC2.3, CC9.2 (external communication, partner management)
- ISO 27001: A.14.2 (supplier relationship changes)
- ISO 27701: A.2.2 (sub-processor change notification)

**Evidence to Gather:**
- Sub-processor change procedure covering:
  - Process for notifying controller of changes
  - Advance notice period
  - Objection handling process
  - Timeline for implementation
- Log/register of sub-processor changes including:
  - Date of change (addition/removal)
  - Sub-processor name
  - Notification date to controller
  - Objection received? (Y/N)
  - Resolution
- For selected changes:
  - Dated controller notification (email, letter)
  - Objection records (if any) with resolutions
  - Evidence of non-use (if objection sustained)
  - Specific approval (if required per DPA)
- If no changes: written confirmation and documentation of procedure

---

### F.4 Data Protection Obligations Passed to Sub-Processors
**ISAE Requirement:** Sub-processor agreements impose same data protection obligations as in controller DPA; verified for 3+

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 4: **Key requirement**: Sub-processor agreement must:
    - Impose same data protection obligations on sub-processor
    - As are imposed on processor in controller agreement
    - In particular, authorization/instruction and confidentiality
    - Processor remains liable if sub-processor fails
- **Art 82 - Liability** (implied in Article 28(4))
  - Processor liable for sub-processor non-compliance
- **Art 30 - Records of processing activities** (Controller and processor)
  - Document sub-processor agreements

**Secondary References:**
- SOC 2: CC5.2, CC9.2 (control activities, partner obligations)
- ISO 27001: A.14.2 (supplier security requirements)
- ISO 27701: A.2.2 (sub-processor obligations)

**Evidence to Gather:**
- Sub-processor register (from F.2)
- For 3 selected sub-processors:
  - Signed data processing agreement/contract
  - Mapping/comparison document showing:
    - Art 28 obligations from controller DPA
    - Corresponding obligations in sub-processor DPA
    - Confirmation of equivalent protections
    - Key clauses: authorization, confidentiality, security measures, deletion, audit rights
  - Evidence of adequate security level (Annex II equivalent)
- Sub-processor DPA template (if not all negotiated)

---

### F.5 Sub-Processor Register with Required Details
**ISAE Requirement:** Sub-processor register includes: name, business registration number, address, processing description

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 2: Processor must provide list of sub-processors to controller
  - Information must enable controller to exercise rights
- **Art 30 - Records of processing activities** (Controller and processor)
  - Maintain records of sub-processor details
- **Art 5 - Principles** (Principles)
  - Para 2(a): Accountability (maintain sub-processor information)

**Secondary References:**
- SOC 2: CC2.1, CC9.2 (information quality, vendor inventory)
- ISO 27001: A.14.2 (supplier inventory)

**Evidence to Gather:**
- Sub-processor register (from F.2) containing:
  - Sub-processor name
  - Business registration number
  - Registered address
  - Description of processing/services provided
  - Approval status (specific/general)
  - Date added/approved
  - Contact information (if applicable)
- Register available to controllers upon request
- Register updated when changes occur

---

### F.6 Sub-Processor Risk Assessment & Monitoring
**ISAE Requirement:** Risk assessment for each sub-processor; regular monitoring (meetings, inspections, audits); controllers informed

**Primary GDPR References (Cyberday):**
- **Art 28 - Data processor** (Controller and processor)
  - Para 1: Processor responsible for sub-processor compliance
  - Para 3(c): DPA must include security measures (due diligence on sub-processor)
  - Processor must monitor sub-processor compliance
- **Art 5 - Principles** (Principles)
  - Para 2(a): Accountability (demonstrate monitoring of sub-processor)
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1: Appropriate security measures (extend to sub-processor)
  - Para 2: Appropriate to risk and nature of processing
- **Art 30 - Records of processing activities** (Controller and processor)
  - Document sub-processor monitoring

**Secondary References:**
- SOC 2: CC3.2, CC4.1, CC9.2 (risk identification, monitoring, partner management)
- DORA: Third-party risk assessment and monitoring
- ISO 27001: A.14.2 (monitoring supplier performance)
- NIST CSF 2.0: Identify, Assess functions

**Evidence to Gather:**
- Risk assessments for sub-processors covering:
  - Type of data processed
  - Volume of data
  - Security measures
  - Regulatory compliance
  - Incident history
- Latest monitoring evidence (one or more):
  - ISAE 3000 report from sub-processor
  - SOC 2 Type II report
  - ISO 27001 certification
  - Audit report (internal or external)
  - Review meeting records (date, findings)
  - Inspection records (date, observations)
- Findings/observations log showing:
  - Issues identified
  - Remediation actions
  - Timeline for correction
  - Verification of correction
- Controller communication records:
  - Notifications of significant findings
  - Updates on remediation status
  - Proof of controller awareness

---

## G – Transfers to Third Countries

### G.1 Third-Country Transfer Procedure & Annual Review
**ISAE Requirement:** Written procedures for third-country transfers requiring documented controller instructions; uses valid transfer basis; annual review

**Primary GDPR References (Cyberday):**
- **Art 44 - General principle** (Transfers of personal data)
  - Personal data only transferred to third country if safeguards in Chapter V
  - Only per controller instructions
- **Art 45-49 - Transfer mechanisms** (Transfers of personal data)
  - Art 45: Adequacy decision from EU Commission
  - Art 46: Appropriate safeguards (SCC, BCR, etc.)
  - Art 49: Derogations for specific situations
- **Art 28 - Data processor** (Controller and processor)
  - Para 1: Only process per controller instructions
  - Processor responsible for lawful transfers
- **Art 5 - Principles** (Principles)
  - Para 1(a): Lawfulness (transfer must be lawful)
  - Para 2(a): Accountability (document transfer basis)

**Secondary References:**
- SOC 2: D2.1 (data retention per objectives, including location)
- ISO 27701: International data transfer controls
- ISO 27001: A.8.1 (storage in different locations)
- ISO 27017: Cross-border data transfer controls

**Evidence to Gather:**
- Third-country transfer procedure covering:
  - Identification of transfers
  - Assessment of transfer basis (Art 45/46/49)
  - Documentation requirements
  - Controller notification/authorization process
  - Compliance with Schrems II (if applicable)
  - Supplementary measures (if needed)
- Procedure based on GDPR Chapter V requirements
- Dated record of latest procedure review/update (within 12 months)

---

### G.2 Transfers Follow Controller Instructions/Approvals
**ISAE Requirement:** Transfers only per documented controller approvals; register of third-country transfers; verified for 3+ transfers

**Primary GDPR References (Cyberday):**
- **Art 44 - General principle** (Transfers of personal data)
  - No transfer without Chapter V safeguards
  - Only per controller instructions
- **Art 28 - Data processor** (Controller and processor)
  - Para 1: Only process per controller instructions (includes transfers)
  - Processor accountable for lawful transfers
- **Art 5 - Principles** (Principles)
  - Para 2(a): Accountability (document approvals/instructions)

**Secondary References:**
- SOC 2: D2.2 (processing consistency with objectives)
- ISO 27701: Transfer authorization
- ISO 27017: Cross-border transfer approval

**Evidence to Gather:**
- Third-country transfer register containing:
  - Processing activity/data category
  - Recipient/country
  - Transfer date (or ongoing if continuous)
  - Affected controller(s)
  - Transfer basis used (Art 45/46/49)
  - Supplementary measures (if applicable)
- For 3 selected transfers:
  - Controller DPA or written approval:
    - Authorization for transfer to recipient/country
    - Specification of transfer basis
  - Transfer records/documentation:
    - Evidence transfer occurred as approved
    - Data transfer logs
    - Recipient confirmation
  - Compliance verification
- If < 3 transfers: all available with count noted
- If no third-country transfers: written confirmation

---

### G.3 Transfer Mechanism & Supporting Assessment
**ISAE Requirement:** Each transfer has appropriate documented mechanism; assessment of validity; supplementary safeguards if needed

**Primary GDPR References (Cyberday):**
- **Art 45 - Adequacy decision** (Transfers of personal data)
  - Transfer if Commission has adopted adequacy decision for country
  - No other safeguards required
  - Examples: Canada, Japan, Uruguay (current)
- **Art 46 - Appropriate safeguards** (Transfers of personal data)
  - Transfer subject to appropriate safeguards including:
    - Binding corporate rules
    - Standard contractual clauses (SCCs)
    - Approved codes of conduct
    - Approved certifications
- **Art 49 - Derogations** (Transfers of personal data)
  - Limited exceptions when Chapter V doesn't apply:
    - Data subject consent
    - Contract with data subject
    - Public interest
    - Legal claim
    - Vital interests
    - (Others in Art 49)
- **Schrems II considerations** (if applicable):
  - Assessment of third-country legal framework
  - Supplementary measures needed
  - EU Standard Contractual Clauses (SCCs) with supplementary measures

**Secondary References:**
- SOC 2: CC3.2 (risk identification, including transfer risk)
- ISO 27701: Assessment of adequacy of safeguards
- ISO 27017: Transfer mechanism documentation
- DORA: Third-country operational resilience

**Evidence to Gather:**
- For 3 transfers (or all if fewer):
  - Transfer mechanism documentation:
    - **If Art 45**: Adequacy decision reference
    - **If Art 46**: 
      - Standard Contractual Clauses (SCCs) signed
      - OR Binding Corporate Rules (BCRs)
      - OR Approved code of conduct/certification
      - With date and parties
    - **If Art 49**: Derogation basis documented
      - Data subject consent, OR
      - Contract with subject, OR
      - Other basis with explanation
  - Schrems II assessment (if using SCCs):
    - Analysis of third-country legal framework
    - Assessment of government access/surveillance
    - Supplementary measures documentation:
      - Encryption at rest
      - Pseudonymization
      - Technical controls
      - Contractual protections
  - Risk assessment justifying mechanism chosen
- Procedure for assessing transfer mechanisms (if not in G.1)
- Approval documentation
- Evidence of data controller awareness/approval

---

## H – Assistance with Data Subject Rights

### H.1 Data Subject Rights Assistance Procedure & Annual Review
**ISAE Requirement:** Written procedures for processor to assist controller with data subject rights; annual review

**Primary GDPR References (Cyberday):**
- **Articles 12-23 - Data subject rights** (Data subject rights)
  - Art 12: Rights transparency and modalities
  - Art 13-14: Information to be provided
  - Art 15: Right of access
  - Art 16: Right to rectification
  - Art 17: Right to erasure
  - Art 18: Right to restriction
  - Art 19: Notification of rectification/erasure
  - Art 20: Right to data portability
  - Art 21: Right to object
  - Art 22: Automated decision-making
  - Art 23: Restrictions on rights
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(e): DPA must specify processor assistance with rights requests
  - Processor must assist controller in fulfilling rights
- **Art 5 - Principles** (Principles)
  - Para 1(a): Transparency (in exercising rights)
  - Para 2(a): Accountability (document rights procedures)

**Secondary References:**
- SOC 2: P2.1, P3.1 (choice communication, scope consistency)
- ISO 27701: Data subject rights support processes
- ISO 27001: A.5.1 (information security policies)

**Evidence to Gather:**
- Procedure for data subject rights assistance covering:
  - Types of requests (access, deletion, correction, etc.)
  - Receiving requests from controller
  - Timeframe for assistance
  - Methods of assistance (system access, data extracts, etc.)
  - Documentation/logging of requests
  - Escalation for complex requests
  - Regular review mechanism
- Dated record of latest procedure review/update (within 12 months)
- Evidence of alignment with Art 28(3)(e) DPA requirements

---

### H.2 Capability to Assist with All Agreed Rights
**ISAE Requirement:** Procedures enable timely assistance for access, correction, deletion, restriction, information requests as agreed

**Primary GDPR References (Cyberday):**
- **Art 15 - Right of access** (Data subject rights)
  - Processor must assist controller to provide data subject copy
  - Information about processing
- **Art 16 - Right to rectification** (Data subject rights)
  - Processor must assist with correcting inaccurate data
  - Demonstrate correction made
- **Art 17 - Right to erasure** (Data subject rights)
  - Processor must assist controller with deletion
  - Confirm deletion to controller
- **Art 18 - Right to restriction** (Data subject rights)
  - Processor must restrict processing per instruction
  - Document restriction
- **Art 20 - Right to data portability** (Data subject rights)
  - Processor must assist in providing data in machine-readable form
- **Art 21 - Right to object** (Data subject rights)
  - Processor must assist with handling objections
  - Restrict processing upon objection
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(e): DPA specifies which rights processor assists with

**Secondary References:**
- SOC 2: P2.1, P3.1, P4.1, P4.2 (choice, scope, requests, data deletion)
- ISO 27701: Individual rights management
- ISO 27001: A.5.1 (policies for fulfilling rights)

**Evidence to Gather:**
- Work instructions/procedures for each right:
  - **Access requests**: System query, data extract, format (PDF/CSV)
  - **Rectification**: Correction form, approval, update process
  - **Deletion**: Data purge process, confirmation of deletion
  - **Restriction**: Flagging/blocking, process to remove restriction
  - **Portability**: Export formats, delivery method
  - **Objection**: Processing stop, retention policy
- System documentation or redacted demonstration showing:
  - User interface for rights requests
  - Automated/manual processing
  - Timestamping of requests
  - Audit trail of actions
- Request log showing:
  - Date received
  - Right type
  - Requester (controller/subject)
  - Resolution time
  - Completion status
- Completed request example (redacted):
  - Request details
  - Processor response
  - Data provided/action taken
  - Timeline
  - Controller notification
- If no requests received: confirmation of procedure readiness

---

## I – Personal Data Breach Management

### I.1 Breach Notification Procedure & Annual Review
**ISAE Requirement:** Written procedure for processor to inform controller of breaches without undue delay; annual review

**Primary GDPR References (Cyberday):**
- **Art 33 - Notification to supervisory authority** (Controller and processor)
  - Controller responsible for notifying authority within 72 hours
  - **Processor must notify controller without undue delay**
  - Implied: Processor needs breach detection and notification procedure
- **Art 34 - Communication to data subject** (Controller and processor)
  - Controller notifies subject if high risk
  - Processor assists controller
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(f): DPA must specify processor obligation to notify controller of breach
  - Processor responsible for breach notification process
- **Art 5 - Principles** (Principles)
  - Para 2(a): Accountability (document breach procedures)
- **Art 30 - Records of processing activities** (Controller and processor)
  - Document breach management procedures

**Secondary References:**
- SOC 2: C1.2, CC7.3, CC2.3 (confidentiality disposal, security events, external communication)
- ISO 27001: A.17.1 (incident management procedure)
- ISO 27701: Breach notification procedure
- NIS2 Directive: Incident notification timelines

**Evidence to Gather:**
- Breach response procedure covering:
  - Definition of personal data breach (per Art 4(12))
  - Detection mechanisms
  - Assessment of risk to rights/freedoms
  - Documentation of facts
  - Notification decision process
  - Content of controller notification
  - Timeframe (without undue delay, no later than Art 33 requires)
  - Escalation process
  - Sub-processor notification (if applicable)
- Data processing agreement (Annex) specifying:
  - Processor notification obligation
  - Notification timing
  - Content of notification
- Dated record of latest review/approval (within 12 months)

---

### I.2 Breach Identification Controls: Awareness, Monitoring, Log Review
**ISAE Requirement:** Controls to identify breaches: staff awareness, network monitoring, access-log review

**Primary GDPR References (Cyberday):**
- **Art 33 - Notification of breach** (Controller and processor)
  - Processor must identify breaches to notify controller
  - Implies: Detection capability required
- **Art 32 - Security of processing** (Controller and processor)
  - Para 1(c): Ability to restore availability and access (implies breach detection)
  - Para 1(g): Testing of security measures (includes monitoring)
  - Para 2: Appropriate to risk
- **Art 5 - Principles** (Principles)
  - Para 1(f): Integrity and confidentiality (monitoring supports this)
  - Para 2(a): Accountability (demonstrate breach detection)

**Secondary References:**
- SOC 2: CC7.2, CC7.3, CC2.2 (monitoring, event evaluation, staff communication)
- CIS 18 Controls: Control 8 (audit logging), Control 17 (awareness)
- ISO 27001: A.12.4 (event logging), A.6.2 (awareness training)
- NIST CSF 2.0: Detect function

**Evidence to Gather:**
- **Staff Awareness:**
  - Latest training material on breach recognition (can reuse from C.7):
    - Definition of personal data breach
    - Examples (unauthorized access, loss, modification, etc.)
    - Reporting procedure
    - Escalation contacts
  - Training records for relevant staff
- **Network Monitoring:**
  - Network monitoring/SIEM configuration
  - Alert rules for suspicious activity
  - Documentation of tools used (IDS/IPS, firewall, etc.)
  - Alert review procedure
- **Access Log Review:**
  - Access logging configuration
  - Log retention policy
  - Log review procedure:
    - Frequency (daily, weekly, etc.)
    - Who reviews
    - Analysis methodology
    - Escalation criteria
  - Recent redacted investigation example:
    - Alert/log entry
    - Analysis performed
    - Conclusion (breach vs false positive)
    - Timeline

---

### I.3 24-Hour Notification to Controller
**ISAE Requirement:** Breaches notified to controller within 24 hours of processor awareness; includes sub-processor breaches

**Primary GDPR References (Cyberday):**
- **Art 33 - Notification of breach** (Controller and processor)
  - Para 1: Controller must notify supervisory authority within **72 hours** (GDPR requirement)
  - BUT processor must notify controller **without undue delay** and in any case **no later than controller notification to authority**
  - In practice: processor typically has **24 hours** to notify controller
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(f): DPA specifies notification timeline (typically 24 hours)
  - Processor accountable for timely notification
- **Art 5 - Principles** (Principles)
  - Para 2(a): Accountability (demonstrate timely notification)

**Secondary References:**
- SOC 2: CC7.3, CC2.3 (security events, external communication)
- ISO 27001: A.17.1 (incident response timelines)
- ISO 27701: Timely breach notification
- NIS2 Directive: 24-hour notification to authority

**Evidence to Gather:**
- Incident and breach register containing:
  - Breach ID
  - Detection date/time
  - Discovery method (monitoring, staff report, law enforcement, etc.)
  - Description of breach
  - Data categories affected
  - Approximate number of subjects
  - Severity assessment
  - Risk to rights/freedoms
  - Processor awareness time
  - Controller notification date/time
  - Time elapsed (should be ≤ 24 hours)
  - Sub-processor involvement (if any)
  - Status (contained, under investigation, resolved)
- For actual breach(es):
  - Case file for selected breach showing:
    - Initial detection/awareness (timestamp)
    - Investigation findings
    - Scope of breach
    - Root cause
    - Sub-processor notification (if applicable, with timestamps)
    - Dated notification to controller:
      - Email or formal letter
      - Content per Art 28(3)(f) DPA
      - Timestamp (within 24 hours of awareness)
    - Initial response actions taken
    - Timeline of investigation
    - Final report to controller
  - Evidence of escalation to leadership/incident management
  - Evidence of sub-processor notification (if multi-processor breach)
- If no breaches occurred: written confirmation in register

---

### I.4 Assistance with Reports to Danish Data Protection Authority
**ISAE Requirement:** Procedure for assisting controller with notifications to Danish DPA; cover: breach nature, consequences, measures taken/proposed

**Primary GDPR References (Cyberday):**
- **Art 33 - Notification to supervisory authority** (Controller and processor)
  - Para 3: Notification to supervisory authority must include:
    - Name and contact of data protection officer (if appointed)
    - Description of personal data breach
    - Likely consequences for natural persons
    - Measures taken or proposed to address breach and mitigate harm
  - Para 4: Processor must cooperate with controller and authority
- **Art 34 - Communication to data subject** (Controller and processor)
  - If high risk, controller communicates to subjects
  - Processor assists controller
- **Art 28 - Data processor** (Controller and processor)
  - Para 3(f): DPA specifies processor assistance with breach reporting
  - Processor must provide information controller needs for notification
- **Art 30 - Records of processing activities** (Controller and processor)
  - Document breach response and reporting

**Secondary References:**
- SOC 2: CC2.3, CC7.3 (external communication, event documentation)
- ISO 27001: A.17.1 (incident documentation and reporting)
- ISO 27701: Breach reporting to authorities

**Evidence to Gather:**
- Breach response procedure or reporting template containing:
  - Breach description elements:
    - Type of breach (unauthorized access, loss, modification, etc.)
    - Data categories affected
    - Number of subjects (estimated/confirmed)
    - Likely consequences:
      - Physical harm risk
      - Psychological harm
      - Financial harm
      - Discrimination risk
      - Other impacts
  - Measures taken or proposed:
    - Immediate containment actions
    - Mitigation measures
    - Communication plan to subjects
    - Long-term preventive measures
  - Processor assistance requirements:
    - Information processor will provide to controller
    - Timeline for providing information
    - Coordination/communication channel
- For relevant breach(es):
  - Documentation processor provided to controller:
    - Breach investigation report
    - Risk assessment (consequence analysis)
    - Proposed measures/remediations
  - Evidence of controller DPA notification submission
  - Response/acknowledgment from Danish DPA (if received)
  - Subject notification records (if high risk)
  - Remediation tracking
- If no breaches occurred: procedure documentation demonstrating readiness

---

## Cyberday Framework Summary

**Primary GDPR References Used:**

| GDPR Section | Articles | ISAE Controls Mapped |
|---|---|---|
| **Principles** | Art 5-11 | All controls (accountability basis) |
| **Controller & Processor** | Art 24-39 | A.1-A.3, B.1-B.15, C.1-C.7, D.1-D.3, E.1-E.2, F.1-F.6, H.1-H.2, I.1-I.4 |
| **Data Subject Rights** | Art 12-23 | H.1, H.2 |
| **Transfers** | Art 44-49 | G.1, G.2, G.3 |
| **Liability** | Art 83 | Throughout (accountability) |

**Secondary Cyberday Frameworks:**
- SOC 2: Supporting implementation controls
- ISO 27001 (2022): Security management system controls
- ISO 27017: Cloud-specific security
- ISO 27701: Privacy-specific controls
- DORA: Operational resilience (third-party risk)
- NIS2 Directive: Incident notification
- NIST CSF 2.0: Risk assessment framework
- CIS 18 Controls: Foundational controls
- Cyber Essentials: Basic cyber hygiene

---

## Next Steps

1. **Load Mapping into Cyberday:** Reference this mapping for each ISAE 3000 control
2. **Align Cyberday Tasks:** Ensure Cyberday tasks are created for each GDPR article requirement
3. **Evidence Collection:** Use GDPR articles as primary search filters in Cyberday
4. **Compliance Tracking:** Monitor completion of GDPR Article requirements per control
5. **Audit Preparation:** Prepare evidence package organized by:
   - GDPR Article (primary)
   - ISAE Control Number (secondary)
   - SOC 2/ISO 27001 (supplementary verification)

---

**Document Version:** 1.0 GDPR-Primary  
**Last Updated:** 2026-10-02  
**Next Review:** 2027-10-02

