# ISAE 3000 Type 1 Controls → Cyberday Reference Document Mapping

**Prepared for:** Elumi  
**Framework:** ISAE 3000 Type 1 with Reasonable Assurance  
**Reference System:** Cyberday Compliance Platform  
**Date:** 2026-10-02

---

## A – Controller Instructions

### A.1 Processing Instructions & Procedure Review
**ISAE Requirement:** Written procedures requiring documented controller instructions; annual assessments

**Recommended Cyberday References:**
- **SOC 2 - CC3.1:** Sufficient specifying of objectives (establishes control objectives framework)
- **SOC 2 - CC5.3:** Establishment of policies (document and maintain policies)
- **SOC 2 - CC7.1:** Procedures for monitoring changes to configurations
- **GDPR (Cyberday):** Article 28 - Processor obligations regarding instructions
- **ISO 27001 (2022):** Control A.5.1 - Policies for information security

**Evidence to Gather:**
- Link to documented controller instruction procedure in cyberday system
- Annual procedure review records/dates
- Updated processing instructions registry

---

### A.2 Compliance with Processing Agreements
**ISAE Requirement:** Data processor only processes personal data per controller instructions; DPA alignment

**Recommended Cyberday References:**
- **SOC 2 - P5.1:** Ensuring processing activities by the entity are consistent with its objectives
- **SOC 2 - CC2.1:** Quality information to support internal controls (ensure clarity of DPA terms)
- **GDPR (Cyberday):** Article 5(1)(a) - Processing lawfulness principle
- **ISO 27017:** Control A.2.1 - Cloud-specific data processing requirements

**Evidence to Gather:**
- Processing activities register (mapped to DPAs)
- Sample DPAs with processing scope
- Activity logs showing alignment with instructions

---

### A.3 Reporting Potentially Unlawful Instructions
**ISAE Requirement:** Data processor assesses instructions and reports those violating GDPR/EU law to controller

**Recommended Cyberday References:**
- **SOC 2 - CC3.3:** Potential fraud is considered (evaluation of non-compliance risks)
- **SOC 2 - CC2.3:** Communication with external parties (escalation to controllers)
- **GDPR (Cyberday):** Article 36 - Data Protection Impact Assessment triggers
- **NIS2 Directive (Cyberday):** Incident reporting and escalation procedures

**Evidence to Gather:**
- Procedure for assessing instruction lawfulness
- Case records (if applicable) with controller notifications
- Confirmation of zero unlawful cases (if none occurred)

---

## B – Technical and Physical Security Measures

### B.1 Safeguards Implementation & Review
**ISAE Requirement:** Written procedures for safeguards as agreed with controllers; annual assessments

**Recommended Cyberday References:**
- **SOC 2 - CC5.1:** Control activities for mitigation of risks
- **SOC 2 - CC6.1c:** Technical security for protected information assets
- **SOC 2 - CC4.1:** Evaluation of internal controls
- **ISO 27001 (2022) - Full (Active):** A.5 - Organizational Controls
- **ISO 27017 (Active):** Cloud-specific technical and organizational measures

**Evidence to Gather:**
- Security measures implementation procedure
- Latest procedure review date
- DPA security annex
- Implementation evidence (configurations, screenshots, audit reports)

---

### B.2 Risk Assessment & Technical Measures
**ISAE Requirement:** Risk assessment performed; appropriate technical measures implemented based on assessed risk

**Recommended Cyberday References:**
- **SOC 2 - CC3.2:** Identification of risks related to objectives
- **SOC 2 - CC5.1:** Control activities for mitigation of risks
- **SOC 2 - CC5.2:** Control activities for achievement of objectives
- **DORA (Active):** Risk assessment and management framework
- **NIST CSF 2.0 (Active):** Identify & Protect functions
- **ISO 27001 (2022) - A.12:** Operational Controls (security measures)

**Evidence to Gather:**
- Latest dated risk assessment
- Risk assessment review and management approval
- DPA security requirements
- Evidence of technical measure implementation

---

### B.3 Antivirus Protection & Updates
**ISAE Requirement:** Antivirus software installed and regularly updated on relevant systems

**Recommended Cyberday References:**
- **SOC 2 - CC6.1c:** Technical security for protected information assets (malware protection)
- **SOC 2 - CC7.2:** Monitoring of system components for anomalies
- **CIS 18 Controls (Active):** Control 10 - Malware Defenses
- **ISO 27001 (2022) - A.12.2:** Malware protection
- **NIST CSF 2.0:** Detect function

**Evidence to Gather:**
- Inventory of systems processing personal data
- Antivirus/endpoint protection report showing coverage
- Patch update status report (last 90 days)

---

### B.4 Firewall Protection for External Access
**ISAE Requirement:** External access to systems protected through secured firewall

**Recommended Cyberday References:**
- **SOC 2 - CC6.2:** Prior to issuing system credentials (logical access control)
- **SOC 2 - CC7.1:** Procedures for monitoring changes to configurations
- **CIS 18 Controls (Active):** Control 1 - Inventory and Control of Enterprise Assets
- **ISO 27001 (2022) - A.13.1:** Network security boundary
- **NIST CSF 2.0:** Protect function (access control)

**Evidence to Gather:**
- Network diagram showing external access routes and firewall placement
- Current firewall configuration/rules export
- Firewall configuration standard document

---

### B.5 Network Segmentation
**ISAE Requirement:** Internal networks segmented to restrict access to personal data systems/databases

**Recommended Cyberday References:**
- **SOC 2 - CC6.1a:** Identification and listing of assets (define protected assets)
- **SOC 2 - CC6.2b:** Logical access control for protected information (network-level controls)
- **CIS 18 Controls (Active):** Control 1 & 3 - Network architecture
- **ISO 27001 (2022) - A.13.1:** Network segregation
- **NIST CSF 2.0:** Protect function (segmentation)

**Evidence to Gather:**
- Network segmentation diagram
- VLAN/firewall configuration showing restricted access
- List of permitted inter-segment connections

---

### B.6 Access Control for Personal Data
**ISAE Requirement:** Access to personal data limited to users with work-related need; periodic review

**Recommended Cyberday References:**
- **SOC 2 - CC6.2:** Prior to issuing system credentials; logical access must be approved
- **SOC 2 - CC4.1:** Evaluation of internal controls (periodic access review)
- **SOC 2 - CC6.1b:** Logical access control for protected information assets
- **ISO 27001 (2022) - A.9:** Access Control
- **GDPR (Cyberday):** Article 32(1)(b) - Restricting access to personal data
- **CIS 18 Controls (Active):** Control 2 - Access Control

**Evidence to Gather:**
- Access control procedure with authorization and review process
- Current user access listing
- Sample access approvals and business justifications
- Latest access review records

---

### B.7 System Monitoring & Alerts
**ISAE Requirement:** System monitoring with alarm features; investigation and escalation of security events

**Recommended Cyberday References:**
- **SOC 2 - CC7.2:** Monitoring of system components for anomalies
- **SOC 2 - CC7.3:** Evaluation of security events
- **SOC 2 - CC7.4:** Evaluation of monitoring and response to events
- **SOC 2 - C1.2:** Disposal procedures for confidential information (incident response)
- **CIS 18 Controls (Active):** Control 8 - Audit Logging
- **NIST CSF 2.0:** Detect function
- **ISO 27001 (2022) - A.12.4:** Event logging and monitoring

**Evidence to Gather:**
- Monitoring configuration for relevant systems
- Alert overview/rule set
- Investigation records for 3 selected alerts
- Controller notifications (if applicable)

---

### B.8 Encryption for Internet/Email Transfers
**ISAE Requirement:** Effective encryption applied when transmitting sensitive/confidential personal data via internet/email

**Recommended Cyberday References:**
- **SOC 2 - CC6.1c:** Technical security for protected information assets (encryption in transit)
- **SOC 2 - C1.2:** Measures to prevent unauthorized access to confidential information
- **ISO 27001 (2022) - A.10.1:** Cryptography
- **ISO 27017 (Active):** Cloud cryptographic controls
- **NIST CSF 2.0:** Protect function (encryption)

**Evidence to Gather:**
- Procedure/user guidance for encrypted transfers
- Configuration or screenshots of secure channels
- Redacted transfer example
- Overview of any unencrypted transfers (or confirmation of none)

---

### B.9 Logging of User & Security Events
**ISAE Requirement:** Logging of admin activities, security incidents, changes to logging, rights changes, failed logins, etc.

**Recommended Cyberday References:**
- **SOC 2 - CC7.2:** Monitoring of system components for anomalies (comprehensive logging)
- **SOC 2 - CC7.3:** Evaluation of security events
- **SOC 2 - CC6.2c:** Monitoring and evaluating logical access (privileged user tracking)
- **CIS 18 Controls (Active):** Control 8 - Audit Logging & Response
- **ISO 27001 (2022) - A.12.4:** Event logging & monitoring
- **ISO 27017 (Active):** Cloud logging controls
- **NIST CSF 2.0:** Detect function

**Evidence to Gather:**
- Logging standard/policy covering privileged activity and failed logins
- Current logging configuration
- Representative redacted log extracts
- Log protection and retention settings documentation

---

### B.10 Pseudonymization/Anonymization in Dev/Test
**ISAE Requirement:** Personal data in development/testing must be pseudonymized/anonymized (or under documented controller agreement)

**Recommended Cyberday References:**
- **SOC 2 - PI1.2:** Implementation of policies and procedures for system inputs (data quality control)
- **GDPR (Cyberday):** Article 32(1)(d) - Pseudonymization and encryption
- **ISO 27701 (Active):** Privacy-specific controls for data minimization
- **ISO 27001 (2022) - A.5:** Organizational controls (data handling)
- **DORA (Active):** Data security in operational environments

**Evidence to Gather:**
- Procedure for using personal data in development/testing
- Inventory of dev/test databases
- Data extracts/config evidence for 3 selected databases showing anonymization
- If identifiable data used: relevant DPA/instructions and approval evidence

---

### B.11 Vulnerability Scans & Penetration Testing
**ISAE Requirement:** Technical measures tested regularly through vulnerability scans and penetration tests; weaknesses addressed

**Recommended Cyberday References:**
- **SOC 2 - CC4.1:** Evaluation of internal controls (periodic assessment)
- **SOC 2 - CC7.2:** Monitoring of system components for anomalies
- **CIS 18 Controls (Active):** Control 5 - Vulnerability Management
- **NIST CSF 2.0:** Identify & Detect functions
- **ISO 27001 (2022) - A.14.2:** Vulnerability management
- **DORA (Active):** Internal testing and monitoring

**Evidence to Gather:**
- Testing schedule
- Latest vulnerability scan and penetration test reports (scope, date, internal vs external)
- Finding tracker
- Recent remediation or risk acceptance record with controller communication (if relevant)

---

### B.12 Change & Patch Management
**ISAE Requirement:** System changes and patches made consistently per established procedures; includes security patches

**Recommended Cyberday References:**
- **SOC 2 - CC8.1:** Change management procedures (formal change control)
- **SOC 2 - CC7.1:** Procedures for monitoring changes to configurations
- **CIS 18 Controls (Active):** Control 6 - Access Control & Asset Management
- **ISO 27001 (2022) - A.14.1:** Information security change management
- **NIST CSF 2.0:** Protect function

**Evidence to Gather:**
- Change and patch management procedure
- Current patch-status report
- Selected approved change/deployment tickets

---

### B.13 User Access Management & Periodic Review
**ISAE Requirement:** Formalized procedure for granting/removing access; regular reconsideration of access with business need justification

**Recommended Cyberday References:**
- **SOC 2 - CC6.2:** Prior to issuing system credentials; periodic review of access
- **SOC 2 - CC4.1:** Evaluation of internal controls (periodic access review)
- **SOC 2 - CC7.3:** Evaluation of security events (removal on departure)
- **ISO 27001 (2022) - A.9.2:** User access management (onboarding, review, offboarding)
- **GDPR (Cyberday):** Article 32(1)(b) - Restricting access
- **CIS 18 Controls (Active):** Control 2 - Access Control

**Evidence to Gather:**
- Access management procedure
- Current user access listing
- Access requests/approvals for 3 employees with business justification
- Latest periodic access review with change records
- Employee departure/deactivation record

---

### B.14 Two-Factor Authentication for High-Risk Processing
**ISAE Requirement:** Two-factor authentication required and active for high-risk systems/accounts

**Recommended Cyberday References:**
- **SOC 2 - CC6.2:** Prior to issuing system credentials (multi-factor authentication for sensitive access)
- **SOC 2 - CC6.1c:** Technical security for protected information assets (access controls)
- **CIS 18 Controls (Active):** Control 2 - Access Control (MFA requirement)
- **ISO 27001 (2022) - A.9.4:** Access management for privileged rights
- **NIST CSF 2.0:** Protect function
- **DORA (Active):** MFA for critical systems

**Evidence to Gather:**
- Procedure/risk assessment identifying high-risk systems and accounts
- System settings or screenshots showing MFA enforcement
- VPN guidance (if applicable)

---

### B.15 Physical Access Safeguards
**ISAE Requirement:** Physical access controls restrict access by authorized persons only to premises/data centers where personal data are stored

**Recommended Cyberday References:**
- **SOC 2 - CC6.1a:** Identification and listing of assets (physical locations)
- **SOC 2 - CC6.3:** Physical access to facilities, equipment, and assets
- **CIS 18 Controls (Active):** Control 1 - Physical Asset Management
- **ISO 27001 (2022) - A.11.1:** Physical security perimeter
- **NIST CSF 2.0:** Protect function (physical access)

**Evidence to Gather:**
- Physical access and badge/key procedure with issuance and deactivation
- Current list of authorized persons
- Latest access review
- Selected access record
- Third-party facility report (if data center outsourced)

---

## C – Organisational Measures

### C.1 Information Security Policy & Management Approval
**ISAE Requirement:** Written information security policy approved by management, communicated to stakeholders, based on risk assessment; annual review

**Recommended Cyberday References:**
- **SOC 2 - CC1.1:** Management commitment
- **SOC 2 - CC2.2:** Internal communication of information (dissemination of security policy)
- **SOC 2 - CC3.2:** Identification of risks related to objectives (risk-based policy)
- **ISO 27001 (2022) - A.5.1:** Policies for information security
- **GDPR (Cyberday):** Article 32 - Security of processing
- **NIST CSF 2.0:** Govern function (policy establishment)

**Evidence to Gather:**
- Current information security policy
- Dated management approval/review (within past year)
- Intranet screenshot or distribution record showing availability to staff

---

### C.2 Policy Compliance with Data Processing Agreements
**ISAE Requirement:** Management verifies information security policy doesn't conflict with DPAs; policy covers security commitments in contracts

**Recommended Cyberday References:**
- **SOC 2 - CC2.1:** Quality information to support internal controls (policy alignment)
- **SOC 2 - CC5.2:** Control activities for achievement of objectives (DPA fulfillment)
- **GDPR (Cyberday):** Article 28(4) - Processor obligations alignment with DPA
- **ISO 27001 (2022) - A.5.1:** Policy integration with contractual obligations

**Evidence to Gather:**
- Management's documented assessment/mapping between policy and contractual security requirements
- For 3 selected DPAs: relevant security clauses and policy coverage evidence
- Documentation of gaps resolution

---

### C.3 Employee Screening During Recruitment
**ISAE Requirement:** Employees screened per procedure as part of employment; includes references, criminal records, diplomas per DPA requirements

**Recommended Cyberday References:**
- **SOC 2 - CC1.2:** Board of directors oversight (establishment of hiring standards)
- **SOC 2 - CC1.3:** Established responsibilities (HR procedures)
- **ISO 27001 (2022) - A.6.1:** Personnel screening
- **GDPR (Cyberday):** Article 28 Recital 81 - Personnel selection criteria
- **DORA (Active):** Staff qualification requirements

**Evidence to Gather:**
- Employee screening procedure
- Overview of DPA screening requirements
- For 3 DPAs: requirement mapping in procedure
- For 3 employees: redacted screening checklists with dates and outcomes
- (If <3 hires: all available with count noted)

---

### C.4 Employee Confidentiality & Information Security Induction
**ISAE Requirement:** Employees sign confidentiality agreements upon appointment; receive induction on information security policy and data processing procedures

**Recommended Cyberday References:**
- **SOC 2 - CC1.1:** Management commitment (communication of security culture)
- **SOC 2 - CC2.2:** Internal communication of information (staff awareness)
- **ISO 27001 (2022) - A.6.2:** Information security awareness, education and training
- **GDPR (Cyberday):** Article 28 - Processor obligations
- **ISO 27017 (Active):** Cloud-specific training requirements

**Evidence to Gather:**
- Onboarding/induction procedure
- List of employees appointed
- For 3 new hires: signed confidentiality agreements
- Dated induction records covering information security policy and processing procedures
- (If <3 hires: all available with count noted)

---

### C.5 Employee Offboarding: Access Removal & Asset Return
**ISAE Requirement:** Formalized process to ensure users' rights deactivated/terminated upon departure; assets returned

**Recommended Cyberday References:**
- **SOC 2 - CC6.2:** Prior to issuing credentials (removal upon termination)
- **SOC 2 - CC6.2c:** Monitoring and evaluating logical access (access removal)
- **ISO 27001 (2022) - A.6.3:** Return of assets
- **GDPR (Cyberday):** Article 32(1) - Security measures apply until data deletion

**Evidence to Gather:**
- Offboarding procedure
- List of employees who left
- Recent completed offboarding checklist
- Access deactivation ticket
- Asset return confirmation (if applicable)

---

### C.6 Continuation of Confidentiality Obligations Post-Departure
**ISAE Requirement:** Upon resignation/dismissal, employees reminded that confidentiality agreement remains valid and confidentiality duty continues

**Recommended Cyberday References:**
- **SOC 2 - CC1.1:** Management commitment (reinforcement of ethical standards)
- **SOC 2 - CC2.3:** Communication with external parties (confidentiality requirements)
- **ISO 27001 (2022) - A.6.2:** Information security awareness
- **GDPR (Cyberday):** General confidentiality principles

**Evidence to Gather:**
- Standard departure notice or offboarding instruction on continuing confidentiality
- For recent departing employee: signed confidentiality agreement
- Dated reminder or acknowledgement (if provided)

---

### C.7 Security Awareness Training
**ISAE Requirement:** Regular security awareness training provided to employees on IT security and data processing security

**Recommended Cyberday References:**
- **SOC 2 - CC1.1:** Management commitment (tone at the top)
- **SOC 2 - CC2.2:** Internal communication of information (staff education)
- **SOC 2 - PI2.2:** Education of personnel regarding privacy (privacy-specific training)
- **ISO 27001 (2022) - A.6.2:** Information security awareness, education and training
- **CIS 18 Controls (Active):** Control 17 - Security Awareness & Training
- **NIST CSF 2.0:** Govern function (awareness & training)

**Evidence to Gather:**
- Latest training material with date (including personal data protection content)
- Attendance/completion overview for relevant staff
- Follow-up records for missing training

---

## D – Return and Deletion of Personal Data

### D.1 Storage & Deletion Procedures & Annual Review
**ISAE Requirement:** Written procedures for storing and deleting personal data per controller agreement; annual assessment of procedure updates

**Recommended Cyberday References:**
- **SOC 2 - D1.1:** Notification of personal data processing objectives to data subjects
- **SOC 2 - D2.2:** Ensuring personal data processing is consistent with objectives (retention alignment)
- **GDPR (Cyberday):** Article 17 - Right to erasure ("right to be forgotten")
- **ISO 27701 (Active):** Privacy-specific data retention controls
- **ISO 27001 (2022) - A.8.3:** Retention of information

**Evidence to Gather:**
- Current storage and deletion procedure
- Dated record of latest procedure review and updates

---

### D.2 Retention Periods & Deletion Routines per Agreement
**ISAE Requirement:** Specific retention periods and deletion routines defined in agreement; verified compliance for selected activities

**Recommended Cyberday References:**
- **SOC 2 - D2.1:** Ensuring retention of personal data in accordance with objectives
- **SOC 2 - D2.2:** Ensuring personal data processing is consistent with objectives
- **GDPR (Cyberday):** Article 5(1)(e) - Storage limitation principle
- **ISO 27701 (Active):** Data minimization & retention
- **NIST CSF 2.0:** Govern function (data lifecycle)

**Evidence to Gather:**
- Controller instructions or DPA specifying retention periods
- Retention schedule
- Deletion procedure
- For 2 processing activities: records/system settings showing data retention
- For 2 processing activities: deletion logs showing completed deletion
- (If <2 available: provide all with count noted)

---

### D.3 Return or Deletion Upon Termination
**ISAE Requirement:** Data returned to controller and/or deleted per agreement upon processing termination; no unlawful retention

**Recommended Cyberday References:**
- **SOC 2 - D2.3:** Depending on the nature of processing relationships, removal of personal data
- **GDPR (Cyberday):** Article 17 - Right to erasure
- **ISO 27701 (Active):** Data return and destruction procedures
- **ISO 27001 (2022) - A.8.3:** Retention of information (removal of data)

**Evidence to Gather:**
- Termination procedure covering return, deletion, and lawful retention
- Most recent terminated arrangement with related instructions
- Return receipt, deletion record, or lawful retention record
- Confirmation if no arrangement ended

---

## E – Storage and Processing Locations

### E.1 Storage & Processing Procedure Aligned with DPA
**ISAE Requirement:** Written procedure requiring personal data stored per controller agreement; annual assessment; compliance verified for 3 activities

**Recommended Cyberday References:**
- **SOC 2 - D2.2:** Ensuring personal data processing is consistent with objectives (location compliance)
- **SOC 2 - CC2.1:** Quality information to support internal controls (location transparency)
- **GDPR (Cyberday):** Article 28(3)(c) - Processor location obligations
- **ISO 27017 (Active):** Cloud processing location controls
- **ISO 27001 (2022) - A.8.1:** Onsite and offsite equipment

**Evidence to Gather:**
- Current storage and processing procedure
- Evidence of latest review
- Overview of processing activities
- For 3 activities: DPA and system configuration/data-flow evidence showing location compliance

---

### E.2 Actual Processing/Storage Locations Match Approved Locations
**ISAE Requirement:** Actual processing and storage locations correspond to controller-approved locations; verified for 3 activities

**Recommended Cyberday References:**
- **SOC 2 - D2.1:** Ensuring retention of personal data in accordance with objectives
- **SOC 2 - CC7.1:** Procedures for monitoring changes to configurations (geo-compliance)
- **GDPR (Cyberday):** Article 28(3)(c) & Chapter V - Location of processing
- **ISO 27017 (Active):** Cloud region and jurisdiction controls
- **DORA (Active):** Geographical concentration of resources

**Evidence to Gather:**
- Processing-activity register or location inventory identifying sites, countries, cloud regions, service providers
- For 3 activities: DPA/controller approvals
- Dated configuration or data-flow evidence showing actual processing/storage locations

---

## F – Use of Sub-Processors

### F.1 Sub-Processor Appointment Procedure & Annual Review
**ISAE Requirement:** Written procedures for engaging sub-processors; includes DPA requirements; annual assessment

**Recommended Cyberday References:**
- **SOC 2 - CC5.3:** Establishment of policies (sub-processor governance)
- **SOC 2 - CC9.2:** Partner risk management (sub-processor selection)
- **GDPR (Cyberday):** Article 28(2) & (4) - Sub-processor authorization and instruction
- **ISO 27001 (2022) - A.14.2:** Supplier relationships & governance
- **DORA (Active):** Critical third-party risk management

**Evidence to Gather:**
- Sub-processor appointment procedure
- DPA agreement template for sub-processors
- Dated record of latest procedure review

---

### F.2 Sub-Processor Authorization & Register
**ISAE Requirement:** Only approved sub-processors used; verified authorizations for 2 selected sub-processors

**Recommended Cyberday References:**
- **SOC 2 - CC9.2:** Partner risk management (approved vendor management)
- **SOC 2 - CC5.2:** Control activities for achievement of objectives (authorization)
- **GDPR (Cyberday):** Article 28(2) - Specific or general authorization
- **ISO 27001 (2022) - A.14.2:** Supplier relationships

**Evidence to Gather:**
- Current sub-processor register identifying service and affected controllers
- For 2 sub-processors: DPA or written controller approvals evidencing authorization

---

### F.3 Sub-Processor Change Notification & Approval
**ISAE Requirement:** Controllers notified/asked to approve sub-processor changes as agreed; objection procedures in place

**Recommended Cyberday References:**
- **SOC 2 - CC2.3:** Communication with external parties (notification of changes)
- **SOC 2 - CC9.2:** Partner risk management (change management)
- **GDPR (Cyberday):** Article 28(2)(h) - Notification and objection rights
- **ISO 27001 (2022) - A.14.2:** Changes in supplier relationships

**Evidence to Gather:**
- Sub-processor change procedure and log
- Dated controller notices for selected changes
- Objections and resolutions, or specific approvals
- Confirmation if no changes occurred

---

### F.4 Data Protection Obligations Passed to Sub-Processors
**ISAE Requirement:** Sub-processor agreements impose same data protection obligations as in controller DPA; verified for 3 sub-processors

**Recommended Cyberday References:**
- **SOC 2 - CC5.2:** Control activities for achievement of objectives (contractual requirements)
- **SOC 2 - CC9.2:** Partner risk management (obligation cascade)
- **GDPR (Cyberday):** Article 28(4) - Equivalent obligations for sub-processors
- **ISO 27001 (2022) - A.14.2:** Supplier security requirements

**Evidence to Gather:**
- Sub-processor register
- For 3 sub-processors: signed DPA agreements
- Comparison/mapping showing controller DPA obligations pass to sub-processor DPA

---

### F.5 Sub-Processor Register with Required Details
**ISAE Requirement:** Approved sub-processor list includes: name, business registration number, address, processing description

**Recommended Cyberday References:**
- **SOC 2 - CC2.1:** Quality information to support internal controls (data accuracy)
- **SOC 2 - CC9.2:** Partner risk management (vendor inventory)
- **GDPR (Cyberday):** Article 28(2) - Information about sub-processors
- **ISO 27001 (2022) - A.14.2:** Supplier information management

**Evidence to Gather:**
- Sub-processor register from F.2, including:
  - Name
  - Business registration number
  - Address
  - Processing description
  - Approval status

---

### F.6 Sub-Processor Risk Assessment & Monitoring
**ISAE Requirement:** Risk assessment performed for each sub-processor; regular monitoring (meetings, inspections, audits); controllers informed

**Recommended Cyberday References:**
- **SOC 2 - CC3.2:** Identification of risks related to objectives (third-party risk)
- **SOC 2 - CC4.1:** Evaluation of internal controls (monitoring)
- **SOC 2 - CC9.2:** Partner risk management (periodic review of third parties)
- **DORA (Active):** Critical third-party risk assessment and monitoring
- **NIST CSF 2.0:** Identify & Assess functions (third-party risk)
- **ISO 27001 (2022) - A.14.2:** Monitoring of supplier performance

**Evidence to Gather:**
- Current risk assessments for sub-processors
- Latest ISAE 3000, SOC 2, or equivalent assurance reports
- Records of review/monitoring (meetings, inspections)
- Findings and follow-up records with controller communications (if applicable)

---

## G – Transfers to Third Countries

### G.1 Third-Country Transfer Procedure & Annual Review
**ISAE Requirement:** Written procedures requiring documented controller instructions for third-country transfers using valid transfer basis; annual assessment

**Recommended Cyberday References:**
- **SOC 2 - D2.1:** Ensuring retention of personal data in accordance with objectives (location controls)
- **GDPR (Cyberday):** Chapter V - Transfers of personal data to third countries
- **GDPR (Cyberday):** Articles 45-49 - Adequacy decisions and transfer mechanisms
- **ISO 27701 (Active):** International data transfer controls
- **DORA (Active):** Geographical limitations on data processing

**Evidence to Gather:**
- Third-country transfer procedure
- Dated record of latest procedure review

---

### G.2 Transfers Follow Controller Instructions/Approvals
**ISAE Requirement:** Transfers only per documented controller approvals; register of third-country transfers maintained; verified for 3 transfers

**Recommended Cyberday References:**
- **SOC 2 - D2.2:** Ensuring personal data processing is consistent with objectives (transfer authorization)
- **GDPR (Cyberday):** Article 28(3)(c) - Controller authorization for transfers
- **ISO 27701 (Active):** Data transfer authorization
- **ISO 27017 (Active):** Cross-border data transfer controls

**Evidence to Gather:**
- Third-country transfer register identifying recipients, destinations, affected controllers
- For 3 transfers: DPA or controller approvals with transfer records
- (If <3 transfers: all available with count noted)

---

### G.3 Transfer Mechanism & Supporting Assessment
**ISAE Requirement:** Each third-country transfer has appropriate documented transfer mechanism and assessment of validity; supplementary safeguards if needed

**Recommended Cyberday References:**
- **GDPR (Cyberday):** Articles 45-49 - Transfer mechanisms:
  - Article 45 - Adequacy decisions
  - Article 46 - Appropriate safeguards (SCCs, BCRs)
  - Article 49 - Derogations for specific situations
- **SOC 2 - CC3.2:** Identification of risks related to objectives (transfer risk assessment)
- **ISO 27701 (Active):** Assessment of adequacy of safeguards
- **DORA (Active):** Third-country operational resilience

**Evidence to Gather:**
- For 3 transfers: transfer mechanism documentation (SCC, adequacy decision, etc.)
- Supplementary safeguards assessment (if applicable)
- Procedure for assessing transfer mechanisms (if not in G.1)

---

## H – Assistance with Data Subject Rights

### H.1 Data Subject Rights Assistance Procedure & Annual Review
**ISAE Requirement:** Written procedures for processor to assist controller with data subject rights; annual assessment

**Recommended Cyberday References:**
- **SOC 2 - P2.1:** Communication of choices about personal information to data subjects (choice assistance)
- **SOC 2 - P3.1:** Scope of personal data collection consistent with privacy objectives (scope management)
- **GDPR (Cyberday):** Articles 15-22 - Data subject rights
- **GDPR (Cyberday):** Article 28(3)(e) - Processor assistance obligations
- **ISO 27701 (Active):** Data subject rights support processes

**Evidence to Gather:**
- Procedure for receiving and assisting with data-subject rights requests
- Dated record of latest procedure review

---

### H.2 Capability to Assist with All Agreed Rights
**ISAE Requirement:** Procedures enable timely assistance for access, correction, deletion, restriction, information requests as agreed

**Recommended Cyberday References:**
- **SOC 2 - P2.1:** Communication of choices (assist with opt-out/object)
- **SOC 2 - P3.1:** Scope consistency (assist with access)
- **SOC 2 - P4.1 & P4.2:** Requests from data subjects (correction/deletion assistance)
- **GDPR (Cyberday):** Articles 15-22 - Specific rights and processor obligations
- **ISO 27701 (Active):** Assistance with individual rights

**Evidence to Gather:**
- Work instructions for access, rectification, deletion, restriction, information requests
- System documentation or redacted demonstration of relevant functions
- Request log and completed request example (or confirmation of zero)

---

## I – Personal Data Breach Management

### I.1 Breach Notification Procedure & Annual Review
**ISAE Requirement:** Written procedure for processor to inform controller of breaches without undue delay; annual assessment

**Recommended Cyberday References:**
- **SOC 2 - C1.2:** Disposal procedures for confidential information (breach response)
- **SOC 2 - CC7.3:** Evaluation of security events (incident classification)
- **SOC 2 - CC2.3:** Communication with external parties (controller notification)
- **GDPR (Cyberday):** Article 33 - Notification to supervisory authority
- **GDPR (Cyberday):** Article 28(3)(f) - Processor notification to controller
- **NIS2 Directive (Cyberday):** Incident notification timelines
- **ISO 27701 (Active):** Personal data breach management
- **ISO 27001 (2022) - A.17.1:** Incident management procedure

**Evidence to Gather:**
- Breach-response and controller-notification procedure
- Dated record of latest review and approval

---

### I.2 Breach Identification Controls: Awareness, Monitoring, Log Review
**ISAE Requirement:** Controls to identify breaches: staff awareness, network monitoring, access-log review

**Recommended Cyberday References:**
- **SOC 2 - CC7.2:** Monitoring of system components for anomalies (network monitoring)
- **SOC 2 - CC7.3:** Evaluation of security events (anomaly investigation)
- **SOC 2 - CC2.2:** Internal communication of information (breach awareness)
- **CIS 18 Controls (Active):** Control 8 - Audit Logging; Control 17 - Awareness & Training
- **NIST CSF 2.0:** Detect function (anomaly detection)
- **ISO 27001 (2022) - A.12.4:** Event logging & monitoring

**Evidence to Gather:**
- Latest breach awareness material (can reuse from C.7)
- Network alert settings and access-log review procedure
- Redacted recent investigation example

---

### I.3 Timely Breach Notification (Within 24 Hours)
**ISAE Requirement:** Breaches notified to controller within 24 hours of processor awareness; includes sub-processor breaches

**Recommended Cyberday References:**
- **SOC 2 - CC7.3:** Evaluation of security events (timely incident response)
- **SOC 2 - CC2.3:** Communication with external parties (urgent notification)
- **GDPR (Cyberday):** Article 33(1) - Notification within 72 hours (GDPR requirement)
- **GDPR (Cyberday):** Article 28(3)(f) - Processor notification to controller
- **NIS2 Directive (Cyberday):** Incident notification timeline (within 24 hours to authority)
- **ISO 27701 (Active):** Timely breach notification
- **ISO 27001 (2022) - A.17.1:** Incident response timelines

**Evidence to Gather:**
- Incident and breach register (with scope/filter documentation)
- For actual breach: case file showing awareness time, sub-processor notice, dated controller notification
- Confirmation if no breaches occurred

---

### I.4 Assistance with Reports to Danish Data Protection Authority
**ISAE Requirement:** Procedure for assisting controller in filing reports with Danish DPA covering: breach nature, consequences, measures taken/proposed

**Recommended Cyberday References:**
- **SOC 2 - CC2.3:** Communication with external parties (authority notification assistance)
- **SOC 2 - CC7.3:** Evaluation of security events (documentation of incident details)
- **GDPR (Cyberday):** Article 33 - Content of notification to supervisory authority
- **GDPR (Cyberday):** Denmark-specific guidance on DPA reporting
- **ISO 27001 (2022) - A.17.1:** Incident response and post-incident activities

**Evidence to Gather:**
- Breach-response procedure or reporting template covering:
  - Nature of breach
  - Likely consequences
  - Measures taken or proposed
- For relevant breach: information provided to controller and response records
- Procedure documentation (if no breaches occurred)

---

## Summary: Cyberday Framework Alignment

**Primary Cyberday Frameworks Referenced for ISAE 3000:**
1. **SOC 2 (Active)** — Primary reference (63 requirements across 13 Trust Service Categories)
2. **GDPR (Active)** — Data protection obligations
3. **ISO 27001 (2022): Full (Active)** — Information security management
4. **ISO 27017 (Active)** — Cloud-specific controls
5. **ISO 27701 (Active)** — Privacy controls
6. **DORA (Active)** — Operational resilience & risk management
7. **NIS2 Directive (Active)** — Incident reporting & resilience (EU context)
8. **NIST CSF 2.0 (Active)** — Risk & security framework
9. **CIS 18 Controls (Active)** — Foundational security controls
10. **Cyber Essentials (Active)** — Basic cyber hygiene

**Key Cyberday SOC 2 Trust Service Categories Heavily Leveraged:**
- **CC (Common Criteria):** Control environment, risk assessment, monitoring, change management, access controls
- **PI (Processing Integrity):** Data accuracy, availability, completeness
- **Security (C & A):** Confidentiality, availability controls
- **Privacy (P):** Privacy practices, data management, data subject rights
- **Availability (A):** Continuity, recovery

---

**Next Steps:**
1. Load this mapping into your Cyberday system for each control
2. Use the recommended framework filters to pull specific evidence documents
3. Cross-reference task assignments in Cyberday to ensure all required evidence is captured
4. Track completion status for each evidence element per control
5. Prepare audit evidence package for ISAE 3000 Type 1 review

