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

## COVERAGE SUMMARY

> **Recomputed against the ISO/IEC 27001:2022 Annex A control set (93 controls, 4 themes).**
> The figures previously shown here ("116 controls", "95% coverage", "110 of 116") were
> derived from a 15-category / 116-control taxonomy that does not exist in the 2022
> revision. The table below counts **distinct Annex A controls** and uses the per-control
> **Alignment** verdicts already recorded in the sections above — no verdicts were added
> or changed.

### By theme

| Theme | Annex A controls | Assessed here | Fully aligned (HIGH) | Partially aligned (MEDIUM) | Not covered | Not yet assessed |
|---|---|---|---|---|---|---|
| A.5 — Organisational | 37 | 31 | 20 | 6 | 5 | 6 |
| A.6 — People | 8 | 7 | 5 | 1 | 1 | 1 |
| A.7 — Physical | 14 | 11 | 4 | 6 | 1 | 3 |
| A.8 — Technological | 34 | 22 | 11 | 9 | 2 | 12 |
| **TOTAL** | **93** | **71** | **40** | **22** | **9** | **22** |

### Headline figures

- **62 of 93 Annex A controls (67%)** have an identified ISAE 3000 mapping (HIGH or MEDIUM alignment).
- Of the **71 controls assessed** in this document, **62 (87%)** map to an ISAE control.
- **9 controls (10% of 93)** are assessed as outside ISAE processor-audit scope.
- **22 controls (24% of 93)** are **not yet assessed** in this document — see the gap list below.

### Annex A controls not yet assessed in this document (22)

| Theme | Controls |
|---|---|
| A.5 — Organisational | A.5.8 Information security in project management; A.5.14 Information transfer; A.5.28 Collection of evidence; A.5.35 Independent review of information security; A.5.36 Compliance with policies, rules and standards; A.5.37 Documented operating procedures |
| A.6 — People | A.6.8 Information security event reporting |
| A.7 — Physical | A.7.7 Clear desk and clear screen; A.7.8 Equipment siting and protection; A.7.9 Security of assets off-premises |
| A.8 — Technological | A.8.2 Privileged access rights; A.8.3 Information access restriction; A.8.4 Access to source code; A.8.11 Data masking; A.8.12 Data leakage prevention; A.8.13 Information backup; A.8.15 Logging; A.8.17 Clock synchronisation; A.8.29 Security testing in development and acceptance; A.8.30 Outsourced development; A.8.33 Test information; A.8.34 Protection of information systems during audit testing |

Several of these controls *are* covered by ISAE controls elsewhere in this documentation
set — for example A.5.14 under ISAE E.1/G.1, A.8.13 under the B-series backup
control, A.8.15 under B.7/B.9, A.8.2 under B.14, and A.8.33 under B.10 — but they have no
dedicated entry in this mapping. **These 22 entries must be completed before the coverage
figure above is treated as final.**

---

## Key Findings

### Coverage: 67% of Annex A mapped, 24% not yet assessed

**Fully aligned (40 controls — 43% of 93)**
- Core operational security controls have direct ISAE 3000 equivalents
- Strong alignment on: access control, supplier management, incident response, policies, HR security

**Partially aligned (22 controls — 24% of 93)**
- Supportive ISAE equivalents exist but not one-to-one
- Examples: application security (A.8.25–A.8.28 → ISAE B.10), physical equipment controls (A.7.10–A.7.14 → ISAE B.15)

**Not covered (9 controls — 10% of 93)**
- Primarily organisational governance and infrastructure planning: A.5.6, A.5.13, A.5.29, A.5.30, A.5.32, A.6.4, A.7.6, A.8.6, A.8.23
- Assessed as outside ISAE processor-audit scope

**Not yet assessed (22 controls — 24% of 93)**
- Listed above; required to complete the Statement of Applicability basis

> **Note for the Statement of Applicability:** ISO/IEC 27001:2022 clause 6.1.3(d) requires
> the SoA to address **all 93** Annex A controls with an inclusion/exclusion justification.
> The 22 unassessed controls above are therefore mandatory gaps to close, not optional.

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
   - 62 of 93 Annex A controls (67%) currently have an identified ISAE mapping
   - 9 controls are assessed as out of processor-audit scope

3. **Evidence cross-referencing**
   - ISO 27001 audit evidence can support ISAE requirements
   - Vice versa: ISAE evidence can demonstrate ISO compliance

4. **Gap identification**
   - 9 out-of-scope Annex A controls are correctly not covered by ISAE — these are
     organisational governance and infrastructure planning, not processor operational controls
   - 22 Annex A controls are **not yet assessed** in this mapping and must be added before
     the Statement of Applicability is complete (clause 6.1.3(d) requires all 93)

---

**Document Version:** 1.1  
**Last Updated:** 2026-10-12  
**Change in v1.1:** Annex A references restated against ISO/IEC 27001:2022 (2013 numbering removed); control-set facts and coverage figures recomputed on the 93-control / 4-theme basis.  
**Next Review:** 2027-10-02

