# ISO/IEC 27001 Control Reference Audit & Corrections

**Date:** 2026-10-12
**Scope:** All Markdown files in this repository
**Trigger:** Several control references were labelled as the 2022 revision but used 2013 numbering.

---

## 1. Basis for verification

Every reference was checked against the **ISO/IEC 27001:2022 Annex A** control set:
**93 controls in 4 themes** — A.5 Organisational (37), A.6 People (8), A.7 Physical (14),
A.8 Technological (34). There is **no A.9–A.18 in the 2022 revision**; those clause groups
belong to ISO/IEC 27001:2013 (14 groups, 114 controls).

Reference list used: `compliance-expert` skill, `references/iso27001.md` (full 93-control
Annex A table).

**Method:** every `.md` file was grepped for `A.<n>.<n>` patterns and for `ISO 27001` /
`ISO/IEC 27001`. Each hit was read in the context of its surrounding control objective, and
the reference was judged against the **described intent**, not the number alone — necessary
because several numbers exist in both revisions with different meanings (notably **A.8.1**:
2013 "Responsibility for assets" / 2022 "User endpoint devices"). A final automated scan
confirms no remaining reference falls outside the valid 2022 ranges.

---

## 2. Summary by file

| File | Control refs corrected | Year labels added | Factual/count corrections | Notes |
|---|---|---|---|---|
| `ISAE_3000_Cyberday_Mapping.md` | 29 | — | — | Was systematically 2013-numbered while labelled "(2022)" |
| `ISAE_3000_GDPR_Mapping.md` | 32 | 41 | — | Year was unlabelled throughout; now `ISO 27001:2022` |
| — *data-residency re-map (§5.1)* | 3 | — | — | Applied after review decision |
| — *data-residency addition to E.2 (§5.2)* | 2 added | — | — | New mapping, not a correction |
| — *A.5.5 added to I.4 (§5.3)* | 2 added | — | — | Closes an inconsistency between documents |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | 13 | 1 | Control set + coverage table rebuilt | Also had 3 non-existent `A.4.x` refs, a 116-control/15-category taxonomy, and a duplicate A.7.2 section (consolidated, §5.4) |
| `DESCRIPTION_OF_PROCESSING_ISAE3000.md` | 14 (+7 Cyberday tags) | — | 3 coverage claims | |
| `B3_AUDIT_EVIDENCE_SUMMARY.md` | 6 | — | — | |
| `GOOGLE_DOCS_UPDATES_RECOMMENDATIONS.md` | 6 | 7 | 8 coverage claims | |
| `PROJECT_STATUS.md` | — | — | 4 coverage claims | |
| `GDPR_to_ISAE_Coverage_Checklist.md` | 0 | 0 | 0 | No ISO references |
| `ISAE_3000_Document_GDPR_References.md` | 0 | 0 | 0 | No ISO references |

---

## 3. Corrections — 2013 numbering labelled as 2022

*Line numbers are those of the corrected files on this branch. The ISAE control ID in each
section heading is the stable reference.*

### 3.1 `ISAE_3000_Cyberday_Mapping.md` (all labelled "ISO 27001 (2022)")

| Line | Was | Now | Reason |
|---|---|---|---|
| 90 | A.12 — Operational Controls | **A.8** — Technological Controls | 2013 A.12 (Operations security) → 2022 theme A.8 |
| 107 | A.12.2 — Malware protection | **A.8.7** — Protection against malware | 2013 A.12.2.1 |
| 124 | A.13.1 — Network security boundary | **A.8.20** — Networks security | 2013 A.13.1.1 |
| 141 | A.13.1 — Network segregation | **A.8.22** — Segregation of networks | 2013 A.13.1.3 |
| 158 | A.9 — Access Control | **A.5.15** — Access control | 2013 A.9 theme |
| 180 | A.12.4 — Event logging and monitoring | **A.8.16** — Monitoring activities (with A.8.15) | Control is system monitoring + alerting |
| 196 | A.10.1 — Cryptography | **A.8.24** — Use of cryptography | 2013 A.10.1.1 |
| 216 | A.12.4 — Event logging & monitoring | **A.8.15** — Logging | Control is event logging specifically |
| 254 | A.14.2 — Vulnerability management | **A.8.8** — Management of technical vulnerabilities | 2013 A.12.6.1 |
| 272 | A.14.1 — Information security change management | **A.8.32** — Change management | 2013 A.12.1.2 / A.14.2.2 |
| 289 | A.9.2 — User access management | **A.5.18** — Access rights | 2013 A.9.2 |
| 309 | A.9.4 — Access management for privileged rights | **A.8.5 / A.8.2** — Secure authentication (MFA); privileged access rights | ISAE control is 2FA for high-risk accounts |
| 327 | A.11.1 — Physical security perimeter | **A.7.1** — Physical security perimeters (with A.7.2) | 2013 A.11.1.1 |
| 381 | A.6.1 — Personnel screening | **A.6.1** — Screening | Number correct; official title applied |
| 400 | A.6.2 — Information security awareness, education and training | **A.6.3** — same title | A.6.2 (2022) is "Terms and conditions of employment" |
| 419 | A.6.3 — Return of assets | **A.5.11** — Return of assets | A.6.3 (2022) is awareness/training |
| 437 | A.6.2 — Information security awareness | **A.6.5** — Responsibilities after termination or change of employment | ISAE control is post-departure confidentiality |
| 454 | A.6.2 — Information security awareness, education and training | **A.6.3** — same title | As line 400 |
| 475 | A.8.3 — Retention of information | **A.5.33** — Protection of records (retention) | A.8.3 (2022) is "Information access restriction" |
| 510 | A.8.3 — Retention of information (removal of data) | **A.8.10** — Information deletion | As above; intent is deletion |
| 530 | A.8.1 — Onsite and offsite equipment | **A.5.23** — Information security for use of cloud services + **A.5.14** — Information transfer | Data residency — see §5.1 |
| 569 | A.14.2 — Supplier relationships & governance | **A.5.19** — Information security in supplier relationships | 2013 A.15 |
| 586 | A.14.2 — Supplier relationships | **A.5.19** — same | |
| 601 | A.14.2 — Changes in supplier relationships | **A.5.22** — Monitoring, review and change management of supplier services | |
| 618 | A.14.2 — Supplier security requirements | **A.5.20** — Addressing information security within supplier agreements | |
| 634 | A.14.2 — Supplier information management | **A.5.19** — ... (supplier register) | |
| 655 | A.14.2 — Monitoring of supplier performance | **A.5.22** — Monitoring, review and change management of supplier services | |
| 766 | A.17.1 — Incident management procedure | **A.5.24** — Information security incident management planning and preparation | 2013 A.16.1.1; A.17 was business continuity |
| 783 | A.12.4 — Event logging & monitoring | **A.8.16** — Monitoring activities (with A.8.15) | |
| 802 | A.17.1 — Incident response timelines | **A.5.26** — Response to information security incidents | 2013 A.16.1.5 |
| 820 | A.17.1 — Incident response and post-incident activities | **A.5.26 / A.5.27** — Response to, and learning from, incidents (plus **A.5.5** at line 819, see §5.3) | 2013 A.16.1.5–6 |

### 3.2 `ISAE_3000_GDPR_Mapping.md`

Revision year was **unlabelled** throughout (`ISO 27001: A.x.y`); all 41 bullets now read
`ISO 27001:2022:`. The header's "Supporting Framework" line now reads
`ISO/IEC 27001:2022, ISO/IEC 27701`.

| Line | Was | Now |
|---|---|---|
| 117 | A.5, A.12 (organizational and operational controls) | **A.5, A.8** (organisational and technological controls) |
| 143 | A.12 (operational controls based on risk) | **A.8** (technological controls based on risk) |
| 168 | A.12.2 (malware protection) | **A.8.7** (protection against malware) |
| 193 | A.13.1 (network security) | **A.8.20** (networks security) |
| 217 | A.13.1 (network segregation) | **A.8.22** (segregation of networks) |
| 243 | A.9 (access control) | **A.5.15** (access control) |
| 274 | A.12.4 (event logging and monitoring) | **A.8.15** (logging), **A.8.16** (monitoring activities) |
| 299 | A.10.1 (cryptography) | **A.8.24** (use of cryptography) |
| 328 | A.12.4 (event logging, monitoring, protected logs) | **A.8.15**, **A.8.16** |
| 390 | A.14.2 (vulnerability management) | **A.8.8** (management of technical vulnerabilities) |
| 424 | A.14.1 (information security change management) | **A.8.32** (change management) |
| 455 | A.9.2 (user access management) | **A.5.18** (access rights), **A.5.16** (identity management) |
| 491 | A.9.4 (privileged access rights) | **A.8.5** (secure authentication), **A.8.2** (privileged access rights) |
| 519 | A.11.1 (physical security perimeter) | **A.7.1**, **A.7.2** (physical entry) |
| 615 | A.6.1 (personnel screening) | **A.6.1** (screening) — title only |
| 650, 746 | A.6.2 (awareness and training) | **A.6.3** (information security awareness, education and training) |
| 685 | A.6.3 (return of assets) | **A.5.11** (return of assets) |
| 717 | A.6.2 (ongoing awareness) | **A.6.5** (responsibilities after termination or change of employment) |
| 787 | A.8.3 (retention of information) | **A.5.33** (protection of records – retention) |
| 859 | A.8.3 (retention and disposal) | **A.5.33**, **A.8.10** (information deletion) |
| 898 | A.8.1 (on-site and off-site storage) | **A.5.23** (information security for use of cloud services), **A.5.14** (information transfer) — see §5.1 |
| 979, 1011, 1117 | A.14.2 (supplier relationships / information management / inventory) | **A.5.19** (information security in supplier relationships) |
| 1045, 1152 | A.14.2 (supplier relationship changes / monitoring supplier performance) | **A.5.22** (monitoring, review and change management of supplier services) |
| 1086 | A.14.2 (supplier security requirements) | **A.5.20** (addressing information security within supplier agreements) |
| 1204 | A.8.1 (storage in different locations) | **A.5.23** (information security for use of cloud services), **A.5.14** (information transfer) — see §5.1 |
| 1446 | A.17.1 (incident management procedure) | **A.5.24** |
| 1487 | A.12.4 (event logging), A.6.2 (awareness training) | **A.8.15**, **A.8.16**, **A.6.3** |
| 1535 | A.17.1 (incident response timelines) | **A.5.26** |
| 1596 | A.17.1 (incident documentation and reporting) | **A.5.5** (contact with authorities), **A.5.26**, **A.5.27** — see §5.3 |

---

## 4. Corrections — wrong 2022 control (number exists, meaning does not match)

These were **not** 2013 numbering. The number is valid in 2022 but denotes a different
control than the text described — the most error-prone category, and the reason each
reference was judged on intent.

| File | Line | Was | Actually means in 2022 | Now |
|---|---|---|---|---|
| `ISO_27001_2022_ISAE_3000_Mapping.md` | 113 | A.5.8 — Use of Cryptography | A.5.8 = Information security in project management | **A.8.24** — Use of cryptography |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | 297 | A.8.2 — User Authentication for External Connections | A.8.2 = Privileged access rights | **A.8.5** — Secure authentication |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | 321 | A.7.7 — Delivery and Loading Areas | A.7.7 = Clear desk and clear screen | **A.7.2** — Physical entry; section merged into the canonical A.7.2 (see §5.4) |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | 369 | A.8.3 — Managing Removable Media | A.8.3 = Information access restriction | **A.7.10** — Storage media |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | 377 | A.8.4 — Utility Supply | A.8.4 = Access to source code | **A.7.11** — Supporting utilities |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | 385 | A.8.5 — Cabling Security | A.8.5 = Secure authentication | **A.7.12** — Cabling security |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | 393 | A.8.6 — Acquisition, Installation, Replacement and Removal of Equipment | A.8.6 = Capacity management | **A.7.13 / A.7.14** — Equipment maintenance; secure disposal or re-use |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | 537 | A.8.29 — Information Systems Resilience and Redundancy | A.8.29 = Security testing in development and acceptance | **A.8.14** — Redundancy of information processing facilities |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | — | A.8.30 — Development, Testing and Production Environments | A.8.30 = Outsourced development | **A.8.31** — Separation of development, test and production environments |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | — | A.8.31 — Change of Platform | A.8.31 = Separation of dev/test/prod | **A.8.32** — Change management |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | — | A.8.32 — Monitoring and Reviewing | A.8.32 = Change management | **A.8.16** — Monitoring activities |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | — | A.5.18 — Rights of Access | — | **A.5.18** — Access rights (official title) |
| `ISO_27001_2022_ISAE_3000_Mapping.md` | — | A.5.24 — Planning and Preparing for Information Security Incident Handling | — | **A.5.24** — Information security incident management planning and preparation (official title) |
| `DESCRIPTION_OF_PROCESSING_ISAE3000.md` | 541 | A.5.23 (Encryption and key management) | A.5.23 = Information security for use of cloud services | **A.8.24** — Use of cryptography |
| `DESCRIPTION_OF_PROCESSING_ISAE3000.md` | 541 | A.8.27 (Protection of system architecture) | — | **A.8.27** — Secure system architecture and engineering principles (title) |
| `DESCRIPTION_OF_PROCESSING_ISAE3000.md` | 644 | A.8.12 (Security of system installations) | A.8.12 = Data leakage prevention | **A.8.19** — Installation of software on operational systems |
| `DESCRIPTION_OF_PROCESSING_ISAE3000.md` | 955 | A.5.23 (Encryption and key management), A.8.24 (Data encryption) | as above | **A.8.24** — Use of cryptography, including key management |
| `DESCRIPTION_OF_PROCESSING_ISAE3000.md` | 1182 | A.8.32 (Monitoring system activity) | A.8.32 = Change management | **A.8.16** — Monitoring activities |
| `DESCRIPTION_OF_PROCESSING_ISAE3000.md` | 1313 | A.8.34 (Incident handling) | A.8.34 = Protection of information systems during audit testing | **removed** — A.5.24–A.5.27 already cover it |
| `DESCRIPTION_OF_PROCESSING_ISAE3000.md` | 1332 | A.8.30 (Development and testing environments) | A.8.30 = Outsourced development | **A.8.31** — Separation of development, test and production environments |
| `DESCRIPTION_OF_PROCESSING_ISAE3000.md` | 1370 | A.8.31 (Change of platform, operating system or applications) | A.8.31 = Separation of dev/test/prod | **A.8.32** — Change management |
| `DESCRIPTION_OF_PROCESSING_ISAE3000.md` | 432 | A.6.3 (Information and digital literacy) | — | **A.6.3** — Information security awareness, education and training (title) |
| `DESCRIPTION_OF_PROCESSING_ISAE3000.md` | 742, 841, 1294, 1390 | A.8.7 "Prevention of malware"; A.8.20 "Network security"; A.8.22 "Network segregation"; A.8.13 "Backup procedures"; A.5.18 "Rights of access" | — | Official titles: Protection against malware; Networks security; Segregation of networks; Information backup; Access rights |
| `B3_AUDIT_EVIDENCE_SUMMARY.md` | 611, 819 | A.8.12 (Configuration Management) | A.8.12 = Data leakage prevention | **A.8.9** — Configuration management |
| `B3_AUDIT_EVIDENCE_SUMMARY.md` | 820 | A.6.3 — Information and digital literacy | — | **A.6.3** — Information security awareness, education and training |
| `B3_AUDIT_EVIDENCE_SUMMARY.md` | 389, 601, 817 | A.8.7 — Prevention of malware | — | **A.8.7** — Protection against malware |
| `GOOGLE_DOCS_UPDATES_RECOMMENDATIONS.md` | 143 | ISO A.5.23 (technical and cryptographic controls) | A.5.23 = cloud services | **A.8.24**, A.8.x |
| `GOOGLE_DOCS_UPDATES_RECOMMENDATIONS.md` | 147 | ISO A.5.10 (retention, deletion, DSR) | A.5.10 = Acceptable use of information and other associated assets | **A.5.33**, **A.8.10** |
| `GOOGLE_DOCS_UPDATES_RECOMMENDATIONS.md` | 149 | ISO A.5.23 (secure data access and transfer) | A.5.23 = cloud services | **A.5.14**, **A.8.24** |
| `GOOGLE_DOCS_UPDATES_RECOMMENDATIONS.md` | 114, 213 | ISO#A5.15-22 (Access Controls) | A.5.19–A.5.22 are supplier controls | **ISO#A5.15-18** |
| `DESCRIPTION_OF_PROCESSING_ISAE3000.md` | 1672 | ISO#A5.15-22 (Access Controls) | as above | **ISO#A5.15-18** |

**Cyberday tags updated to match** (`DESCRIPTION_OF_PROCESSING_ISAE3000.md`): lines 601/632
`ISO#A5.23` → `ISO#A8.24`; 702/730 `ISO#A8.12` → `ISO#A8.19`; 1019/1050 `ISO#A5.23, ISO#A8.24`
→ `ISO#A8.24`; 1247/1280 `ISO#A8.32` → `ISO#A8.16`. **These tags exist in Cyberday and must be
re-tagged there to stay consistent with the documents.**

### 4.1 A.8.1 — the ambiguous number, resolved by intent

A.8.1 appears in both revisions with different meanings (2013 "Responsibility for assets" /
2022 "User endpoint devices"), so each instance was judged on its described intent:

| Location | Described intent | Resolution |
|---|---|---|
| `ISAE_3000_Cyberday_Mapping.md:530` | "Onsite and offsite equipment" (storage/processing locations) | → **A.5.23 + A.5.14** (see §5.1) |
| `ISAE_3000_GDPR_Mapping.md:898` | "on-site and off-site storage" | → **A.5.23 + A.5.14** (see §5.1) |
| `ISAE_3000_GDPR_Mapping.md:1204` | "storage in different locations" (third-country transfers) | → **A.5.23 + A.5.14** (see §5.1) |
| `ISO_27001_2022_ISAE_3000_Mapping.md:289` | "User Endpoint Devices" — endpoint protection, malware, inventory | **Already correct 2022 usage — left unchanged** |

---

## 5. Flagged — genuinely ambiguous, not silently guessed

### 5.1 RESOLVED — data residency controls mapped to A.5.23 + A.5.14

The original `A.8.1` references under ISAE **E.1** ("Storage & Processing Procedure Aligned
with DPA") and **G.1** (third-country transfer procedure) were first restated as the literal
renumber of their 2013 intent — A.7.9 Security of assets off-premises (2013 A.11.2.6) — and
flagged, because these ISAE controls are really about **data residency**: which cloud region
and jurisdiction personal data is stored and processed in, not physical assets leaving the
premises.

**Decision taken (2026-10-12): use A.5.23 and A.5.14 for the data residency controls.**
Applied at:

| File | Line | ISAE control | Was (original) | Interim | Final |
|---|---|---|---|---|---|
| `ISAE_3000_Cyberday_Mapping.md` | 530–531 | E.1 | A.8.1 "Onsite and offsite equipment" | A.7.9 | **A.5.23** Information security for use of cloud services + **A.5.14** Information transfer |
| `ISAE_3000_Cyberday_Mapping.md` | 549–550 | E.2 | *(no ISO 27001 reference)* | — | **A.5.23** + **A.5.14** (added) |
| `ISAE_3000_GDPR_Mapping.md` | 898 | E.1 | A.8.1 "on-site and off-site storage" | A.7.9 | **A.5.23** + **A.5.14** |
| `ISAE_3000_GDPR_Mapping.md` | 935 | E.2 | *(no ISO 27001 reference)* | — | **A.5.23** + **A.5.14** (added) |
| `ISAE_3000_GDPR_Mapping.md` | 1204 | G.1 | A.8.1 "storage in different locations" | A.5.14 | **A.5.23** + **A.5.14** |

A.7.9 is no longer referenced anywhere and remains on the "not yet assessed" list in
`ISO_27001_2022_ISAE_3000_Mapping.md`, which is correct — that document does not assess it.

### 5.2 RESOLVED — ISAE E.2 given the same mapping

E.2 ("Actual Processing/Storage Locations Match Approved Locations") is the sibling
data-residency control. It carried SOC 2, GDPR, ISO 27017, DORA (and in the GDPR mapping
ISO 27701) references but **no ISO 27001 reference at all** — so there was nothing to correct
here; this was a mapping that was missing, not a wrong one.

**Decision taken (2026-10-12): add A.5.23 + A.5.14 to E.2 as well.** Applied in both mapping
documents — see the E.2 rows in the §5.1 table. Note this is an *addition* to the control
mapping rather than a reference correction: it widens ISAE E.2's ISO 27001 coverage.

### 5.3 RESOLVED — ISAE I.4 given A.5.5 Contact with authorities

The `A.17.1` reference under ISAE **I.4** ("Assistance with Reports to Danish Data Protection
Authority") was restated as **A.5.26 / A.5.27**, preserving its original "incident response and
post-incident activities" wording — but the control is specifically about **filing reports with
a supervisory authority**, for which **A.5.5 (Contact with authorities)** is the closest 2022
control.

**Decision taken (2026-10-12): add A.5.5 to I.4.** Applied at:

| File | Line | Now |
|---|---|---|
| `ISAE_3000_Cyberday_Mapping.md` | 819–820 | **A.5.5** Contact with authorities; **A.5.26 / A.5.27** Response to, and learning from, incidents |
| `ISAE_3000_GDPR_Mapping.md` | 1596 | **A.5.5** (contact with authorities), **A.5.26**, **A.5.27** |

This closes an inconsistency rather than inventing a mapping: `ISO_27001_2022_ISAE_3000_Mapping.md`
already mapped **A.5.5 → ISAE I.1, I.4** (MEDIUM alignment), so the link was asserted in one
document and missing from the other two. A.5.5 was already counted as assessed, so the coverage
figures in §6 are unchanged.

### 5.4 RESOLVED — A.7.7 "Delivery and Loading Areas" consolidated into A.7.2

2013 A.11.1.6 was **merged into A.7.2 Physical entry** in the 2022 revision; there is no
standalone 2022 control for delivery and loading areas (A.7.7 in 2022 is "Clear desk and
clear screen"). Retitling the old A.7.7 section therefore produced two A.7.2 sections in
`ISO_27001_2022_ISAE_3000_Mapping.md`.

**Resolved (2026-10-12):** the two sections are merged into the single A.7.2 section at
line 321. Its requirement list now carries the delivery and loading items — "Segregation of
delivery and loading areas from secure areas" and "Control and inspection of incoming and
outgoing materials" — alongside the original physical-entry requirements, and an inline
consolidation note records where they came from. The duplicate section is deleted.

The merged section keeps **HIGH** alignment (the verdict of the canonical A.7.2 section); the
duplicate's MEDIUM verdict is dropped. This does not move any coverage figure, because A.7.2
was already counted once as a distinct control: A.7 remains 11 of 14 assessed with HIGH 4,
MEDIUM 6, not covered 1, and the totals stay at 71 assessed / 40 / 22 / 9 and 62 of 93 (67%).
Re-verified programmatically after the merge.

**A.7.7 Clear desk and clear screen** stays on the not-yet-assessed gap list in §6, which is
correct — no section assesses it. Note the A.7.6 "Working in Secure Areas" section mentions
a clean-desk policy in passing, so some of that content exists but is not mapped to A.7.7.

### 5.5 ISAE B.11 (vulnerability scans / pen testing) → A.5.7 Threat Intelligence

Left unchanged: A.5.7 is a **valid 2022 control** with a correct title, so this is not a
numbering error. It is, however, a weak mapping — scanning and pen testing are
**A.8.8 (Management of technical vulnerabilities)** and **A.8.29 (Security testing in
development and acceptance)**. Affects `ISO_27001_2022_ISAE_3000_Mapping.md:105`,
`GOOGLE_DOCS_UPDATES_RECOMMENDATIONS.md:117/225`, `DESCRIPTION_OF_PROCESSING_ISAE3000.md:1675`.
**Mapping-quality issue for review, deliberately not changed.**

### 5.6 ISAE B.10 (pseudonymisation in dev/test) → A.5 (theme-level)

Left unchanged: "A.5 — Organisational controls" is valid 2022. But the precise controls are
**A.8.11 (Data masking)** and **A.8.33 (Test information)**.
**Recommend tightening; not changed** because the existing reference is not wrong.

### 5.7 ISO 27701 / ISO 27017 references

`ISO 27701: A.2.1 / A.2.2 / A.3.1` and `ISO 27017: A.2.1` do not match the Annex A structure
of those standards either. **Out of scope for this ISO 27001 pass — flagged for a separate
check.**

---

## 6. Material change — control counts and coverage figures

This is the most significant consequence and **needs sign-off**.

The documents described ISO 27001:2022 as **"116 controls across 15 categories"** and claimed
**"95% coverage (110 of 116 controls)"**. The 2022 revision has **93 controls in 4 themes**;
the 116/15 taxonomy does not exist in either revision (2013 had 114 controls in 14 groups).
The percentage was therefore computed against a denominator that does not exist.

`ISO_27001_2022_ISAE_3000_Mapping.md` was recounted on the real 93-control basis, using the
**per-control `Alignment` verdicts already recorded in that document** — no verdict was added,
removed, or changed:

| Theme | Annex A controls | Assessed | Fully aligned | Partially aligned | Not covered | **Not yet assessed** |
|---|---|---|---|---|---|---|
| A.5 — Organisational | 37 | 31 | 20 | 6 | 5 | 6 |
| A.6 — People | 8 | 7 | 5 | 1 | 1 | 1 |
| A.7 — Physical | 14 | 11 | 4 | 6 | 1 | 3 |
| A.8 — Technological | 34 | 22 | 11 | 9 | 2 | 12 |
| **TOTAL** | **93** | **71** | **40** | **22** | **9** | **22** |

> **Superseded by §10.** The 22 unassessed controls have since been assessed, taking coverage
> to **82 of 93 (88%)**. The account below is the record of what this correction pass found at
> the time, and is kept as-is for traceability.

**Restated headline: 62 of 93 Annex A controls (67%) have an identified ISAE mapping**, down
from the claimed 95%. The drop is **not** a loss of controls — it is that 22 Annex A controls
were never assessed and the old denominator was inflated. Of the 71 controls actually
assessed, 87% map to an ISAE control.

The 22 unassessed controls are: A.5.8, A.5.14, A.5.28, A.5.35, A.5.36, A.5.37, A.6.8, A.7.7,
A.7.8, A.7.9, A.8.2, A.8.3, A.8.4, A.8.11, A.8.12, A.8.13, A.8.15, A.8.17, A.8.29, A.8.30,
A.8.33, A.8.34. Several are in fact covered by ISAE controls elsewhere in this set (A.5.14 and
A.7.9 under E.1/G.1, A.8.13 under the backup control, A.8.15 under B.7/B.9, A.8.2 under B.14,
A.8.33 under B.10) but have no entry in the mapping document.

**ISO/IEC 27001:2022 clause 6.1.3(d) requires the Statement of Applicability to address all 93
Annex A controls** with an inclusion/exclusion justification, so these 22 are mandatory gaps,
not optional.

The 67% figure was propagated to the four documents that quoted the old number
(`PROJECT_STATUS.md`, `DESCRIPTION_OF_PROCESSING_ISAE3000.md`,
`GOOGLE_DOCS_UPDATES_RECOMMENDATIONS.md`, and the mapping document itself), because leaving
"110 of 116" would have left a false statement about the standard in place.
**If you would rather restate these differently, this is the change to revisit.**

Two related overclaims were also corrected:
- "All ISO 27001:2022 security controls are supported by ISAE controls"
  (`DESCRIPTION_OF_PROCESSING_ISAE3000.md:139`)
- "Coverage Status: 100% mapped to GDPR and ISO 27001:2022"
  (`DESCRIPTION_OF_PROCESSING_ISAE3000.md:222`)

---

## 7. Also corrected: non-existent A.4 references

`ISO_27001_2022_ISAE_3000_Mapping.md` listed `A.4.1`, `A.4.2`, `A.4.3` as Annex A controls
under "FOUNDATION (Section 4: 23 Controls)". **There is no Annex A.4.** These are
management-system requirements from **Clause 4** of the main standard and are now cited as
`Clause 4.1 / 4.2 / 4.3`, with a note that they are excluded from the 93-control Annex A counts.

Per-category control counts in that document's own headings were also corrected where they
did not match the controls actually listed (Category 2: 7→6, Category 5: 12→11,
Category 6: 6→3, Category 11: 2→1, Category 12: 8→3, Category 13: 5→3).

---

## 8. Verified correct — left unchanged

Confirmed valid 2022 references, no edit needed: A.5.1, A.5.2, A.5.3, A.5.4, A.5.5, A.5.6,
A.5.7, A.5.9, A.5.10, A.5.11, A.5.12, A.5.13, A.5.15, A.5.16, A.5.17, A.5.19, A.5.20, A.5.21,
A.5.22, A.5.23, A.5.25, A.5.26, A.5.27, A.5.29, A.5.30, A.5.31, A.5.32, A.5.33, A.5.34, A.6.1,
A.6.2, A.6.4, A.6.6, A.6.7, A.7.1–A.7.6, A.8.1 (endpoint-device usage only), A.8.7, A.8.8,
A.8.9, A.8.10, A.8.18, A.8.19, A.8.20, A.8.21, A.8.22, A.8.23, A.8.25, A.8.26, A.8.27, A.8.28.

---

## 9. Follow-up actions

| # | Action | Owner |
|---|---|---|
| 1 | ~~Decide A.7.9 vs A.5.23/A.5.14 for data-residency controls~~ — **resolved 2026-10-12: A.5.23 + A.5.14 applied to E.1, E.2 and G.1** (§5.1, §5.2) | Done |
| 2 | Sign off or restate the coverage figure (§6) — now **88% (82 of 93)** after the completion pass, see §10 | Compliance |
| 3 | ~~Assess the 22 outstanding Annex A controls~~ — **done 2026-10-12** (§10); SoA still needs status + owner per control | Partly done |
| 4 | Re-tag the changed `ISO#...` tags in Cyberday (§4) | Cyberday admin |
| 5 | ~~Consolidate the duplicate A.7.2 sections~~ — **resolved 2026-10-12** (§5.4) | Done |
| 6 | Review the weak mappings in §5.5 and §5.6 (§5.3 resolved 2026-10-12: A.5.5 added to I.4) | Compliance |
| 7 | Separate check of the ISO 27701 / ISO 27017 references (§5.7) | Compliance |
| 8 | Apply the same corrections to the Google Docs versions of these documents | Doc owner |

---

## 10. SoA completion pass — the 22 unassessed controls (2026-10-12)

The 22 controls listed in §6 as not yet assessed have been assessed against the same
45-control ISAE 3000 set and the same alignment scale, and added to
`ISO_27001_2022_ISAE_3000_Mapping.md` as **Category 15**. All 93 Annex A controls now have an
entry, so clause 6.1.3(d) is satisfied for the *mapping* basis.

### Verdicts assigned

| Alignment | Count | Controls |
|---|---|---|
| **HIGH** | 9 | A.5.14 Information transfer; A.5.37 Documented operating procedures; A.6.8 Information security event reporting; A.8.2 Privileged access rights; A.8.3 Information access restriction; A.8.11 Data masking; A.8.15 Logging; A.8.29 Security testing in development and acceptance; A.8.33 Test information |
| **MEDIUM** | 11 | A.5.8 Information security in project management; A.5.28 Collection of evidence; A.5.35 Independent review of information security; A.5.36 Compliance with policies, rules and standards; A.7.8 Equipment siting and protection; A.7.9 Security of assets off-premises; A.8.4 Access to source code; A.8.12 Data leakage prevention; A.8.13 Information backup; A.8.30 Outsourced development; A.8.34 Protection of information systems during audit testing |
| **LOW / NOT COVERED** | 2 | A.7.7 Clear desk and clear screen; A.8.17 Clock synchronisation |

### Revised coverage (all 93 assessed)

| Theme | Controls | HIGH | MEDIUM | No ISAE coverage |
|---|---|---|---|---|
| A.5 — Organisational | 37 | 22 | 10 | 5 |
| A.6 — People | 8 | 6 | 1 | 1 |
| A.7 — Physical | 14 | 4 | 8 | 2 |
| A.8 — Technological | 34 | 17 | 14 | 3 |
| **TOTAL** | **93** | **49** | **33** | **11** |

**82 of 93 (88%) mapped**, up from 62 of 93 (67%). The rise is entirely the newly assessed
controls — no existing verdict was changed. Re-derived programmatically from the document.

### Three substantive gaps found in the ISAE control set itself

Not mapping problems — gaps in what the 45-control engagement actually tests:

1. **No backup or restore control.** Nothing in the ISAE set names backup, yet GDPR
   Art. 32(1)(c) requires the ability to restore availability and access to personal data in a
   timely manner. A.8.13 maps only to the generic B.1/B.2 safeguards. **Recommend adding
   backup and restore-testing evidence to the engagement.**
2. **No off-premises asset control.** A.7.9 has no ISAE counterpart while remote working
   (A.6.7) is in scope, so devices outside the premises are untested.
3. **Availability coverage is thin overall.** A.5.29, A.5.30, A.8.6 and A.8.13 all fall outside
   ISAE coverage, leaving GDPR Art. 32(1)(b)–(c) resilience obligations largely unevidenced.

### Two points requiring management input

- **"No ISAE coverage" is not a justification for exclusion.** The 11 controls with no ISAE
  mapping are still applicable to the ISMS; ISAE and Annex A have different scopes. Exclusion
  under clause 6.1.3(d) needs a risk-based justification.
- **A.8.30 Outsourced development** is the one control whose applicability cannot be determined
  from these documents: excludable if all development is in-house, included if any is contracted
  out. **Needs confirming.**

### What is still outstanding for the SoA

This pass establishes which ISAE control addresses which Annex A control. It does **not**
assert that any control is implemented. The SoA additionally requires, per control: the
inclusion/exclusion decision, the justification, implementation status and an owner. That
remains management's to supply.
