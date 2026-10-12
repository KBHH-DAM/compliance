# ISO 27001:2022 to ISAE 3000 Control Mapping

**Prepared for:** Elumi  
**Framework:** ISAE 3000 Type 1 Audit for ISO 27001:2022 Compliance  
**Primary Reference:** ISO/IEC 27001:2022 — 93 Annex A controls in 4 themes (A.5 Organisational, A.6 People, A.7 Physical, A.8 Technological)  
**Secondary Framework:** SOC 2, GDPR, NIST CSF  
**Date:** 2026-10-02

---

## Overview: ISO 27001:2022 Coverage

ISO/IEC 27001:2022 Annex A defines **93 controls** organised into **4 themes**:

| Theme | Controls | Scope |
|---|---|---|
| **A.5 — Organisational** | 37 | Policies, roles, asset management, access control, supplier relationships, incident management, compliance |
| **A.6 — People** | 8 | Screening, terms of employment, awareness and training, remote working, event reporting |
| **A.7 — Physical** | 14 | Perimeters, entry, equipment, storage media, utilities, cabling, disposal |
| **A.8 — Technological** | 34 | Endpoints, authentication, malware, vulnerabilities, configuration, logging, networks, cryptography, secure development, change management |

The 2022 revision replaced the 14 clause groups (A.5–A.18) and 114 controls of
ISO/IEC 27001:2013 with these 4 themes and 93 controls. **There is no A.9–A.18
in the 2022 revision**, so any reference such as A.9.2, A.11.1, A.12.4, A.13.1,
A.14.2 or A.17.1 is 2013 numbering and must be restated against the 2022 set.

The numbered *categories* used in the sections below are this document's own
functional grouping for mapping purposes — they are **not** part of the standard.
Each category heading states how many Annex A controls that section assesses:

1. **Governance** - Policies, roles, segregation of duties
2. **Asset Management** - Inventory, acceptable use, return of assets
3. **Access Management** - Access control, identity, authentication, supplier relationships
4. **Information Protection** - Incident planning, endpoints, authentication
5. **Physical Security** - Perimeters, entry, facilities, equipment
6. **Legal & Compliance** - Requirements, IP rights, records
7. **Human Resource Security** - Screening, training, responsibilities
8. **System & Network Security** - Malware protection, networks
9. **Secure Configuration** - Configuration management, privileged utilities
10. **Application Security** - SDLC, requirements, architecture
11. **Threat & Vulnerability Management** - Vulnerability management
12. **Information Security Event Management** - Assessment, response, learning
13. **Continuity Management** - Disruption, readiness, capacity
14. **ISMS Foundation (Clause 4)** - Organization, context, scope — management-system requirements, not Annex A controls

---

## Alignment Model

**ISO 27001:2022** provides the detailed security controls framework.  
**ISAE 3000** defines audit requirements for data processors.  
**Mapping approach:** Each ISO control → Related ISAE control(s) → Supporting evidence.

---

## CATEGORY 1: GOVERNANCE (8 Controls)

### ISO 27001 A.5.1 - Policies for Information Security
**ISAE Control:** C.1 - Info Security Policy & Approval  
**Alignment:** HIGH  
**Requirement:** 
- Policies for information security established, documented, and communicated
- Policies reviewed and updated regularly
- ISAE requires: Documented policy, management approval, annual review

### ISO 27001 A.5.2 - Information Security Roles and Responsibilities
**ISAE Control:** C.1, C.3  
**Alignment:** HIGH  
**Requirement:**
- Security roles assigned and responsibilities defined
- Communication of roles to relevant staff
- ISAE requires: Organizational responsibility structure, screening requirements

### ISO 27001 A.5.3 - Segregation of Duties
**ISAE Control:** B.6, B.13  
**Alignment:** MEDIUM  
**Requirement:**
- Segregation of duties defined to prevent conflicts
- Implemented through role separation
- ISAE requires: Access control with business justification

### ISO 27001 A.5.4 - Management Responsibilities
**ISAE Control:** C.1  
**Alignment:** HIGH  
**Requirement:**
- Management accountability for information security
- Resource allocation for security
- ISAE requires: Management approval of policies

### ISO 27001 A.5.5 - Contact with Authorities
**ISAE Control:** I.1, I.4  
**Alignment:** MEDIUM  
**Requirement:**
- Contact information maintained for authorities
- Cooperation with regulatory bodies
- ISAE requires: Breach notification procedures (Art 31 gap)

### ISO 27001 A.5.6 - Contact with Special Interest Groups
**ISAE Control:** —  
**Alignment:** LOW/NOT COVERED  
**Requirement:**
- Engagement with industry groups, security research
- ISAE scope: Not processor operational control

### ISO 27001 A.5.7 - Threat Intelligence
**ISAE Control:** B.11  
**Alignment:** MEDIUM  
**Requirement:**
- Use threat intelligence for security measures
- Vulnerability management based on threats
- ISAE requires: Vulnerability scanning and pen testing

### ISO 27001 A.8.24 - Use of Cryptography
*Previously listed as "A.5.8 - Use of Cryptography". A.5.8 in the 2022 revision is
"Information security in project management"; use of cryptography is A.8.24 (Technological
theme). Retained in this category for continuity with the existing ISAE mapping.*

**ISAE Control:** B.8  
**Alignment:** HIGH  
**Requirement:**
- Cryptographic controls for confidentiality/integrity
- Encryption for sensitive data
- ISAE requires: Encryption for internet/email transfers

---

## CATEGORY 2: ASSET MANAGEMENT (6 Controls)

### ISO 27001 A.5.9 - Inventory of Information and Other Associated Assets
**ISAE Control:** B.3, B.7  
**Alignment:** HIGH  
**Requirement:**
- Inventory of information assets
- Record of storage locations and systems
- ISAE requires: Inventory of systems processing personal data

### ISO 27001 A.5.10 - Acceptable Use of Information and Other Associated Assets
**ISAE Control:** B.10  
**Alignment:** MEDIUM  
**Requirement:**
- Rules for appropriate use of assets
- Enforcement of acceptable use policy
- ISAE requires: Pseudonymization in dev/test environments

### ISO 27001 A.5.11 - Return of Assets
**ISAE Control:** C.5  
**Alignment:** HIGH  
**Requirement:**
- Procedures for asset return on departure
- Verification of return
- ISAE requires: Employee offboarding with asset return

### ISO 27001 A.5.12 - Classification of Information
**ISAE Control:** A.1, E.1  
**Alignment:** MEDIUM  
**Requirement:**
- Information classified by protection needs
- Classification guide and criteria
- ISAE requires: Processing activity classification

### ISO 27001 A.5.13 - Labelling of Information
**ISAE Control:** —  
**Alignment:** LOW/NOT COVERED  
**Requirement:**
- Labels indicating information classification
- ISAE scope: Not specific procedural requirement

### ISO 27001 A.5.34 - Privacy and Protection of PII
**ISAE Control:** All controls (privacy principle)  
**Alignment:** HIGH  
**Requirement:**
- Privacy requirements met
- Data subject rights supported
- ISAE requires: All controls aligned with privacy

---

## CATEGORY 3: ACCESS MANAGEMENT (8 Controls)

### ISO 27001 A.5.15 - Access Control
**ISAE Control:** B.6, B.13, B.14  
**Alignment:** HIGH  
**Requirement:**
- Access granted based on need
- Least privilege principle
- MFA for high-risk access
- Periodic access review

### ISO 27001 A.5.16 - Identity Management
**ISAE Control:** B.6, C.4  
**Alignment:** HIGH  
**Requirement:**
- User identity uniquely identified
- Identity provisioning/deprovisioning
- Onboarding and offboarding procedures

### ISO 27001 A.5.17 - Authentication Information
**ISAE Control:** B.14  
**Alignment:** HIGH  
**Requirement:**
- Strong authentication credentials
- Two-factor authentication for sensitive access
- Password management

### ISO 27001 A.5.18 - Access Rights
**ISAE Control:** H.2  
**Alignment:** HIGH  
**Requirement:**
- User rights defined and documented
- Access rights appropriate to role
- Support for data subject access rights

### ISO 27001 A.5.19 - Information Security in Supplier Relationships
**ISAE Control:** F.1, F.2, F.6  
**Alignment:** HIGH  
**Requirement:**
- Security requirements in supplier contracts
- Supplier risk assessment
- Ongoing supplier monitoring

### ISO 27001 A.5.20 - Addressing Information Security Within Supplier Agreements
**ISAE Control:** F.4  
**Alignment:** HIGH  
**Requirement:**
- Security clauses in supplier agreements
- Obligations equivalent to organization's
- SLA and remediation procedures

### ISO 27001 A.5.21 - Managing Information Security in the ICT Supply Chain
**ISAE Control:** F.2, F.3  
**Alignment:** HIGH  
**Requirement:**
- Sub-processor authorization and monitoring
- Change notification for supply chain changes
- Documented sub-processor agreements

### ISO 27001 A.5.22 - Monitoring, Review and Change Management of Supplier Services
**ISAE Control:** F.6  
**Alignment:** HIGH  
**Requirement:**
- Regular monitoring of supplier performance
- Risk assessment of suppliers
- Review and remediation of issues

---

## CATEGORY 4: INFORMATION PROTECTION (7 Controls)

### ISO 27001 A.5.23 - Information Security for Use of Cloud Services
**ISAE Control:** E.1, E.2  
**Alignment:** HIGH  
**Requirement:**
- Cloud service assessment before use
- Data location and residency requirements
- Processor responsibilities in cloud

### ISO 27001 A.5.24 - Information Security Incident Management Planning and Preparation
**ISAE Control:** I.1, I.2  
**Alignment:** HIGH  
**Requirement:**
- Incident response plan
- Roles and responsibilities
- Detection and escalation procedures

### ISO 27001 A.5.25 - Assessment and Decision on Information Security Events
**ISAE Control:** I.2, I.3  
**Alignment:** HIGH  
**Requirement:**
- Assessment of security events
- Classification of incidents
- Decision to report or escalate

### ISO 27001 A.5.26 - Response to Information Security Incidents
**ISAE Control:** I.1, I.3  
**Alignment:** HIGH  
**Requirement:**
- Incident response actions
- Containment and remediation
- Timely notification (24-hour requirement)

### ISO 27001 A.5.27 - Learning from Information Security Incidents
**ISAE Control:** I.1, I.4  
**Alignment:** MEDIUM  
**Requirement:**
- Post-incident review and learning
- Preventive measures based on lessons
- Communication of learnings

### ISO 27001 A.8.1 - User Endpoint Devices
**ISAE Control:** B.3, B.7  
**Alignment:** MEDIUM  
**Requirement:**
- Protection of endpoint devices
- Malware protection and monitoring
- Inventory and configuration control

### ISO 27001 A.8.5 - Secure Authentication (including remote access)
*Previously listed as "A.8.2 - User Authentication for External Connections", which is not
a 2022 control title (A.8.2 is Privileged access rights). Remote-working aspects are also
covered by A.6.7 Remote working (Category 7).*

**ISAE Control:** B.14  
**Alignment:** HIGH  
**Requirement:**
- Strong authentication for remote access
- MFA requirement
- Secure VPN/remote access protocols

---

## CATEGORY 5: PHYSICAL SECURITY (11 Controls)

### ISO 27001 A.7.1 - Physical Security Perimeters
**ISAE Control:** B.15  
**Alignment:** HIGH  
**Requirement:**
- Physical security perimeter for facilities
- Barriers and fencing
- Access control at perimeter

### ISO 27001 A.7.2 - Physical Entry
*Consolidation note: the 2022 revision merged 2013 A.11.1.6 "Delivery and loading areas"
into A.7.2 Physical entry, so the delivery and loading requirements below were previously
carried as a separate section numbered A.7.7. A.7.7 in the 2022 revision is "Clear desk and
clear screen", which this document does not yet assess — see the gap list in the coverage
summary.*

**ISAE Control:** B.15  
**Alignment:** HIGH  
**Requirement:**
- Authorization required for physical access
- Visitor management procedures
- Badge and key control
- Segregation of delivery and loading areas from secure areas
- Control and inspection of incoming and outgoing materials

### ISO 27001 A.7.3 - Securing Offices, Rooms and Facilities
**ISAE Control:** B.15  
**Alignment:** HIGH  
**Requirement:**
- Physical protection of equipment
- Secure storage of assets
- Environmental controls (power, cooling)

### ISO 27001 A.7.4 - Physical Security Monitoring
**ISAE Control:** B.7, B.15  
**Alignment:** HIGH  
**Requirement:**
- CCTV monitoring
- Intrusion detection
- Audit trails of physical access

### ISO 27001 A.7.5 - Protecting Against Physical and Environmental Threats
**ISAE Control:** B.15  
**Alignment:** MEDIUM  
**Requirement:**
- Protection from fire, flood, earthquake
- Environmental hazard mitigation
- Business continuity planning

### ISO 27001 A.7.6 - Working in Secure Areas
**ISAE Control:** B.15  
**Alignment:** LOW/NOT COVERED  
**Requirement:**
- Clean desk policy
- Visitor escort requirements
- ISAE scope: General practice, not specific control

### ISO 27001 A.7.10 - Storage Media
**ISAE Control:** B.8, B.9  
**Alignment:** MEDIUM  
**Requirement:**
- Procedures for removable media use
- Encryption of removable media
- Audit and tracking of media

### ISO 27001 A.7.11 - Supporting Utilities
**ISAE Control:** B.1, E.1  
**Alignment:** MEDIUM  
**Requirement:**
- Redundant power supplies
- Backup power for critical systems
- Environmental monitoring

### ISO 27001 A.7.12 - Cabling Security
**ISAE Control:** B.4, B.5  
**Alignment:** MEDIUM  
**Requirement:**
- Protection of data cables
- Segregation from power cables
- Cable management practices

### ISO 27001 A.7.13 / A.7.14 - Equipment Maintenance; Secure Disposal or Re-use of Equipment
*Previously listed as "A.8.6 - Acquisition, Installation, Replacement and Removal of
Equipment", which is not a 2022 control (A.8.6 is Capacity management). The 2013 controls
A.11.2.4 and A.11.2.7 map to A.7.13 and A.7.14 respectively. The "installation control"
element below relates to A.8.19 Installation of software on operational systems
(Category 9) rather than to physical equipment.*

**ISAE Control:** B.12, B.15  
**Alignment:** MEDIUM  
**Requirement:**
- Equipment lifecycle management
- Installation control
- Secure removal of equipment
- Data sanitization before disposal

---

## CATEGORY 6: LEGAL & COMPLIANCE (3 Controls)

### ISO 27001 A.5.31 - Legal, Statutory, Regulatory and Contractual Requirements
**ISAE Control:** A.1, A.2  
**Alignment:** HIGH  
**Requirement:**
- Identification of legal requirements
- Compliance monitoring
- Documentation of requirements alignment

### ISO 27001 A.5.32 - Intellectual Property Rights
**ISAE Control:** —  
**Alignment:** LOW/NOT COVERED  
**Requirement:**
- Protection of organization's IP
- ISAE scope: Not processor operational control

### ISO 27001 A.5.33 - Protection of Records
**ISAE Control:** D.1, D.2  
**Alignment:** HIGH  
**Requirement:**
- Retention of records
- Protection from damage/loss
- Secure destruction

---

## CATEGORY 7: HUMAN RESOURCE SECURITY (7 Controls)

### ISO 27001 A.6.1 - Screening
**ISAE Control:** C.3  
**Alignment:** HIGH  
**Requirement:**
- Background screening before employment
- Reference checks
- Criminal record verification

### ISO 27001 A.6.2 - Terms and Conditions of Employment
**ISAE Control:** C.4  
**Alignment:** HIGH  
**Requirement:**
- Security responsibilities in employment terms
- Confidentiality agreements
- Acceptable use policies

### ISO 27001 A.6.3 - Information Security Awareness, Education and Training
**ISAE Control:** C.7  
**Alignment:** HIGH  
**Requirement:**
- Regular security awareness training
- Training on policies and procedures
- Record of training completion

### ISO 27001 A.6.4 - Disciplinary Process
**ISAE Control:** —  
**Alignment:** LOW/NOT COVERED  
**Requirement:**
- Procedures for security violations
- ISAE scope: Organizational policy, not operational control

### ISO 27001 A.6.5 - Responsibilities after Termination or Change of Employment
**ISAE Control:** C.5, C.6  
**Alignment:** HIGH  
**Requirement:**
- Access removal on departure
- Continuation of confidentiality obligations
- Return of assets

### ISO 27001 A.6.6 - Confidentiality or Non-Disclosure Agreements
**ISAE Control:** C.4, C.6  
**Alignment:** HIGH  
**Requirement:**
- Signed confidentiality agreements
- Coverage of post-employment obligations
- Enforcement mechanisms

### ISO 27001 A.6.7 - Remote Working
**ISAE Control:** B.4, B.8, B.14  
**Alignment:** MEDIUM  
**Requirement:**
- Security for remote workers
- VPN requirements
- MFA for remote access

---

## CATEGORY 8: SYSTEM & NETWORK SECURITY (6 Controls)

### ISO 27001 A.8.7 - Protection Against Malware
**ISAE Control:** B.3  
**Alignment:** HIGH  
**Requirement:**
- Antivirus/anti-malware software
- Regular updates
- Malware detection and response

### ISO 27001 A.8.20 - Networks Security
**ISAE Control:** B.4, B.5  
**Alignment:** HIGH  
**Requirement:**
- Firewall protection
- Network segmentation
- Intrusion detection/prevention

### ISO 27001 A.8.21 - Security of Network Services
**ISAE Control:** B.4, B.8  
**Alignment:** MEDIUM  
**Requirement:**
- Security parameters in network services
- Encrypted communications
- Service availability protection

### ISO 27001 A.8.22 - Segregation of Networks
**ISAE Control:** B.5  
**Alignment:** HIGH  
**Requirement:**
- Network segmentation
- Isolation of sensitive networks
- VLANs and separate segments

### ISO 27001 A.8.23 - Web Filtering
**ISAE Control:** —  
**Alignment:** LOW/NOT COVERED  
**Requirement:**
- Control of web access
- ISAE scope: General practice, not specific control

### ISO 27001 A.8.14 - Redundancy of Information Processing Facilities
**ISAE Control:** B.1  
**Alignment:** MEDIUM  
**Requirement:**
- Redundancy for critical systems
- Failover capabilities
- Business continuity

---

## CATEGORY 9: SECURE CONFIGURATION (4 Controls)

### ISO 27001 A.8.9 - Configuration Management
**ISAE Control:** B.12  
**Alignment:** HIGH  
**Requirement:**
- Documented baselines
- Change control process
- Configuration tracking

### ISO 27001 A.8.10 - Information Deletion
**ISAE Control:** D.1, D.3  
**Alignment:** HIGH  
**Requirement:**
- Secure data deletion procedures
- Confirmation of deletion
- Proper disposal of media

### ISO 27001 A.8.18 - Use of Privileged Utility Programs
**ISAE Control:** B.13, B.14  
**Alignment:** HIGH  
**Requirement:**
- Restriction of privileged utilities
- Logging of privileged access
- Audit of utility use

### ISO 27001 A.8.19 - Installation of Software on Operational Systems
**ISAE Control:** B.12  
**Alignment:** HIGH  
**Requirement:**
- Software installation controls
- Approval requirements
- Configuration management

---

## CATEGORY 10: APPLICATION SECURITY (7 Controls)

### ISO 27001 A.8.25 - Secure Development Life Cycle
**ISAE Control:** B.10  
**Alignment:** MEDIUM  
**Requirement:**
- Security in development process
- Design review
- Testing before deployment

### ISO 27001 A.8.26 - Application Security Requirements
**ISAE Control:** B.10  
**Alignment:** MEDIUM  
**Requirement:**
- Security requirements in application design
- Input validation
- Output encoding

### ISO 27001 A.8.27 - Secure System Architecture and Engineering Principles
**ISAE Control:** B.1  
**Alignment:** MEDIUM  
**Requirement:**
- Secure design principles
- Least privilege in application design
- Separation of concerns

### ISO 27001 A.8.28 - Secure Coding
**ISAE Control:** B.10  
**Alignment:** MEDIUM  
**Requirement:**
- Coding standards for security
- Code review processes
- Vulnerability prevention

### ISO 27001 A.8.31 - Separation of Development, Test and Production Environments
**ISAE Control:** B.10  
**Alignment:** HIGH  
**Requirement:**
- Separation of dev/test/prod environments
- Data pseudonymization in dev/test
- Access control per environment

### ISO 27001 A.8.32 - Change Management
**ISAE Control:** B.12  
**Alignment:** MEDIUM  
**Requirement:**
- Platform change procedures
- Testing of changes
- Rollback procedures

### ISO 27001 A.8.16 - Monitoring Activities
*Previously listed as "A.8.32 - Monitoring and Reviewing". A.8.32 in the 2022 revision is
Change management; monitoring is A.8.16. Related logging requirements fall under A.8.15
Logging, which this document does not yet assess.*

**ISAE Control:** B.7, B.11  
**Alignment:** MEDIUM  
**Requirement:**
- Application security monitoring
- Log review and analysis
- Performance monitoring

---

## CATEGORY 11: THREAT & VULNERABILITY MANAGEMENT (1 Control — A.5.7 Threat intelligence is covered under Category 1)

### ISO 27001 A.8.8 - Management of Technical Vulnerabilities
**ISAE Control:** B.11  
**Alignment:** HIGH  
**Requirement:**
- Vulnerability scanning
- Penetration testing
- Patch management
- Remediation of findings

---

## CATEGORY 12: INFORMATION SECURITY EVENT MANAGEMENT (3 Controls — cross-referenced from Category 4)

### ISO 27001 A.5.25 - Assessment and Decision on Information Security Events
**ISAE Control:** I.2, I.3  
**Alignment:** HIGH  

### ISO 27001 A.5.26 - Response to Information Security Incidents
**ISAE Control:** I.1, I.3  
**Alignment:** HIGH  

### ISO 27001 A.5.27 - Learning from Information Security Incidents
**ISAE Control:** I.1, I.4  
**Alignment:** MEDIUM  

(See detailed descriptions in Category 4)

---

## CATEGORY 13: CONTINUITY MANAGEMENT (3 Controls)

### ISO 27001 A.5.29 - Information Security During Disruption
**ISAE Control:** —  
**Alignment:** LOW/NOT COVERED  
**Requirement:**
- Continuity of processing during incidents
- ISAE scope: Business continuity planning, not processor operational

### ISO 27001 A.5.30 - ICT Readiness for Business Continuity
**ISAE Control:** —  
**Alignment:** LOW/NOT COVERED  
**Requirement:**
- Redundancy and recovery capabilities
- ISAE scope: Infrastructure planning

### ISO 27001 A.8.6 - Capacity Management
**ISAE Control:** —  
**Alignment:** LOW/NOT COVERED  
**Requirement:**
- Monitoring of resource capacity
- ISAE scope: Infrastructure management

---

## CATEGORY 14: ISMS FOUNDATION (Clause 4 — management-system requirements, not Annex A controls)

These are requirements of ISO/IEC 27001:2022 **Clause 4**, not Annex A controls. They are foundational to the ISMS but are management-system requirements rather than operational security controls, and are therefore excluded from the 93-control Annex A counts below.

### ISO 27001 Clause 4.1 - Understanding the Organization and its Context
**ISAE Control:** A.1  
**Alignment:** MEDIUM  
**Requirement:**
- Understanding of organization
- Identification of requirements
- Integration with business processes

### ISO 27001 Clause 4.2 - Understanding the Needs and Expectations of Interested Parties
**ISAE Control:** —  
**Alignment:** LOW  
**Requirement:**
- Identification of stakeholders
- Understanding of needs
- ISAE scope: Organizational governance

### ISO 27001 Clause 4.3 - Determining the Scope of the ISMS
**ISAE Control:** A.1, E.1  
**Alignment:** MEDIUM  
**Requirement:**
- Definition of ISMS scope
- Documented boundaries
- Processing activities

(Remaining Clause 5–10 requirements are management-system requirements, not Annex A controls)

---

## CATEGORY 15: SoA COMPLETION PASS — THE 22 PREVIOUSLY UNASSESSED CONTROLS

ISO/IEC 27001:2022 clause 6.1.3(d) requires the Statement of Applicability to address **all
93** Annex A controls. The 22 controls below had no entry in this document; they are assessed
here against the same 45-control ISAE 3000 set and the same HIGH / MEDIUM / LOW alignment
scale used above, so that the coverage figures now cover the full Annex A.

**Scope of this assessment:** these entries map each Annex A control to the ISAE 3000
control(s) that address it. They do **not** state whether the control is implemented at
Elumi. A Statement of Applicability additionally needs, per control, an
inclusion/exclusion decision, a justification, implementation status and an owner — those
are management's to supply and are not asserted here.

They are grouped by Annex A theme rather than by this document's functional categories, to
keep the completion pass auditable as one block.

---

### Theme A.5 — Organisational (6 controls)

### ISO 27001 A.5.8 - Information Security in Project Management
**ISAE Control:** B.2, B.10, B.12
**Alignment:** MEDIUM
**Requirement:**
- Information security integrated into project and change management
- Security requirements identified at project initiation
- ISAE requires: risk assessment driving technical measures (B.2), pseudonymised data in
  development and testing (B.10), and change procedures (B.12) — but no explicit
  project-management control
- Applicable: Elumi develops software and runs a DPIA per release, so security in project
  management is in scope

### ISO 27001 A.5.14 - Information Transfer
**ISAE Control:** B.8, E.1, E.2, G.1, G.2, G.3
**Alignment:** HIGH
**Requirement:**
- Rules, procedures and agreements for transferring information
- Protection of information in transit
- ISAE requires: encryption for internet and email transfers (B.8), storage and processing
  locations per the DPA (E.1, E.2), and documented third-country transfer basis (G.1–G.3)
- Already cited as the 2022 control for ISAE E.1, E.2 and G.1 in the two mapping documents

### ISO 27001 A.5.28 - Collection of Evidence
**ISAE Control:** B.9, I.2, I.4
**Alignment:** MEDIUM
**Requirement:**
- Procedures for identifying, collecting and preserving evidence of information security events
- ISAE requires: logging of admin activity and security events (B.9), log review to identify
  breaches (I.2), and documentation of breach nature, consequences and measures for the
  supervisory authority report (I.4)
- Gap: ISAE does not require forensic evidence-handling or chain-of-custody procedures

### ISO 27001 A.5.35 - Independent Review of Information Security
**ISAE Control:** The ISAE 3000 engagement itself; C.1
**Alignment:** MEDIUM
**Requirement:**
- Independent review of the information security approach at planned intervals
- ISAE position: **the ISAE 3000 Type 1 report is itself an independent external review** and
  is the strongest available evidence for this control
- Gap: a Type 1 report is point-in-time. A.5.35 expects reviews at planned intervals, so
  recurring engagements (or a Type 2) are what sustain this control between reports. The
  annual procedure assessments in A.1, B.1 and C.1 are management reviews, not independent ones

### ISO 27001 A.5.36 - Compliance with Policies, Rules and Standards for Information Security
**ISAE Control:** A.2, C.2, and the annual assessments in A.1, B.1, C.1, D.1, E.1, F.1, G.1, H.1, I.1
**Alignment:** MEDIUM
**Requirement:**
- Regular review that information security policies and standards are complied with
- ISAE requires: processing only per controller instructions (A.2), management verification
  that the policy does not conflict with the DPAs (C.2), and annual assessment of every
  documented procedure
- Distinction: the ISAE annual assessments review whether *procedures need updating*, which
  is not the same as reviewing whether personnel and processes *comply* with them. Treat the
  compliance-monitoring element as only partly covered

### ISO 27001 A.5.37 - Documented Operating Procedures
**ISAE Control:** A.1, B.1, C.1, D.1, E.1, F.1, G.1, H.1, I.1
**Alignment:** HIGH
**Requirement:**
- Operating procedures documented and made available to those who need them
- ISAE requires **written procedures** for every control family: controller instructions (A.1),
  safeguards (B.1), security policy (C.1), storage and deletion (D.1), storage locations (E.1),
  sub-processors (F.1), third-country transfers (G.1), data subject rights (H.1) and breach
  notification (I.1). This is the most densely covered control in Annex A for this engagement

---

### Theme A.6 — People (1 control)

### ISO 27001 A.6.8 - Information Security Event Reporting
**ISAE Control:** I.1, I.2, I.3, C.7
**Alignment:** HIGH
**Requirement:**
- Mechanism for personnel to report observed or suspected information security events
- ISAE requires: a breach notification procedure (I.1), staff awareness as a breach
  identification control (I.2), notification to the controller within 24 hours (I.3), and
  security awareness training (C.7)

---

### Theme A.7 — Physical (3 controls)

### ISO 27001 A.7.7 - Clear Desk and Clear Screen
**ISAE Control:** B.15 (indirect)
**Alignment:** LOW/NOT COVERED
**Requirement:**
- Clear desk rules for papers and removable media; clear screen rules for information facilities
- ISAE scope: general working practice, not a specific processor control. The A.7.6 "Working
  in Secure Areas" entry above mentions a clean-desk policy in passing, but no ISAE control
  tests it
- Still **applicable** for the SoA — a clear-desk/clear-screen rule is expected in the ISMS
  policy set even though no ISAE control covers it

### ISO 27001 A.7.8 - Equipment Siting and Protection
**ISAE Control:** B.15, F.4, F.6
**Alignment:** MEDIUM
**Requirement:**
- Equipment sited and protected against environmental threats and unauthorised access
- ISAE requires: physical access controls for premises and data centres (B.9 evidence via B.15)
- Note: for Hetzner-hosted infrastructure this is largely a sub-processor control, evidenced
  through F.4 (obligations passed down) and F.6 (sub-processor monitoring), not by Elumi directly.
  On-premises equipment remains Elumi's own

### ISO 27001 A.7.9 - Security of Assets Off-Premises
**ISAE Control:** B.15, C.5
**Alignment:** MEDIUM
**Requirement:**
- Protection of assets used or stored outside the organisation's premises
- ISAE requires: physical access safeguards (B.15) and asset return on departure (C.5)
- Gap: ISAE has no explicit off-premises or remote-working asset control. With remote working
  in scope (A.6.7), laptops and mobile devices off-premises are a real exposure that no ISAE
  control tests
- This control is **no longer used** as the mapping for ISAE E.1/G.1 — those are data-residency
  controls and map to A.5.23 + A.5.14

---

### Theme A.8 — Technological (12 controls)

### ISO 27001 A.8.2 - Privileged Access Rights
**ISAE Control:** B.6, B.9, B.13, B.14
**Alignment:** HIGH
**Requirement:**
- Allocation and use of privileged access rights restricted and managed
- ISAE requires: access limited to work-related need (B.6), logging of admin activities (B.9),
  formalised grant/removal with periodic review (B.13), and two-factor authentication for
  high-risk accounts (B.14)

### ISO 27001 A.8.3 - Information Access Restriction
**ISAE Control:** B.6, B.13
**Alignment:** HIGH
**Requirement:**
- Access to information and other associated assets restricted per the access control policy
- ISAE requires: access to personal data limited to users with a work-related need, with
  periodic review (B.6, B.13)

### ISO 27001 A.8.4 - Access to Source Code
**ISAE Control:** B.6, B.13 (indirect)
**Alignment:** MEDIUM
**Requirement:**
- Read and write access to source code, development tools and software libraries appropriately managed
- ISAE requires: general access restriction (B.6, B.13), but has no source-code-specific control
- Applicable: Elumi is a software developer, so repository and pipeline access is in scope and
  should be covered by the SoA even though no ISAE control tests it

### ISO 27001 A.8.11 - Data Masking
**ISAE Control:** B.10
**Alignment:** HIGH
**Requirement:**
- Data masking in line with the access control policy and applicable legislation
- ISAE requires: personal data in development and testing pseudonymised or anonymised, or
  processed under documented controller agreement (B.10) — a direct match, and the GDPR
  Art. 32(1)(a) pseudonymisation measure

### ISO 27001 A.8.12 - Data Leakage Prevention
**ISAE Control:** B.4, B.5, B.8, B.9
**Alignment:** MEDIUM
**Requirement:**
- Data leakage prevention measures applied to systems, networks and devices processing or storing sensitive information
- ISAE requires: firewall protection (B.4), network segmentation (B.5), encryption of
  transfers (B.8) and logging (B.9), which constrain exfiltration paths
- Gap: no ISAE control requires DLP tooling, egress monitoring or content inspection as such

### ISO 27001 A.8.13 - Information Backup
**ISAE Control:** B.1, B.2 (only generically)
**Alignment:** MEDIUM
**Requirement:**
- Backup copies maintained and tested in accordance with the agreed backup policy
- **Finding: the 45-control ISAE 3000 set has no explicit backup or restore control.** B.1 and
  B.2 cover safeguards and risk-based technical measures generically, which is the only hook
- This is a substantive gap, not just a mapping gap: GDPR Art. 32(1)(c) requires the ability to
  restore availability and access to personal data in a timely manner. Recommend adding backup
  and restore-testing evidence to the engagement even though the ISAE control set does not
  name it

### ISO 27001 A.8.15 - Logging
**ISAE Control:** B.9, B.7
**Alignment:** HIGH
**Requirement:**
- Logs recording activities, exceptions, faults and other relevant events produced, stored,
  protected and analysed
- ISAE requires: logging of admin activities, security incidents, changes to logging itself,
  rights changes and failed logins (B.9), plus monitoring and escalation (B.7) — a direct match

### ISO 27001 A.8.17 - Clock Synchronisation
**ISAE Control:** — (enabler for B.9)
**Alignment:** LOW/NOT COVERED
**Requirement:**
- Clocks of information processing systems synchronised to approved time sources
- ISAE scope: no ISAE control names clock synchronisation
- Still **applicable** for the SoA: synchronised time is what makes the B.9 logs correlatable
  and evidentially useful, so it underpins a control that *is* tested, and A.5.28 evidence
  collection depends on it

### ISO 27001 A.8.29 - Security Testing in Development and Acceptance
**ISAE Control:** B.11, B.10, B.12
**Alignment:** HIGH
**Requirement:**
- Security testing processes defined and implemented in the development life cycle
- ISAE requires: regular vulnerability scans and penetration tests with weaknesses
  addressed (B.11), controlled dev/test data (B.10) and tested changes (B.12)

### ISO 27001 A.8.30 - Outsourced Development
**ISAE Control:** F.1, F.2, F.4, F.6
**Alignment:** MEDIUM — **or excludable; see note**
**Requirement:**
- Direction, monitoring and review of outsourced system development activities
- ISAE requires: sub-processor appointment procedure (F.1), authorisation (F.2), obligations
  passed down (F.4) and risk assessment and monitoring (F.6) — these apply if development is
  outsourced
- **Decision needed:** if Elumi develops entirely in-house with no outsourced development or
  contracted developers, A.8.30 may legitimately be **excluded** from the SoA with that
  justification. If any development is contracted out, it is included and the F-series applies.
  This is the one control of the 22 whose applicability cannot be determined from the documents

### ISO 27001 A.8.33 - Test Information
**ISAE Control:** B.10
**Alignment:** HIGH
**Requirement:**
- Test information appropriately selected, protected and managed
- ISAE requires: personal data in development and testing pseudonymised or anonymised (B.10) —
  a direct match, assessed alongside A.8.11

### ISO 27001 A.8.34 - Protection of Information Systems During Audit Testing
**ISAE Control:** B.11, F.6
**Alignment:** MEDIUM
**Requirement:**
- Audit tests and assurance activities planned and agreed between tester and management to
  protect operational systems
- ISAE requires: vulnerability scanning and penetration testing (B.11), which must be scoped
  and scheduled so as not to disrupt production, and sub-processor audits and inspections (F.6)
- Gap: ISAE does not require a documented agreement on audit-test scope and timing

---

## COVERAGE SUMMARY

> **All 93 ISO/IEC 27001:2022 Annex A controls are now assessed.** Figures are computed from
> the per-control **Alignment** verdicts recorded in this document and were re-derived
> programmatically after the SoA completion pass (Category 15).

### By theme

| Theme | Annex A controls | Assessed | Fully aligned (HIGH) | Partially aligned (MEDIUM) | Not covered by ISAE |
|---|---|---|---|---|---|
| A.5 — Organisational | 37 | 37 | 22 | 10 | 5 |
| A.6 — People | 8 | 8 | 6 | 1 | 1 |
| A.7 — Physical | 14 | 14 | 4 | 8 | 2 |
| A.8 — Technological | 34 | 34 | 17 | 14 | 3 |
| **TOTAL** | **93** | **93** | **49** | **33** | **11** |

### Headline figures

- **82 of 93 Annex A controls (88%)** have an identified ISAE 3000 mapping (HIGH or MEDIUM).
- **49 controls (53%)** map directly to an ISAE control.
- **33 controls (35%)** are partially covered — an ISAE control addresses part of the
  requirement, and the residual element is named in each entry.
- **11 controls (12%)** have no ISAE coverage. These are **not** automatically excludable from
  the Statement of Applicability — see below.

### The 11 controls with no ISAE coverage

| Control | Why no ISAE control covers it | SoA treatment |
|---|---|---|
| A.5.6 Contact with special interest groups | Not a processor operational control | Likely applicable, no ISAE evidence |
| A.5.13 Labelling of information | No ISAE labelling requirement | Applicable if classification is used |
| A.5.29 Information security during disruption | Business continuity, outside processor audit scope | Applicable — GDPR Art. 32(1)(b)/(c) |
| A.5.30 ICT readiness for business continuity | As above | Applicable — GDPR Art. 32(1)(c) |
| A.5.32 Intellectual property rights | Not a processor operational control | Applicable, low risk |
| A.6.4 Disciplinary process | Organisational policy, not operational | Applicable — supports A.6.3 and A.5.36 |
| A.7.6 Working in secure areas | General practice, no specific ISAE control | Applicable |
| A.7.7 Clear desk and clear screen | General practice, no specific ISAE control | Applicable |
| A.8.6 Capacity management | Infrastructure management, outside scope | Applicable — GDPR Art. 32(1)(b) availability |
| A.8.17 Clock synchronisation | Not named by ISAE, but underpins B.9 logging | Applicable — enabler for logging and evidence |
| A.8.23 Web filtering | General practice, no specific ISAE control | Applicable |

**"Not covered by ISAE" is not a justification for exclusion.** The ISAE 3000 engagement and
the ISO 27001 ISMS have different scopes: ISAE tests a processor's contractual obligations to
controllers, while Annex A covers the whole ISMS. A control can be fully applicable and
correctly implemented yet have no ISAE control testing it. Exclusion under clause 6.1.3(d)
requires a risk-based justification, not the absence of an ISAE mapping.

### Substantive gaps found during the completion pass

Three findings are about the **ISAE control set itself**, not about the mapping:

1. **No backup or restore control.** The 45-control ISAE set has no explicit backup control,
   yet GDPR Art. 32(1)(c) requires the ability to restore availability and access to personal
   data in a timely manner. A.8.13 maps only to the generic B.1/B.2 safeguards. **Recommend
   adding backup and restore-testing evidence to the engagement.**
2. **No off-premises asset control.** A.7.9 has no ISAE counterpart, while remote working
   (A.6.7) is in scope — so laptops and mobile devices outside the premises are an exposure
   that no ISAE control tests.
3. **Availability generally is thin.** A.5.29, A.5.30, A.8.6 and A.8.13 all sit outside ISAE
   coverage, which together leave the GDPR Art. 32(1)(b)–(c) availability and resilience
   obligations largely unevidenced by this engagement.

### What this does and does not establish

These entries map Annex A controls to the ISAE controls that address them. They do **not**
assert that any control is implemented at Elumi. Clause 6.1.3(d) requires the SoA to record,
per control: the inclusion or exclusion decision, the justification, implementation status and
an owner. **That remains outstanding and is management's to supply.** One applicability
question cannot be answered from these documents: **A.8.30 Outsourced development** is
excludable if all development is in-house, and included if any is contracted out.

---

## Key Findings

### Coverage: 88% of Annex A mapped to an ISAE control

**Fully aligned (49 controls — 53%)**
- Core processor obligations map directly: documented procedures, access control, supplier
  management, incident response, logging, HR security, cryptography, test data
- A.5.37 Documented operating procedures is the most densely covered control in Annex A —
  nine ISAE controls require written procedures

**Partially aligned (33 controls — 35%)**
- An ISAE control addresses part of the requirement; each entry names what is left over
- Examples: A.5.28 (evidence collection — no chain-of-custody requirement), A.8.12 (no DLP
  tooling requirement), A.5.36 (procedure review is not compliance monitoring)

**Not covered by ISAE (11 controls — 12%)**
- Listed above with SoA treatment. Mostly business continuity, general working practices and
  organisational policy — applicable controls that this engagement simply does not test

### Notable mapping outcomes

- **A.5.35 Independent review of information security** is satisfied in part by the ISAE 3000
  engagement itself, which is the strongest available evidence for it. A Type 1 report is
  point-in-time, so recurring engagements (or a Type 2) are what sustain the control.
- **A.8.11 Data masking** and **A.8.33 Test information** both map directly to ISAE B.10, which
  is also the GDPR Art. 32(1)(a) pseudonymisation measure — one control objective satisfying
  three framework requirements.
- **A.7.8 Equipment siting** is largely a sub-processor control for Hetzner-hosted
  infrastructure, evidenced through F.4 and F.6 rather than directly.

---

## Mapping ISO 27001:2022 → ISAE 3000 Controls

### Direct Mappings (Highest Confidence)

| ISO 27001 Control | ISAE Control | Alignment |
|---|---|---|
| A.5.1 (Policies) | C.1 | 1:1 |
| A.5.15 (Access) | B.6, B.13, B.14 | 1:3 |
| A.6.1 (Screening) | C.3 | 1:1 |
| A.6.3 (Training) | C.7 | 1:1 |
| A.6.5-6 (Termination) | C.5, C.6 | 1:2 |
| A.5.19-22 (Suppliers) | F.1-F.6 | 1:6 |
| A.7.1-4 (Physical) | B.15 | 1:1 |
| A.8.7 (Malware) | B.3 | 1:1 |
| A.8.20-22 (Network) | B.4, B.5 | 1:2 |
| A.8.9, 18-19 (Config) | B.12 | 1:3 |
| A.8.8 (Vulnerabilities) | B.11 | 1:1 |
| A.5.24-27 (Incidents) | I.1-I.4 | 1:4 |

---

## Recommendations

### For ISAE 3000 Audit Using ISO 27001:2022

1. **Use ISO controls as supplementary documentation**
   - More detailed than ISAE requirements
   - Provides best-practice guidance
   - Evidence of ISO compliance supports ISAE audit

2. **Map ISO controls to ISAE controls**
   - 82 of 93 Annex A controls (88%) have an identified ISAE mapping
   - 11 controls have no ISAE coverage but remain applicable to the ISMS

3. **Evidence cross-referencing**
   - ISO 27001 audit evidence can support ISAE requirements
   - Vice versa: ISAE evidence can demonstrate ISO compliance

4. **Gap identification**
   - All 93 Annex A controls are assessed (clause 6.1.3(d) basis complete for *mapping*)
   - 11 controls have no ISAE coverage — applicable to the ISMS but untested by this
     engagement; absence of an ISAE mapping is not a justification for exclusion
   - Three substantive gaps in the ISAE control set itself: no backup/restore control, no
     off-premises asset control, and thin availability coverage overall (see Coverage Summary)
   - **Outstanding:** per-control inclusion/exclusion decision, justification, implementation
     status and owner — management's to supply. A.8.30 applicability needs confirming

---

**Document Version:** 1.2  
**Last Updated:** 2026-10-12  
**Change in v1.1:** Annex A references restated against ISO/IEC 27001:2022 (2013 numbering removed); control-set facts and coverage figures recomputed on the 93-control / 4-theme basis.  
**Change in v1.2:** The 22 previously unassessed Annex A controls assessed (Category 15); all 93 controls now covered; coverage recomputed at 82 of 93 (88%) mapped.  
**Next Review:** 2027-10-02

