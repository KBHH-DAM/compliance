# ISMS Scope Statement — Data & More ApS

**Purpose:** a precise replacement for the *Scope of the ISMS* section in the Cyberday report
*ISMS description and scope* (current published version: **#5, 28.09.2026**).

**Why this rewrite:** the current scope text lists five *activities* the ISMS is "focused on"
(Data Compliance and Privacy Management, Risk Management, Governance, Incident Response,
Custom Solutions). Those are control topics, not a scope. ISO/IEC 27001:2022 clause 4.3
requires the scope to state the **boundaries and applicability** of the ISMS, and clause 4.3
note/4.1–4.2 require the **interfaces and dependencies** between what the organisation does
itself and what is done by other parties. An auditor reading the v5 text cannot answer:
which legal entity, which services, which locations, which systems, which data, what is
*outside* the ISMS, and who else is involved. Sections 1–3 below answer each of those.

**Source of facts:** `DESCRIPTION_OF_PROCESSING_ISAE3000.md` (ISAE 3000 Type 1 description of
processing), `ISO 27001_27002_2022 _ Report _ Cyberday_SoA_is_included.pdf`, and the Cyberday
reports in this repository. Anything not evidenced by those sources is listed in
**Section 4 — Confirm before publishing** rather than asserted.

---

## 1. Scope statement (paste-ready)

### 1.1 Short form

> The Information Security Management System (ISMS) of **Data & More ApS** (CVR no. 38185659,
> registered at Flæsketorvet 68, DK-1711 København V, Denmark) covers the
> development, delivery, operation and support of the company's **automated data compliance
> platform** — the identification, classification, reporting and remediation-tracking of
> personal data in customer systems — in both delivery models: the **SaaS service hosted on
> Hetzner infrastructure in the EU (Germany)** and the **on-premises deployment installed in
> customer-controlled environments**.
>
> The ISMS covers all Data & More organisational functions (Sales, Customer Success,
> IT Services, Business Services), all personnel including contractors, the company's
> registered office in Copenhagen and its further offices (§1.2 c) together with remote and
> mobile working, and the corporate and production IT used to deliver the service. It covers
> customer personal data processed by Data & More as **data processor and as sub-processor**, the compliance metadata and audit records the
> platform generates, platform source code, and the company's own business information.
>
> The ISMS is established to meet the GDPR, the Danish Data Protection Act and the obligations
> in customer Data Processing Agreements, and is implemented against **ISO/IEC 27001:2022** with
> applicability recorded in the Statement of Applicability, and reported on under
> **ISAE 3000 (Revised)**.
>
> Scope is not limited by industry: Data & More serves customers in all sectors, and no
> industry-specific ISMS theme is excluded on industry grounds.

### 1.2 Boundaries and applicability

**a) Organisational boundary.** Data & More ApS as a single legal entity — CVR no. 38185659,
registered at Flæsketorvet 68, DK-1711 København V, Denmark, founded October 2016, 29 employees
(as-of date to be confirmed, §4.1). **One legal entity covers all operations**, including the
Calgary office and the North American client work run from it: there is no separate company, so
every office in §1.2 c is a Data & More ApS site and all personnel at them are inside this
boundary. All four organisational areas are in scope, with no function excluded:

| Function | In scope because |
|---|---|
| Sales | handles customer and prospect data, contract and DPA negotiation |
| Customer Success | onboarding, configuration and consultancy with access to customer environments |
| IT Services | infrastructure, support, and feature development for the platform |
| Business Services | finance, HR and internal compliance; processes employee and supplier data |

All employees, management, and externally contracted personnel acting under Data & More's
direction are in scope for personnel security, awareness, access control and guideline
acceptance.

**b) Services and products in scope.** The automated data compliance platform, comprising:

1. **Discovery and scanning** of customer data sources, on-premises and in the cloud,
   including continuous/recurring scanning.
2. **Classification and identification** of personal and sensitive data, including
   **customer-specific dictionaries and taxonomies** configured per customer.
3. **Compliance reporting and privacy monitoring**, including dashboards and alerting used by
   customers to evidence their own compliance position.
4. **Remediation management** — tracking and reporting of the handling of identified illegal
   or unnecessary personal data.
5. **Integrations** with customer data platforms, including **Microsoft Purview**, and the
   **AI/LLM-assisted classification capabilities** of the platform. Both are generally available
   to customers and in production; neither is in scope as roadmap only.
6. **Delivery, support and consultancy** wrapped around the above: onboarding, configuration,
   customer support, and the secure development lifecycle that produces releases.

Both delivery models are in scope: **SaaS** (Hetzner, EU/Germany) and **on-premises**
(Data & More software operated in a customer-controlled environment — see 1.3 for the
responsibility split).

**c) Physical and location boundary.**

- **Registered office and headquarters:** Flæsketorvet 68, DK-1711 København V, Denmark.
- **Further offices**, as published on dataandmore.com: Hamburg (Elbchaussee 438, 22609 Hamburg,
  Germany) and Hässleholm (Okvägen 101, 28151 Hässleholm, Sweden). The published office list
  needs confirmation before publishing — the website's contact and about pages do not agree
  (§4.2).
- The **Calgary office** (500 – 4th Avenue SW, Calgary, Alberta, Canada), from which the
  company's North American client work is run. It is a Data & More ApS site and therefore **an
  ISMS location**, and the only one outside the EU/EEA: personnel security, access control,
  endpoint and remote-working controls apply to its personnel as they do everywhere else.
  Calgary personnel have **no access to the customer personal data covered by this scope**.
  Because the company runs **one shared Microsoft tenant across all offices**, that separation
  is enforced by access controls inside the shared tenant, not by separate tenancy — so those
  controls are the whole evidence for the statement, and an auditor will test them (§4.3).
- **Remote and mobile working** by Data & More personnel (covered by the Remote work and mobile
  devices theme).
- The **Hetzner EU datacentre facilities (Germany)** that host the SaaS service — in scope as a
  managed dependency through supplier management and the DPA, not as premises Data & More
  physically controls (see 1.3).
- Customer premises and customer datacentres hosting on-premises deployments — an **interface**,
  not a Data & More location (see 1.4).
- **No storage, processing or access from outside the EU/EEA** of the customer personal data
  covered by this scope. With personnel working from Calgary inside the same tenant, this is an
  access-control statement rather than a structural one: it holds exactly as long as those
  controls hold, and any access that is in fact possible from Calgary requires a transfer basis
  under GDPR Chapter V (§4.3).

**d) Information and assets in scope.**

- **Customer personal data (PII)** ingested, scanned, classified or reported on by the
  platform, processed by Data & More as processor or sub-processor.
- **Compliance data** generated by the platform: scan results, classification output,
  processing records, audit logs.
- **Configuration data**: customer-specific settings, dictionaries, taxonomies, connector
  credentials and scan definitions.
- **Platform source code, build artefacts and infrastructure-as-code.**
- **Data & More internal information**: employee, applicant, supplier, financial, contractual
  and ISMS records.
- Information held **outside data systems** (documents, manual records, printed material),
  covered by the Management of data sets theme.

**e) Technology in scope.**

- The **production SaaS platform** at Hetzner, and the separated **development, staging and
  security-testing environments**.
- The **network zones** operated by Data & More: DMZ, internal processing network, database
  network, management network, and the VPN used for administrative remote access.
- **Corporate IT**: identity and access management, Microsoft 365 / Teams (including the
  Cyberday Guidebook and Taskbook apps), endpoints and mobile devices, endpoint protection
  and EDR, logging and monitoring, and backup.
- The **secure development toolchain**: source control, code review, build and release
  pipelines, and vulnerability scanning.
- **Cyberday** itself, as the system of record for the ISMS.

**f) Requirements the ISMS is scoped to meet.**

- **GDPR** (notably Articles 5, 24, 28, 30, 32–34 and 44–49) and the Danish Data Protection Act.
- **Contractual** obligations in customer Data Processing Agreements and in sub-processor DPAs,
  including partner/reseller chains in which Data & More acts as sub-processor.
- **ISO/IEC 27001:2022**, with per-control applicability, status and owner recorded in the
  Statement of Applicability.
- **ISAE 3000 (Revised)**, under which the control environment is described and reported
  (45 control objectives across categories A–I).

These are the only regulatory drivers in scope for the service described in §1.2 b — see
§1.4(4). Because one legal entity also serves North American clients from Calgary, whether any
regime outside the EU/EEA applies to that work, and whether that work is in this scope at all,
is still open (§4.4).

### 1.3 Interfaces and dependencies

| Interface / dependency | What Data & More is responsible for | What the other party is responsible for |
|---|---|---|
| **Customer data sources and connectors** (on-premises and cloud, including Microsoft Purview) | secure connection, least-privilege scan credentials, scanning and classification, reporting back | lawfulness of processing as controller, source-system security, access decisions, remediation decisions |
| **On-premises deployments** | software security, hardening requirements, documented installation and update guidance, support | hosting infrastructure, physical security, network controls, backup, patching of the host environment, local operations |
| **Hetzner Online GmbH** (SaaS hosting, EU/Germany; named in DPA Appendix B) | tenant configuration, encryption, access control, monitoring, backup verification, supplier oversight | datacentre physical security, facility and hardware availability |
| **Microsoft (365 / Teams / Purview-side services)** | configuration, identity and access control, data minimisation | platform security and availability of the service |
| **Cyberday (ISMS system of record)** | ISMS content, ownership, review cycles, access control | ISMS platform security, change logging, availability |
| **Partners / resellers where Data & More is sub-processor** | sub-processor obligations, security requirements, breach notification up the chain | controller or processor duties toward the data subject |
| **Other sub-processors and suppliers** | selection, DPA execution before access, security verification and monitoring (ISAE controls F.1–F.6) | their own internal security management |
| **Customers' own auditors and supervisory authorities** | evidence provision, audit cooperation, breach notification within contractual and GDPR deadlines | audit scope and findings |

The authoritative register of authorised sub-processors is **Appendix B of the Data Processing
Agreement**, which names Hetzner Online GmbH (Gunzenhausen, Germany). The table above is not a
substitute for it and must not drift from it (§4.3).

### 1.4 Exclusions from scope

Stated explicitly so that no reader has to infer them:

1. **Customer-controlled infrastructure hosting on-premises deployments** — servers, network,
   physical security, backup and host patching. Excluded because Data & More has no control over
   it; addressed instead by documented hardening and operating requirements supplied to the
   customer, and by the responsibility split in 1.3.
2. **Customer processing decisions as controller** — the purposes and lawful bases of the
   processing, data subject request outcomes, and remediation decisions. Excluded because they
   sit with the controller; Data & More acts only on documented instructions.
3. **The internal management systems of sub-processors and suppliers.** Excluded as outside the
   organisational boundary; managed through supplier security requirements, DPAs and monitoring
   rather than by direct control.
4. **Processing or storage of customer personal data outside the EU/EEA** — not performed, so no
   transfer controls under GDPR Articles 44–49 are in scope for it. No privacy regime outside
   the EU/EEA applies to that service. This says nothing about the North American client work
   (§4.4), and it depends on the Calgary access controls in §1.2 c holding. Should a future
   customer contract make another regime applicable, the scope and the controls supporting it
   are reviewed before that contract is signed.
5. **Industry-specific ISMS themes** — not excluded by choice of industry. Data & More supports
   customers in all industries and applies the twelve active ISMS themes without
   industry-specific narrowing.
6. **ISO/IEC 27001:2022 Annex A controls assessed as not applicable** — each is justified
   individually in the Statement of Applicability, not excluded at scope level.

Note: no exclusion is claimed for the **North American client work run from Calgary**. It is
the same legal entity's work, so it cannot be excluded on entity grounds, and whether it falls
inside the service described in §1.2 b or needs an exclusion of its own is open (§4.4).

---

## 2. Where v5 was imprecise

| v5 text | Problem | Replaced by |
|---|---|---|
| "focused on: 1. Data Compliance and Privacy Management … 5. Custom Solutions" | lists control topics, not boundaries; nothing is excluded, so nothing is bounded | §1.2 a–f (organisation, services, locations, information, technology, requirements) + §1.4 exclusions |
| "regulations like GDPR, CCPA, and PIPEDA" | "like" is open-ended, and two of the three named regimes had no evidenced customers or controls behind them, while the ISAE description states European customers and no non-EEA transfers | §1.2 f — GDPR and Danish law named as the only regulatory drivers, with contractual obligations alongside them; §1.4(4) records that no regime outside the EU/EEA applies |
| "monitoring and scanning of data sources, both on-premise and in the cloud" | does not say whose data sources, nor who is responsible for the on-premises environment | §1.2 b(1) + the responsibility split in §1.3 |
| "Utilizing solutions for privacy monitoring, AI enterprise platforms, and Microsoft Purview" | mixes Data & More *product capabilities* with how Data & More *governs itself*; "AI enterprise platforms" is undefined | §1.2 b(3), b(5) — stated as in-scope product capabilities, with Purview named as a customer-side integration in §1.3 |
| "custom dictionaries and taxonomies … specific to different organizations" | reads as a sales feature; does not identify the configuration data as an in-scope asset | §1.2 b(2) + §1.2 d (configuration data as a protected asset class) |
| no legal entity, headcount, locations, delivery models, or hosting named | clause 4.3 boundaries cannot be determined | §1.1 and §1.2 a, c |
| no interfaces or dependencies | clause 4.3 requires them where the organisation depends on others | §1.3 |
| no exclusions | an ISMS with no stated exclusions invites scope challenge at audit | §1.4 |
| "for your organization" (closing line) | written to a customer, not to an auditor or interested party, in a document meant for any interested party | removed; §1.1 is written in the third person |

---

## 3. Consistency with the rest of the ISMS

- **ISAE 3000 description of processing** — same entity, same delivery models, same hosting
  (Hetzner EU/Germany), same processor and sub-processor roles, same "no transfers outside
  EU/EEA" statement, and the same supplier oversight controls (F.1–F.6) referenced in §1.3. Two
  facts have moved on since that description was written and are carried here in their current
  form: headcount (27 as of June 2025 → 29, §4.1) and the office footprint, which the ISAE
  description gives only as "Denmark" while this scope names four offices, one of them outside
  the EU/EEA (§4.2). The ISAE description's own "no transfers outside EU/EEA" wording should be
  re-read against the Calgary position in §1.2 c before the next report.
- **Statement of Applicability** — §1.4(6) defers all Annex A applicability decisions to the SoA,
  so the two documents cannot contradict each other.
- **Cyberday ISMS themes** — the twelve active themes all map onto something inside the boundary:
  Risk management and leadership, Personnel security, Data system management, Email and phishing,
  Incident management, Management of data sets, Partner management, Physical security, Privacy,
  Remote work and mobile devices, Software development, Technical cyber security.
- **Operational environment / external and internal issues** (the next section of the Cyberday
  report) needs no change to be consistent with this scope, though "for our clients" in its
  closing sentence has the same second-person drift noted above.

---

## 4. Confirm before publishing

Answered and folded in above: legal entity details, headcount, the office footprint, the
production status of the Purview and AI capabilities, the hosting description, the removal of
the non-applicable privacy regimes, and the organisational boundary — one legal entity covering
all operations including the Calgary office, with one shared Microsoft tenant across them. Six
questions remain; items 3 and 4 are the ones that decide what the scope may claim.

1. **Headcount as-of date.** The figure given was "29 employees as of June 2029", which is a
   future date — today is October 2026. §1.2 a carries 29 with the date withheld. Confirm the
   correct as-of date (June 2026 being the obvious reading), and that 29 includes the Calgary
   personnel now that one entity covers everything.
2. **Office list.** The website's contact page lists Copenhagen, Hamburg, Hässleholm and
   Calgary, while its about page lists Copenhagen, Calgary, Düsseldorf, Zagreb and Stockholm.
   Confirm which set is current and which are Data & More ApS sites rather than partner or
   representative presence — every one of them is now an ISMS location.
3. **Calgary: the controls, and the Chapter V position.** One tenant spans all offices, so
   "no access from outside the EU/EEA" rests entirely on access controls inside that tenant.
   Needed before publishing: (a) what enforces it — conditional access by location, group
   membership, separate data stores, or something else; (b) evidence that no Calgary account can
   reach in-scope customer personal data, including through administrative or support paths;
   (c) if any access is possible, even standing or break-glass administrative access, the GDPR
   Chapter V transfer basis for it. If (c) applies, §1.2 c and §1.4(4) must both be reworded —
   the current text says no such access exists.
4. **Are the North American client engagements in scope?** They are the same legal entity's
   work, so they cannot be excluded on entity grounds, and the scope currently claims no
   exclusion for them. Either they are the service described in §1.2 b delivered to another
   market — in which case the regimes governing those clients belong in §1.2 f, which is where
   the regimes removed earlier would return for that work only — or they are different work that
   needs an explicit exclusion in §1.4 with its own justification. Silence is the one option
   that will not survive an audit.
5. **Sub-processor register.** No list was supplied, so §1.3 still names only Hetzner Online
   GmbH, Microsoft and Cyberday, with DPA Appendix B cited as the register. Confirm the full
   current list so the two agree.
6. **Hosting locations.** §1.1 and §1.2 c say "EU (Germany)", as instructed and as the ISAE
   description has it. The company's own FAQ, however, describes the hosted service as running
   in ISO-certified datacentres in **Germany and Finland**. If Finland is in use for customer
   data, the scope understates the hosting footprint and needs both named.

---

## 5. Publishing in Cyberday

1. Open a new draft of *ISMS description and scope* (v5 → **v6**).
2. Replace the **Scope of the ISMS** section with §1.1–§1.4 above, once Section 4 is resolved.
3. Change description for the version history: *"Scope restated against ISO/IEC 27001:2022
   clause 4.3: boundaries (organisation, services, locations, information, technology,
   requirements), interfaces and dependencies, and explicit exclusions. Narrowed the stated
   regulatory drivers to those that actually apply."*
4. Publish, and re-share the read-only report with top management and the auditor — the scope is
   the first thing read at the opening meeting.
5. Keep the published PDF in this repository so the ISAE and ISO mapping documents stay in step
   with it.
