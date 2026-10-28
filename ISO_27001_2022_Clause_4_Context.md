# ISO/IEC 27001:2022 — Clause 4: Context of the Organization

**Entity:** Data & More ApS
**ISMS:** Information Security Management System (maintained in Cyberday)
**Document owner:** Compliance Lead
**Approved by:** Management
**Version:** 0.2 draft — [Approval date]
**Reconciled against:** *ISMS description and scope — Report — Cyberday*, Version #5, 28.09.2026 (author: Kristian Boe Helweg Hansen)
**Review:** Annually, at management review (clause 9.3), or on trigger

> Clause 4.1 and 4.2 do not require a documented procedure. They do require that the determination is *made* and that its output is usable in clause 6.1 (risk) and clause 4.3 (scope). This document is the record of that determination, and the issues and requirements below are the inputs the risk assessment and the ISMS scope are built on.

> **Relationship to the Cyberday report.** The Cyberday report is the system of record and the version auditors will be shown. It already answers 4.1 in outline — four external and four internal issues — and it does **not** answer 4.2 at all. This document expands 4.1 to the level of specificity the risk assessment needs, supplies the missing 4.2 determination, and lists the points where the two documents must be brought into line. §R below is the reconciliation record; it is the working list, and once the content here is carried into Cyberday version #6, §R should be cleared.

---

## 4.1 Understanding the organization and its context

Data & More ApS is a Danish ApS, founded October 2016, headquartered in Denmark, with 27 employees (June 2025). It supplies an automated data compliance platform that identifies, reports and helps remediate illegal or unnecessary personal data in customer systems. The platform is delivered either as SaaS on Hetzner infrastructure (EU, Germany) or installed on-premises in the customer's own datacentre. Data & More acts as **data processor** for direct customers and as **sub-processor** where a partner holds the controller or processor relationship.

The intended outcomes of the ISMS are: (a) protection of the confidentiality, integrity and availability of customer data entrusted to the platform; (b) demonstrable assurance to customers and their auditors; and (c) compliance with GDPR and the other obligations in the legal register.

### 4.1.1 External issues

| # | External issue | Why it affects the intended ISMS outcome |
|---|---|---|
| E1 | **GDPR and the Danish Data Protection Act** govern everything the platform touches. Data & More is a processor under Art. 28 and must meet Art. 32 security obligations and assist the controller. | Sets the non-negotiable control baseline and the breach chain (Art. 33(2): notify the controller without undue delay). |
| E1b | **Non-EU data protection regimes — CCPA and PIPEDA.** The Cyberday report names these alongside GDPR in the ISMS focus. The ISAE description names GDPR only and records no processing outside the EU/EEA. | **Open point (R1).** If these are product detection capabilities, they are not obligations of Data & More and should not sit in the ISMS focus. If they are obligations arising from US or Canadian customers, the legal register, E8 and the 4.3 scope are all understated. Resolve before approval. |
| E2 | **Customer and tender assurance demands** — ISAE 3000 reports, ISO 27001 certification, security questionnaires, audit rights in DPAs. | Assurance is a condition of sale, so an ISMS failure is a revenue issue, not only a compliance issue. |
| E3 | **Dependence on Hetzner** as the single hosting provider for the SaaS model. | Concentration and supply-chain risk; drives A.5.19–A.5.22 and continuity planning. |
| E4 | **Threat landscape** — ransomware, credential theft and phishing, compromise of open-source and build dependencies, and the fact that the platform aggregates exactly the personal data an attacker wants. | The product is a high-value target by design; drives A.5.7, A.8.7–A.8.9, A.8.25–A.8.28. |
| E5 | **NIS2** (Danish implementation). At 27 employees Data & More is below the size threshold for an essential or important entity in its own right, but in-scope customers pass NIS2-derived supply-chain requirements down by contract. | Re-confirm the direct-applicability conclusion at each review; treat the contractual pass-down as live today. |
| E6 | **DORA** (in force January 2025) where customers or partners are EU financial entities — Data & More would be an ICT third-party service provider with mandated contract terms, incident reporting support and exit arrangements. | Confirm whether any customer is a financial entity; if so, Art. 30 clauses and the register of information apply. |
| E7 | **Dual delivery model (SaaS vs on-premises)** splits the control boundary: on-premises installations put infrastructure, patching and physical security in the customer's hands. | Requires explicit complementary user entity controls and a scope boundary that does not overstate what Data & More controls. |
| E8 | **No transfers of customer data outside the EU/EEA** — all platform processing on Hetzner EU or in customer-controlled facilities. | Removes Chapter V risk for the service itself. Two qualifications: the corporate tool chain in E11 rests on US-headquartered providers, so the position holds for customer data and not automatically for corporate and HR data; and E1b must be resolved before the claim is restated. Any new sub-processor or support tool outside the EEA reopens this. |
| E9 | **Danish labour market** for security and engineering specialists. | Feeds key-person and continuity risk (I2). |
| E10 | **Market expectation that a compliance vendor is itself exemplary.** | A security incident at Data & More carries reputational damage disproportionate to its size. |
| E11 | **Dependence on the Microsoft and Cyberday tool chain.** Security guidelines and task assurance reach staff only through the Cyberday app in Microsoft Teams (Guidebook and Taskbook); Microsoft Purview is named as a governance component; Cyberday holds the ISMS documentation and its change log. | A second concentration alongside Hetzner (E3), and one that touches the *evidence* itself: loss of or lock-out from Cyberday would remove the audit trail. Drives A.5.19–A.5.22, A.8.13 backup and an export arrangement for ISMS records. |

### 4.1.2 Internal issues

| # | Internal issue | Why it affects the intended ISMS outcome |
|---|---|---|
| I1 | **Small organisation (27 employees)** across Sales, Customer Success, IT Services and Business Services. | Full segregation of duties (A.5.3) is not always achievable; compensating controls — review, logging, four-eyes on privileged actions — must be documented as deliberate design, not left as a gap. |
| I2 | **Key-person dependency** in platform engineering and in the compliance function. | Availability and continuity risk; drives documentation, cross-training, A.5.29–A.5.30. |
| I3 | **Processor role gives limited visibility into the data** being classified — content is customer-determined and may include Art. 9 special-category data. | Controls must assume worst-case sensitivity regardless of what the customer declared. |
| I4 | **Existing compliance estate**: ISAE 3000 Type 1 description with 45 control objectives; all 93 Annex A controls assessed, 82 mapped to ISAE controls; Cyberday as the ISMS platform with 12 themes active and an owner per theme; external penetration test performed. | The ISMS is built on an existing base; the remaining work is status and owner per control in the SoA, not a greenfield build. |
| I5 | **In-house development of the platform**, with its own secure development and vulnerability management policy. | A.8.25–A.8.34 are core, not peripheral: the product *is* the primary asset. |
| I6 | **Hybrid and remote working**, and endpoints used outside the office. | Drives A.6.7, A.7.9, A.8.1. |
| I7 | **Resources and budget proportionate to a 27-person company.** | Risk treatment must be prioritised; the risk acceptance criteria under clause 6.1.2 must reflect what management will actually fund. |
| I8 | **Culture and governance** — management has formally accepted responsibility for control design, implementation, monitoring and remediation, and a voluntary whistleblowing scheme is in place ahead of the 50-employee statutory threshold. | Positive factor; evidences A.5.4, A.5.31, A.5.36, A.5.37. |

> **NOTE (as in the standard):** determining these issues is the establishment of the external and internal context under clause 5.4.1 of ISO 31000:2018. Each issue above is carried into the risk assessment as context, and should be traceable either to at least one risk entry or to a recorded decision that no treatment is needed.

---

## 4.2 Understanding the needs and expectations of interested parties

The organization has determined (a) the interested parties relevant to the ISMS, (b) their relevant requirements, and (c) which of those requirements will be addressed through the ISMS.

| # | Interested party (4.2 a) | Relevant requirements (4.2 b) | Addressed through the ISMS? (4.2 c) |
|---|---|---|---|
| P1 | **Direct customers (controllers)** | Art. 28 processor obligations; confidentiality, integrity and availability of their data; agreed availability; breach notification without undue delay; audit and inspection rights; sub-processor transparency; return or deletion at end of contract. | **Yes, in full.** Primary driver of scope, of A.5.19–A.5.22 and A.8.x, and of the incident process. |
| P2 | **Partners for whom Data & More is sub-processor** | Back-to-back flow-down of the partner's own processor commitments; a notification chain that reaches the controller; evidence the partner can present to its own customers. | **Yes** — contractual flow-down plus the same control set as P1. |
| P3 | **Data subjects whose personal data is processed** | Protection against unauthorised access and misuse; data minimisation and deletion; fulfilment of their rights. | **Partly.** Security of processing: yes. Rights fulfilment: no — exercised by the controller; the ISMS covers Data & More's duty to assist under Art. 28(3)(e). |
| P4 | **Employees** | A safe and lawful workplace; clear security responsibilities and training; proportionate monitoring; lawful handling of HR data; a confidential route to raise concerns without retaliation. | **Yes** — A.6.1–A.6.8, A.5.31, and the voluntary whistleblowing scheme. |
| P5 | **Management and owners** | Protection of the business and of enterprise value; no surprises; proportionate spend; certification and assurance delivered to the agreed timetable. | **Yes** — clause 5 leadership, clause 9.3 management review, risk acceptance criteria. |
| P6 | **Datatilsynet (Danish DPA)** | Compliance as processor; cooperation under Art. 31; support for controller breach notification under Art. 33; records under Art. 30(2). | **Yes** — legal register, incident process, records of processing. |
| P7 | **External auditors and the certification body** | Sufficient appropriate evidence; documented information under clause 7.5; a complete Statement of Applicability covering all 93 Annex A controls with justification, status and owner; management assertion. | **Yes** — documentation, internal audit (9.2) and evidence retention are designed for this. |
| P8 | **Suppliers and sub-processors** — Hetzner (hosting), Microsoft (Teams, Purview), Cyberday (ISMS platform and change log), plus other service providers | Clear security requirements in contract; defined responsibilities; notice of change; right to assess; retrievability of our own records on exit. | **Yes** — A.5.19–A.5.23, supplier register, periodic review. See E11: the Cyberday dependency needs an explicit export and retention arrangement, because the ISMS evidence lives there. |
| P9 | **Prospective customers and procurement functions** | Answers to security questionnaires; evidence of certification or assurance; test results and references. | **Yes, as an output** — assurance artefacts are a deliverable of the ISMS, not a separate activity. |
| P10 | **Financial-sector customers, if any (DORA); NIS2 in-scope customers** | DORA Art. 30 contract clauses, register-of-information entries, incident reporting support, exit and resilience testing; NIS2 supply-chain requirements passed down by contract. | **Conditional.** Confirm applicability at each review; where applicable, met through the ISMS. |
| P11 | **Insurers and financing counterparties** | Evidence of controls as a condition of cover or terms. | **Partly** — the ISMS supplies the evidence; the commercial relationship is outside ISMS scope. |

### Requirements explicitly *not* addressed through the ISMS

Recording these is what makes 4.2 c) a decision rather than a formality:

- Fulfilment of data subject rights requests (P3) — exercised by the controller; Data & More assists only.
- Financial reporting, tax and employment-law obligations — handled by Business Services outside the ISMS.
- Product functionality and commercial terms requested by customers — handled by product management, except where a request has a security consequence.

---

## 4.3 Determining the scope of the ISMS

> **Reconciliation note.** The Cyberday report's "Scope of the ISMS" chapter sets out what an ISMS is and the five areas the ISMS is *focused on* (data compliance and privacy management, risk management, governance, incident response, custom solutions), and states that the scope is not industry-focused. It does not state organizational, service or boundary scope, and it does not address interfaces and dependencies with other organizations. Clause 4.3 a)–c) is therefore only partly met in the report as it stands. The statement below is the proposed boundary wording to carry into Cyberday (R3).

**Scope:** the design, development, operation and support of the Data & More automated data compliance platform, in both the SaaS (Hetzner EU, Germany) and on-premises delivery models, together with the supporting corporate functions at the Danish headquarters, including remote working by Data & More personnel.

**Boundaries and interfaces:**
- **Included** — platform source code and build pipeline; SaaS production, staging and support environments; corporate IT and SaaS tooling used by personnel; customer onboarding and support processes; the personnel, premises and suppliers supporting the above.
- **Excluded / customer responsibility** — infrastructure, OS patching, network and physical security and backup of **on-premises installations** operated by the customer; the customer's source systems; the customer's decisions on what data to process and for how long. Documented as complementary user entity controls.
- **Interfaces and dependencies** — Hetzner (hosting), the partner sub-processor chain, customer source systems.

This determination considers the issues in 4.1, the requirements in 4.2, and the interfaces and dependencies between activities performed by Data & More and those performed by other organizations. The scope is available as documented information.

## 4.4 Information security management system

Data & More ApS establishes, implements, maintains and continually improves an ISMS, including the processes needed and their interactions, in accordance with ISO/IEC 27001:2022. The ISMS is maintained in Cyberday. Process interactions: context (4) → leadership and policy (5) → risk assessment, risk treatment and objectives (6) → resources, competence, awareness and documented information (7) → operational planning and control (8) → monitoring, internal audit and management review (9) → nonconformity, corrective action and continual improvement (10).

---

## §R Reconciliation record — this document vs. the Cyberday ISMS report

Source: *ISMS description and scope — Report — Cyberday*, Version #5, 28.09.2026, 11 pages. Clause 4 content sits on pages 2–4 ("Scope of the ISMS", "Organisation's operational environment", "External Issues", "Internal Issues").

### R.1 Where the two documents agree

The Cyberday report's four external and four internal issues all survive. Nothing in this document contradicts them; the issues here are the same categories stated at the specificity clause 6.1 needs.

| Cyberday issue (v#5) | Expanded here as |
|---|---|
| External 1 — Regulatory Changes | E1, E1b, E5, E6 |
| External 2 — Cyber Threat Landscape | E4 |
| External 3 — Technological Advancements | E7, E11 |
| External 4 — Market Trends | E2, E9, E10 |
| Internal 1 — Organizational Structure | I1, I2, I8 |
| Internal 2 — Resource Availability | I2, I7 |
| Internal 3 — Internal Data Handling Practices | I3, I5, I6 |
| Internal 4 — Employee Awareness and Training | I8 (and A.6.3, delivered through the Cyberday Guidebook) |

The Cyberday report also independently supports several entries here: the 12 ISMS themes with named owners (I4); Partner management, Software development, Remote work and mobile devices and Privacy as active themes (P8, I5, I6, P3); "not industries focused" (P10 — a financial-sector customer is plausible, so the DORA question is live rather than theoretical); and the change-log and report-version controls (clause 7.5, P7).

### R.2 Open points to resolve

| Ref | Finding | Action | Owner |
|---|---|---|---|
| **R1** | The Cyberday report names **CCPA and PIPEDA** in the ISMS focus. The ISAE description names GDPR only and records no processing outside the EU/EEA. The two cannot both be complete. | Decide which is true: product *detection capability* (then remove from the ISMS focus wording, where it reads as a compliance obligation of Data & More) or actual US/Canadian customer obligations (then the legal register, E8 and the 4.3 scope are all understated). | Compliance Lead |
| **R2** | **Clause 4.2 is absent from the Cyberday report.** There is no interested-parties determination anywhere in the 11 pages — no parties, no requirements, no 4.2 c) decision. | Carry §4.2 of this document into Cyberday. This is the single most likely clause 4 nonconformity at audit: 4.2 is a *shall* with three distinct outputs, and none of the three is currently recorded. | Compliance Lead |
| **R3** | **Clause 4.3 is only partly met.** The report states focus areas, not boundaries, and says nothing about interfaces and dependencies — in particular nothing about the SaaS/on-premises split. | Carry the §4.3 boundary statement into Cyberday, including the on-premises exclusions as complementary user entity controls. An unstated boundary invites the auditor to assume customer-operated infrastructure is in scope. | Compliance Lead |
| **R4** | The report does not name **Hetzner, Microsoft or Cyberday** as dependencies in its context chapter, although the Guidebook/Taskbook mechanism it describes runs on Microsoft Teams and the ISMS evidence itself lives in Cyberday. | Add E3 and E11 to the Cyberday operational environment text; confirm an export/retention arrangement for ISMS records (A.5.19–A.5.22, A.8.13). | ISMS Admin |
| **R5** | The report does not state that the issues feed the risk assessment; the link to clause 6.1 is asserted in the risk procedure but not from the context chapter. | Add the traceability sentence (see the NOTE under 4.1.2) so each issue maps to a risk entry or a recorded no-treatment decision. | Compliance Lead |
| **R6** | **No stated interested party for the EU AI Act or for Purview-adjacent AI features**, although "AI enterprise platforms" appear in the ISMS focus. | Confirm whether any AI component is in the product or in internal tooling; if so, add to the legal register and to E1. | Compliance Lead |
| **R7** | Version and date hygiene: the Cyberday report is v#5 dated **28.09.2026**; the ISAE description is v1.0 effective **18.07.2025** with an audit period of calendar 2025; `PROJECT_STATUS.md` is dated 06.10.2025. | Confirm which documents are current before handing any of them to an auditor; a stale effective date is an easy finding. | Compliance Lead |

### R.3 Carry-across checklist for Cyberday version #6

- [ ] Resolve R1, then restate the regulatory scope consistently in both documents
- [ ] Add an Interested parties chapter (§4.2 table, including the "not addressed" list)
- [ ] Replace the scope chapter's focus-area text with, or add to it, the §4.3 boundary statement
- [ ] Add Hetzner, Microsoft and Cyberday to the operational environment as dependencies
- [ ] Add the issue → risk traceability sentence
- [ ] Re-confirm headcount, and E5/E6 applicability, at the same time

---

## Maintenance

| Trigger | Action |
|---|---|
| Annual management review | Re-confirm the 4.1 issues and the 4.2 table; record what changed |
| New customer segment (e.g. first financial-sector customer) | Re-assess E6 and P10 before signature |
| Headcount approaching 50 | Re-assess E5, I1, I8 and the whistleblowing applicability decision |
| New sub-processor or support tool, especially outside the EEA | Re-assess E8 and P8 before adoption |
| Material change to the delivery model or to the Hetzner arrangement | Re-assess E3, E7 and the 4.3 scope statement |
| Material legislative change (NIS2, DORA, GDPR guidance) | Update the legal register and E1/E5/E6 |
| New version of the Cyberday ISMS description and scope report | Re-run §R; clear any carried-across items and record what remains open |

**Related documents:** `DESCRIPTION_OF_PROCESSING_ISAE3000.md`, `ISO_27001_2022_ISAE_3000_Mapping.md`, `ISMS description and scope _ Report _ Cyberday.pdf`, `Information security policy and objectives _ Report _ Cyberday.pdf`, `Risk management procedure and result preview _ Report _ Cyberday.pdf`, `whistleblowing/01_APPLICABILITY_AND_LEGAL_REGISTER.md`.
