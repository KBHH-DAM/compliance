# Internal audit 2026 — findings, and what ISO 27001 certification needs

**Source:** email from Simone Sigh, Sjeni (Simone@sjeni.dk), 26 October 2026 16:11, *Opfølgning på
intern audit lukkemøde*. Draft findings from the closing meeting — Simone states explicitly that
these are **not necessarily the final wordings or requirement bases** that will appear in the report.
**Prepared:** 27 October 2026 · Kristian Boe Helweg Hansen, Compliance Manager

**15 findings: 14 Minor nonconformities, 1 Observation.** No major nonconformities.

---

## Read this first: this is the road to ISO 27001 certification

This is the internal audit that precedes **ISO/IEC 27001:2022 certification**, and the "3. parts
dokumentgennemgang" Simone refers to is the certification body's **Stage 1 documentation review**.
That changes what these findings are. They are not a quality score on the ISMS — they are a list of
the things the certification body is about to look for, found early and cheaply by someone on our
side. Her advice to take the document-requirement deviations first is advice about passing Stage 1.

Every document in this repository was built for the **ISAE 3000 Type 1** engagement and for mapping
**Annex A** controls. Certification is a different exercise: it audits the management system in
**clauses 4 to 10**, which the ISAE engagement never touches and which our mapping documents only
enumerate.

| Where the finding sits | Findings | Coverage in this repository |
|---|---|---|
| Management system clauses 4–10 | 1, 2, 4, 5, 10, 12, 13 | Mapped, not implemented |
| Annex A controls | 6, 7, 8, 9, 11 | Mapped, partly documented |
| Cross-cutting / other | 3, 14, 15 | 15 is in progress; 3 is structural; 14 is untouched |

Nothing here is fixed by better mapping. Eleven of the fifteen need a **document or a record that
does not currently exist** — an audit programme, a management review record, a continuity plan, a
legal requirements register, a nonconformity log. `PROJECT_STATUS.md` still says "zero critical gaps
identified"; that was true of the ISAE scope and is not true of the ISMS.

### The findings land almost exactly on the Stage 1 document set

Stage 1 checks the mandatory documented information and whether the ISMS is ready to be audited in
depth at Stage 2. Set the findings against that list and the overlap is not a coincidence — it is
what Simone audited:

| Mandatory documented information | Clause | Status | Finding |
|---|---|---|---|
| ISMS scope | 4.3 | Exists, inadequate — **replacement drafted** | **1** |
| Information security policy | 5.2 | Exists; generic, and silent on sanctions | **3**, **15** |
| Risk assessment and risk treatment **process** | 6.1.2–6.1.3 | Process not applied; results ad hoc | **2** |
| Statement of Applicability | 6.1.3 d) | **Exists** — `ISO 27001_27002_2022 _ Report _ Cyberday_SoA_is_included.pdf` | — |
| Information security objectives | 6.2 | Exist, three required fields empty | **4** |
| Evidence of competence | 7.2 | Exists — training records, skill tests | — |
| Internal audit **programme** and results | 9.2 | Audit done; no programme behind it | **12** |
| Management review results | 9.3.3 | **Nothing could be shown** | **5** |
| Nonconformities and corrective action | 10.2 | **Nothing exists** | **10** |

Six of the nine rows are open, and two of them — **internal audit (9.2) and management review
(9.3.3)** — are the ones a certification body treats as entry conditions rather than findings. Under
ISO/IEC 17021-1 it expects at least one completed internal audit and one completed management review
before it will audit the system in depth. The internal audit has now happened. **The management
review has not, and that is the single hardest gate on this list**, because it cannot be
back-dated and its required inputs do not all exist yet.

### The dependency that reorders everything

Clause 9.3.2 fixes what a management review must consider. Three of its required inputs are
themselves open findings:

- results of internal audits → **finding 12**
- status of nonconformities and corrective actions → **finding 10**
- results of risk assessment and status of the risk treatment plan → **finding 2**

So the management review cannot simply be scheduled and ticked off. Hold it before those three exist
and it is a review with empty inputs, which becomes a Stage 2 finding in its own right — a worse
outcome than not having held it. **Findings 10, 12 and 2 are therefore prerequisites for finding 5**,
and finding 5 is a prerequisite for certification. That chain, not the Minor/Observation grading,
is what should drive the schedule.

---

## Finding 3 is the root cause of several others

> "The documented procedures and own policies are to a high degree generically generated from the
> document management system in use. The content is approved but not adapted to or assessed against
> the organisation, which makes it unclear whether it meets the expected need in terms of ensuring
> the effectiveness of the management system."

This is the most important finding on the list even though it is scored Minor, because it explains
findings 2, 6, 7 and 9 as symptoms rather than separate problems. The Cyberday-generated policies
are generic by construction: `B2 Risk management policy` runs to 1,700+ lines of template guidance,
`B6 B13 Access management and password policy` to 3,800+. They were approved without being cut down
to what Data & More actually does.

Fixing finding 3 properly means going through the policy set and making each document say what this
company does, which is substantial work. Fixing findings 2, 6, 7 and 9 individually without it
produces four more generic documents and the same finding next year.

Two things in this repository already work the way finding 3 asks for, and are worth using as the
pattern: `C5 C6 Offboarding and departure procedure` and `ISMS_SCOPE_STATEMENT.md`. Both are
specific, short, name real roles, and state what is not covered.

---

## The findings, and what each one needs

Effort figures are rough bands for planning, not quotes.

### Priority 1 — document requirements, before the third-party review

| # | Clause | What it says | What exists today | What it needs | Effort |
|---|---|---|---|---|---|
| **1** | 4.3 | Scope description does not clearly establish the ISMS scope; unclear and imprecise because it carries too much information irrelevant to this type of document | **Already drafted.** `ISMS_SCOPE_STATEMENT.md` is a paste-ready replacement for the Cyberday *ISMS description and scope* v5, written against 4.3 — boundaries, applicability, interfaces, dependencies, and what is outside | Work through its *Section 4 — Confirm before publishing*, then publish it in Cyberday as a new version and re-approve | Hours |
| **2** | 6.1.2 | Risk assessment process not implemented to the point of being used; assessments are ad hoc, not based on the established criteria, do not assess consequences of loss of confidentiality, integrity and availability, and the risk score calculation is opaque | `B2 Risk management policy` (generic, Cyberday) and the deleted `Risk management procedure and result preview` export | A risk method that is actually applied: stated criteria, explicit C/I/A consequence scoring, a worked calculation anyone can follow, and at least one real risk assessment produced using it. This is the largest item on the list | Days |
| **4** | 6.2 i), j), l) | Objectives do not establish the resources required, who is responsible, or when results are evaluated — despite Cyberday supporting all three fields | Objectives exist in the information security policy | Fill in the three fields for each objective. The finding notes the system already supports it, so this is data entry, not drafting | Hours |
| **5** | 9.3.3 | Results of management reviews are not documented as required; nothing could be shown | Nothing | A management review record covering the 9.3.2 inputs and 9.3.3 outputs. **Certification entry condition, and blocked on findings 10, 12 and 2**, which are three of its required inputs — see the dependency chain above. Hold it last among the Priority 1 items, not first | Hours, once its inputs exist |
| **10** | 10.2 | Nonconformities not handled per the requirement; no documented information as evidence; handled ad hoc | Nothing | A nonconformity and corrective action log, with the 10.2 fields: the nonconformity, immediate action, cause analysis, action taken, effectiveness check. **These 15 findings are its first entries** — which is the cheapest way to close this one | Hours |
| **12** | 9.2.2 | No internal audit programme planned, established or implemented | This audit happened, but as a one-off | A programme: frequency, scope and method per audit, criteria, who audits, independence, reporting, and a schedule for the next cycle. The audit that produced these findings is the first entry — document it retrospectively and say so. **Certification entry condition**: the audit itself satisfies 9.2.1, but a certification body will look for the programme behind it | Hours |
| **9** | A.5.31 | Legal, statutory and regulatory requirements relevant to information security, and compliance with them, are not documented — requirements are identified but neither they nor compliance are recorded, so neither is updated | Scattered across the DPA redlines, the GDPR mappings and the transfer procedure | A single register: requirement, source, what it obliges, where we meet it, who owns it, when compliance was last checked. Most of the content already exists in this repository and needs collecting, not researching | Hours |
| **13** (Obs) | 4.2 | Interested parties' requirements handled separately through contracts or internal policies; risk that parties and their requirements are overlooked for want of a consolidated overview | Partly implicit in `ISMS_SCOPE_STATEMENT.md` interfaces and dependencies | An interested-parties register. An observation, not a nonconformity — but it is an hour's work and it closes a predictable future finding | Hours |

### Priority 2 — Annex A controls needing procedures

| # | Clause | What it says | What exists today | What it needs | Effort |
|---|---|---|---|---|---|
| **7** | A.5.24–A.5.26 | No clear, understandable documented procedures for assessing and handling information security events and incidents | `I2 Procedure for Personal Data Breach` (GDPR breach, not security incidents generally); Staff Handbook incident section | Separate the two. A personal data breach is a subset of a security incident, and the Handbook's reporting duty is not a handling procedure. Needs: what counts as an event vs an incident, who assesses, categories, escalation, and what is recorded | Days |
| **8** | A.5.29 + A.5.30 | No plan for maintaining information security during disruption; business continuity not planned or tested; no contingency plans or exercise evidence could be shown | `I1 I4 Continuity management policy` (generic, Cyberday) | A plan specific to this business — what breaks, what the recovery target is, who does what — and at least one tabletop exercise with a written record. The finding notes you *do* handle disruptions competently; this is about planning and evidence, not capability | Days |
| **6** | A.5.13 | No procedures for labelling of information implemented | A classification scheme is referenced in the Handbook's *Policies and documents*, but no labelling procedure | A labelling procedure tied to the existing classification levels: what gets a label, how, and what it means in practice. Keep it small — a labelling scheme nobody applies is finding 3 again | Hours |
| **15** | *not stated* | The sanctions process for non-compliance with the information security policy has not been communicated to relevant stakeholders | **In progress.** `EMPLOYEE_SANCTIONS_AND_DISCIPLINARY_PROCEDURE.md` (v0.1 draft), `INFOSEC_POLICY_SANCTIONS_CLAUSE.md` (clause ready to enter in Cyberday), Handbook Item 20(a) applied as pending suggestions | The documents now exist; **communication is the open half**. Approve the procedure, enter the policy clause, accept the Handbook suggestions, then tell staff and record that you did — the record is what closes the finding | Hours, after approval |

### Priority 3 — quick and self-contained

| # | Clause | What it says | What exists today | What it needs | Effort |
|---|---|---|---|---|---|
| **14** | *not stated* | Job applicants cannot access information about the collection and processing of their data before submitting an application | `C3 Privacy_policy_for_job_applications_and_recruitment` exists as a document | Publish it and link it from every job advert and the application form, before submission. The document is written; this is a website task. **Not covered by either website audit document in this repository** | Under an hour |
| **11** | A.7.7 | Own policy requires screens and computers to be locked as soon as they are left; during an interview a computer was left unlocked while the user left the room | Handbook requires screen lock; the policy is correct | A behavioural finding, not a documentation one. Enforce a short automatic lock timeout technically rather than relying on people, and record it in the awareness training. Technical enforcement is the only durable answer | Under an hour |

---

## Logged in Cyberday as nonconformities

All fifteen findings were entered in the Cyberday nonconformity register on **27 October 2026**,
titled `IA2026-nn` so they sort together and so any finding can be traced from the audit report to a
record and from the record to its closure. **Entering them is itself the corrective action for
finding 10** — clause 10.2's retained documented information is the nature of the nonconformities and
the actions taken.

| Finding | Cyberday ID | Title |
|---|---|---|
| 1 | 14560096 | IA2026-01 ISMS scope description does not clearly establish the ISMS scope (4.3) |
| 2 | 14560100 | IA2026-02 Risk assessment process not implemented in practice (6.1.2) |
| 3 | 14560104 | IA2026-03 Policies and procedures generically generated and not adapted |
| 4 | 14560108 | IA2026-04 Objectives do not state resources, responsibility or evaluation (6.2) |
| 5 | 14560112 | IA2026-05 Results of management reviews not documented (9.3.3) |
| 6 | 14560117 | IA2026-06 No procedures for labelling of information implemented (A.5.13) |
| 7 | 14560131 | IA2026-07 No documented procedure for security events and incidents (A.5.24–A.5.26) |
| 8 | 14560137 | IA2026-08 No plan for information security during disruption (A.5.29, A.5.30) |
| 9 | 14560141 | IA2026-09 Legal and regulatory requirements and compliance not documented (A.5.31) |
| 10 | 14560145 | IA2026-10 Nonconformities not handled per the requirement (10.2) |
| 11 | 14560149 | IA2026-11 Computer left unlocked while the user left the room (A.7.7) |
| 12 | 14560153 | IA2026-12 No internal audit programme planned or established (9.2.2) |
| 13 | 14560157 | IA2026-13 (Observation) No consolidated overview of interested parties (4.2) |
| 14 | 14560161 | IA2026-14 Job applicants cannot access processing information before applying |
| 15 | 14560174 | IA2026-15 Sanctions process not communicated to stakeholders |

Each record carries the finding wording, the requirement basis, the state at the time of the finding,
an initial cause analysis, the planned corrective action, an effectiveness check, the owner and the
effort band — written into the description, because the Cyberday API exposes only `title` and
`description`.

### What still has to be done by hand in Cyberday

The structured template fields cannot be set through the API. For each of the fifteen records:

- [ ] **Source of the non-conformity** → internal audit; **finding method** and **date of
      identifying** → 22.10.2026.
- [ ] **Non-conformity level** → *2 – Minor non-conformity* for fourteen of them; finding 13 is an
      **Observation**, so set it to the observation level rather than Minor.
- [ ] **Linked framework section** → the clause or control named in each title. Findings 3, 14 and 15
      have no requirement basis in the draft findings; leave their link empty until it is confirmed
      with Simone, and use the *Reference to another requirement* free-text field for finding 14 if it
      is confirmed as GDPR Article 13 rather than ISO.
- [ ] **Root cause**, **potential consequences** and **recommended immediate remedial action** →
      copy from the corresponding paragraphs in the description, so the fields a report prints from
      are populated rather than only the free text.
- [ ] **Reassign the records.** All fifteen were created under `kbb@dataandmore.com`, the account the
      API authenticated as. The descriptions name the Compliance Manager as owner; the assignment
      should match, and findings 11 and 8 should go to IT and DevOps respectively.
- [ ] **Due dates** → none were set. Set them from the Stage 1 documentation review date once it is
      known.

### Two register problems the audit exposed

1. **Sixteen of the twenty pre-existing nonconformities are Cyberday's generic placeholders** —
   *Missing policy*, *Missing documentation*, *Monitoring inadequacy*, *Management review
   inadequacy* and similar — created in bulk on 15 October 2024 and 30 September 2026 with no finding
   text, no requirement basis and no action. Six of the 2024 entries were still untreated at the gap
   analysis of 29 September 2026. They should be either populated or closed with a stated reason;
   a register where most rows are empty templates is the evidence behind finding 10, and leaving them
   there invites the finding again at Stage 2.

2. **The internal audit 2026 record links to those placeholder titles, not to these findings.** Its
   *Identified non-conformities and other observations* field lists thirteen generic entries. Relink
   it to `IA2026-01` … `IA2026-15`, which is what makes the audit result traceable under clause 9.2.2.

Also note that nonconformity **14509452 "Security guidelines breach"** (21 October 2026, laptop left
unattended without a screen lock) is the same incident as finding 11, recorded during the audit and
linked to A.5.10. `IA2026-11` was created anyway, so that finding 11 is traceable and carries the
auditor's own requirement basis — the two should be cross-linked, and 14509452 relinked to A.7.7,
rather than one of them being deleted.

---

## Three things to raise with Simone before the report is finalised

She has invited this by saying the wordings and requirement bases are not final.

**1. Findings 3, 14 and 15 have no requirement basis stated.** Finding 3's *OMRÅDE / KRAV* cell is
empty; 14 and 15 have an area but no clause. A finding cannot be closed without knowing which
requirement it is measured against, and the clause determines the fix. My reading: finding 3 is 7.5.1
and 4.4; finding 14 is GDPR Article 13 rather than ISO at all; finding 15 is A.6.4 together with
clause 7.4 on communication. Worth confirming rather than guessing, especially 14 — if it is a GDPR
finding it does not belong in an ISO 27001 nonconformity list in the same way.

**2. Finding 11's wording conflates the two halves of A.7.7.** It reads "define rules for keeping
screens locked on storage media" (*holde skærme låst på lagringsmedier*), which merges clear desk
(papers and removable storage) with clear screen. The audit evidence is clearly about an unlocked
screen. Worth asking for that sentence to be reworded, since the report wording is what gets tracked
and re-audited.

**3. Which of these are "deviations with document requirements"?** Simone's prioritisation advice
turns on that phrase, and findings 11 and 14 plainly are not. Confirming her list against the
priority order above avoids spending the first week on the wrong things.

---

## The rate card, and a problem with it

Simone offers herself or a junior consultant, or a combination. From `timepriser_2026.pdf`, rates
excluding VAT:

| | Junior consultant | Consultant | Senior consultant | Executive |
|---|---|---|---|---|
| **DKK/hour** | 1,250 | 1,650 | 1,850 | 2,500 |
| **Who** | Cecilie, Rikke, Simon | **Simone**, Miski, Eva Marie | Louise | Pernille |

Time is recorded to the nearest 5 minutes and invoiced to the nearest quarter hour; 30-day payment;
30 days' notice on price changes.

**The attachment does not match the email.** Simone writes that she has marked the hourly rates in
the file and that the zone surcharges are also in it. Neither is there. The PDF is four pages —
cover, rates and terms, general terms, and a "why us" page — with no highlighting or marking of any
kind, and no zone surcharge anywhere, including in the page images. Ask her for the marked version
before treating the rates above as her quote.

Also worth noting: the terms page states the sales and delivery terms are *valid until 29.08.2026*,
on a document headed *as of 1 January 2026*. Already expired on its face. Minor, but if these terms
are going to govern an engagement, they should be current.

---

## Suggested sequence

The order is set by the dependency chain, not by the grading. Everything in step 1 exists to make
the management review in step 3 real, because that review is the gate.

**Step 1 — this week, in this order.** Finding **10**'s nonconformity log first, because the other
fourteen findings are its first entries and every subsequent fix gets recorded in it. Then finding
**12**'s audit programme, since this audit is its first entry. Then finding **1**, which is drafted
and needs only confirming and publishing, and finding **4**, which is data entry into fields Cyberday
already provides. Four findings closed, days rather than weeks, and two of the three management
review inputs in place.

**Step 2 — the risk method, finding 2.** The third management review input, and the largest single
item on the list. It is also the one Stage 1 reads most closely, because the risk assessment, the
risk treatment plan and the SoA have to hang together: the SoA already exists, so an assessment
produced by a different method than the SoA assumes will show up as an inconsistency between two
documents the auditor reads side by side. Start it as soon as step 1 is moving, and decide the
external-help question before starting it.

**Step 3 — hold the management review, finding 5.** Only once 10, 12 and 2 exist. Cover the full
9.3.2 input list and minute the 9.3.3 outputs. This is the item that converts the others into
certification readiness.

**In parallel, whenever there is a gap:** findings **11** and **14**, under an hour each. Finding 14
is a live GDPR exposure rather than only an audit point, so it should not wait for the schedule.

**Then finding 15**, the only one already half-built. Approving the sanctions procedure unblocks the
policy clause, the Handbook suggestions and the communication record — and the clause also closes an
unrelated ISAE 3000 gap in C.2, so it pays twice.

**Then findings 9 and 13**, both collection exercises over material that already exists in this
repository.

**Then the substantial content:** findings **7** and **8**, which need real procedures and a tested
plan, and finding **3**, the pass over the whole policy set. Finding 3 is the one to start early even
though it finishes late, because it is the finding most likely to recur at Stage 2 in a different
guise.

**Decide the external help question before starting finding 2.** The risk method is the item where an
experienced consultant saves the most time, and it is also the one most likely to be redone if it is
got wrong. A junior consultant at 1,250 is good value for the register and log work (findings 9, 10,
12, 13); Simone at 1,650 is better value on findings 2 and 3.

---

## Open points

- [ ] Confirm the requirement basis for findings 3, 14 and 15 with Simone.
- [ ] Ask for the marked rate card with the zone surcharges, and for current terms.
- [ ] Confirm the date of the Stage 1 documentation review, since it sets the deadline for everything
      in Priority 1. Ask also whether the certification body has been chosen and booked — Stage 1 and
      Stage 2 are normally separated by weeks, and the gap is where corrective actions land.
- [ ] Decide whether a management review has in fact taken place (finding 5). If one has, the record
      is a write-up; if not, it is a meeting that has to happen — and it should be held after
      findings 10, 12 and 2, not before.
- [ ] Check the risk assessment against the existing Statement of Applicability before rebuilding the
      method (finding 2). The SoA is already published; an assessment built on different assumptions
      puts two mandatory documents in conflict.
- [ ] Confirm with Simone whether she will be the internal auditor for the next cycle under the new
      programme (finding 12), or whether using the same firm for both internal audit and remediation
      advice creates an independence problem she would rather avoid.
- [ ] Update `PROJECT_STATUS.md`, which still reports zero critical gaps and predates this audit.
- [ ] Decide the split between internal work and Sjeni, and on which findings.
- [ ] Complete the structured Cyberday fields on the fifteen `IA2026-nn` records, reassign them from
      `kbb@dataandmore.com` to their real owners, and set due dates once the Stage 1 date is known.
- [ ] Relink the internal audit 2026 record in Cyberday from the generic placeholder nonconformities
      to `IA2026-01` … `IA2026-15`.
- [ ] Decide what happens to the sixteen generic placeholder nonconformities, and cross-link
      14509452 to `IA2026-11`.
