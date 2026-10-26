# Staff Handbook Redline — `DAM__Staff_Handbook`

**Prepared:** 13 October 2026
**Target document:** `DAM__Staff_Handbook v5` (Google Doc ID `1fcMm0QNAHIGK8QoWXDnFLgGGX-wvXKoiJzSOY9k-1d0`, single tab titled `DAM__Staff_Handbook v4`)
**Status:** Draft for review — **Items 3, 6 and 12 require factual confirmation before drafting is final**  
**Updated 26 October 2026:** Item 20 added — three cross-references to a disciplinary procedure that did not exist until [`EMPLOYEE_SANCTIONS_AND_DISCIPLINARY_PROCEDURE.md`](EMPLOYEE_SANCTIONS_AND_DISCIPLINARY_PROCEDURE.md) was drafted. **Part (a) is now in the document as pending suggestions**; parts (b), (c) and (d) are not applied.
**Why this document matters for the audit:** [`DESCRIPTION_OF_PROCESSING_ISAE3000.md:307`](DESCRIPTION_OF_PROCESSING_ISAE3000.md) lists the employee handbook as evidence for Control A.1 (Policies), and `:170` lists it again under training. Baker Tilly will read it.
**Companions:** [BYOD controls](BYOD_REMOTE_WORK_ISAE3000_CONTROLS.md) · [BYOD gap remediation](BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md) · [B.3 extension](B3_CONTROLS_EXTENSION_FOR_BYOD_REMOTE_WORK.md)

---

## Applied to the document — 15 October 2026

Items **1, 2, 10, 14 and 19** are accepted and live. Items **4 (part), 9, 12 Variant A, 13 (part), 15, 16, 17 (part) and 18 (part)** are now in the document as **pending suggestions** awaiting review.

| Item | State | Note |
|---|---|---|
| 1 — Document control | ✅ **Live** | Top of document, ahead of the title. Plain paragraphs, not a table. Four approval fields still blank by design. |
| 2 — Contact details | ✅ **Live** | Section before Appendix 1, with address, CVR and Datatilsynet details. |
| 10 — Review and change log | ✅ **Live** | Replaced the stale "We will correct the date and version…" sentence. |
| 14 — Duplicate paragraph | ✅ **Live** | Removed. |
| 19 — Typos | ✅ **Live** | 8 corrections. |
| — Role rename | ✅ **Live** | `Compliance Manager` throughout (7 replacements). |
| — Confidentiality restore | ✅ **Live** | Heading + 2 paragraphs restored after accidental deletion. |
| **12 — BYOD Variant A** | 🟡 **Suggested** | Full 8-section *Remote Work and Personal Devices* body, replacing the old 3-line work-from-home text. Also removes the mangled splice (see below). |
| **5 — Stale BYOD sentences** | 🟡 **Suggested** | The three sentences in *Communication and security* replaced by a cross-reference to the new section; the mobile-only BYOD sentence deleted. |
| **4 — Incident response (part)** | 🟡 **Suggested** | Fixed the circular self-reference; added the 1-hour deadline, the no-penalty clause, and a *What happens next* block restoring the lost assessment and client-notification duties. |
| **9 — Receipt form** | 🟡 **Suggested** | 5-point acknowledgement including BYOD and device-verification consent, plus `Handbook version acknowledged: 5.0`. |
| **15 — Training schedule** | 🟡 **Suggested** | Induction / annual / role-change, with completion records owned by the Compliance Manager. **Phishing simulations omitted** — not a confirmed control. |
| **16 — SAR routing** | 🟡 **Suggested** | Employee-data vs client-data split, with "do not reply to the requester" instruction. |
| 13 — Platform (part) | 🟡 **Suggested** | `G-Suite` → `Gmail` / "Report spam". **Outlook left alone** — needs the stack confirmed. |
| 17 — Table typo (part) | 🟡 **Suggested** | `UX/IU designer` → `UX/UI designer`. **`Sale` left alone** — `replaceAllText` would corrupt `Sales` elsewhere in the document; fix it by hand. |
| 18 — COVID text (part) | 🟡 **Suggested** | "recent negative test" and "red country" generalised to current authority guidance. **Personal Safety section left alone.** |

### A second splice found and repaired

The accepted bad deletion had also welded two paragraphs together across a boundary. The work-from-home paragraph read:

> "All employees work from home, and we only provide office space if their job duties **include sensitive information, the disclosure of which could be construed as a breach of confidentiality.**  It is a condition of your employment that you have a duty of confidentiality to the Company…"

— the head of the work-from-home sentence welded to the tail of the confidentiality paragraph, which also meant the confidentiality text appeared twice once I restored the original. Replacing the whole work-from-home body with Variant A removed the mangled paragraph, so this is now resolved.

**Cause, for the record:** a `deleteContentRange` whose range ended mid-paragraph rather than on a paragraph boundary. Every delete in this pass was aligned to a paragraph boundary, which is why none of them welded anything.

### Still held, and why

| Item | Held because |
|---|---|
| 3 — Probation | Contract term. I guessed "6 weeks"; needs checking against the written statement of particulars. |
| 6 — Staff outside the EU | Factual determination, and may reopen the Art 44–49 gap closed in `PROJECT_STATUS.md`. |
| 7 — Email monitoring | Needs DK legal review. |
| 8 — Criminal records | Needs DK legal review. |
| 11 — Erasure policy | Verify the policy exists under that name before the Handbook cites it; no such file is in this repository. |
| 12 Variant B | VPN-only access, device health verification, monitoring and the revocation SLA are not implemented. |
| 13 — Outlook | Confirm whether calendars really are in Outlook while mail is in Gmail. |
| 15 — Phishing simulations | Confirm the control exists before the Handbook promises it. |
| 17 — Table currency | Reconcile against actual access for the 25-developer population. |

### 🚨 Historical — the two stray deletion suggestions (resolved, with damage)

My second Variant A attempt computed byte offsets from a read that went stale mid-task — the user accepted Items 1/2/10/14/19 in the browser between my read and my write, which removed ~106 characters of struck-through original text sitting *below* the insertion point and shifted everything after it. The two `deleteContentRange` calls therefore landed 106 characters late, on the wrong paragraphs.

I withdrew both of my misplaced insertions. **I could not withdraw the two deletions** — the Google Docs API has no reject-suggestion method, so these require two clicks in the browser:

| Suggestion | Shows as struck-through | Action |
|---|---|---|
| `bkhuxyvgqso9` (339 ch) | Tail of the work-from-home paragraph, the **`Confidentiality` heading**, and its first two paragraphs | ❌ Accepted → text restored |
| `3uup6i2oq8wf` (444 ch) | The whole **`Security incidents and IT readiness`** body — the reporting duty and the assessment paragraph | ❌ Accepted → section rewritten, duties restored via Item 4 |

**Both were accepted rather than rejected, which deleted live clauses.** All lost text has since been restored or replaced — see *Data loss* below and the 15 October status above.

One pending suggestion *is* correct and can be accepted: the `Working from home` → `Remote Work and Personal Devices` heading rename (`7wsevk7sg9p`). But see inconsistency **C-1** before accepting it alone.

### Lesson applied

All further writes to this document use `writeControl.requiredRevisionId`, so a stale write is **rejected** rather than silently misapplied. The two bad deletions predate that change; the cleanup write used it and succeeded.

**Outstanding before these can be accepted:**

1. **Effective date** and **approver name/title** — four approval-dependent fields remain in Item 1 and the change log. These are *correctly* blank until management approves: an unapproved policy with a filled-in approval line is worse than one with a visible gap.
2. **The approver should not be the document owner.** Kristian owns the Handbook as Compliance Manager, so someone else in management must approve it — the existing `Signed: ___ Chief Executive` block suggests the CEO. Owner/approver separation is what makes the approval record meaningful to an auditor.
3. **v4 date** — not recoverable from Drive metadata (`createdTime` is 15 April 2024, and `modifiedTime` was overwritten by this work). Recorded as "date not recorded"; replace if known.
4. **Incident channel.** Item 2's incident block points to *"Notify management immediately, by phone"* — the route that exists today. It deliberately does **not** name an incident email or on-call number, because [`BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md:34`](BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md) records BYOD incident response as a CRITICAL open gap. Upgrade this text when the channel exists — see Item 4.

### 🚨 Data loss — the two bad deletions were accepted, not rejected

**Both bad suggestions were accepted, which deleted live clauses.** Verified 14 October 2026:

| Text | Status |
|---|---|
| `Confidentiality` HEADING_1 | ❌ Deleted → ✅ **restored** |
| "It is a condition of your employment that you have a duty of confidentiality with regards to D&M." | ❌ Deleted → ✅ **restored** |
| "During your employment, you may find yourself in possession of sensitive information…" | ❌ Deleted → ✅ **restored** |
| "If an employee detects threats to, or breaches of, information security… must immediately notify management" | ❌ Deleted — **superseded by rewrite, see below** |
| "The person responsible for the day-to-day management of D&M Information Security shall carry out an assessment…" | ❌ Deleted — **not replaced, see below** |

The Confidentiality section had been reduced to a single orphaned sentence — *"Any such breach of confidentiality would be deemed as gross misconduct…"* — with no heading and no stated obligation to breach. The penalty survived; the duty did not. Restored verbatim from the pre-edit text in `EDIT` mode (not as a suggestion), since undoing my own error is a correction rather than a proposal.

**Two follow-ups in the rewritten `Security incidents and IT readiness` section:**

1. **Circular cross-reference.** The section now contains *"Notify management immediately, by phone, as set out in Security incidents and IT readiness"* — text copied from the Contact details block, now sitting inside the very section it points to. Delete the trailing clause, or point it at the Contact details section.
2. **Lost assessment and external-communication duty.** The deleted paragraph assigned (a) assessment of reported incidents and (b) responsibility for communicating with affected external parties. Neither appears in the new text. Both are directly audit-relevant for the ISAE incident controls — a processor's duty to notify affected clients is the operative obligation. **Item 4** supplies replacement wording for both under *"What happens next"*.

### Two role questions — resolved 14 October 2026

**Decision 1: the role name and the job title are both "Compliance Manager".** Applied as pending suggestions in the Handbook (7 replacements: `Compliance Officer` ×3, `compliance officer` ×2, `Compliance team` ×1, and the old job title in the contact block). Applied directly in [`DESCRIPTION_OF_PROCESSING_ISAE3000.md`](DESCRIPTION_OF_PROCESSING_ISAE3000.md) and [`PROJECT_STATUS.md`](PROJECT_STATUS.md), with the mapping made explicit under *Key Compliance Roles*:

> *"Compliance Manager" is both the role name used throughout this document and the post-holder's job title; the two are deliberately identical, so that this document, the policies, the Staff Handbook and the evidence set all refer to the role by a single name.*

⚠️ **One tidy-up:** the Handbook contact block now reads `Compliance Manager:` / `Kristian Boe Helweg Hansen,` / `Compliance Manager,` — the old job-title line became a duplicate of the label. Delete the second one while reviewing the suggestions. I left it rather than stacking a suggestion on a suggestion.

**Decision 2: no DPO is required under Art 37(1).** Recorded in the Description of Processing as a positive statement rather than an omission, and the `Data Protection Officer` row is removed from the `PROJECT_STATUS.md` team table (its duties folded into the Compliance Manager row). Existing DPO/CEP/FAS certifications are retained in the text, explicitly framed as professional qualifications rather than designation.

**One action remains on this:** write down the *basis*. An auditor will ask why none of the three Art 37(1) conditions is met, and condition (c) — large-scale processing of special categories — needs an explicit answer given that DMCS scans unstructured client data where special categories may be present. The argument is the processor/controller split: D&M does not determine the purposes or means. A one-page memo approved by management closes it, and is cheaper to write now than to improvise during fieldwork.

**The role name and the job title differ.** The audit documentation refers throughout to a *"Compliance Manager"* ([`DESCRIPTION_OF_PROCESSING_ISAE3000.md:176`](DESCRIPTION_OF_PROCESSING_ISAE3000.md), [`PROJECT_STATUS.md:430`](PROJECT_STATUS.md)), while the actual job title is *Customer Success & Data Protection Manager*. The Handbook text now carries both, so an auditor can map them. Worth making that mapping explicit in the Description of Processing too, rather than leaving two names for one role across the evidence set.

**Is D&M claiming a formal Art 37 DPO?** [`PROJECT_STATUS.md:432`](PROJECT_STATUS.md) lists a *"Data Protection Officer"* as a distinct team role with an unfilled `[Name]`. I have deliberately **not** used the term "DPO" anywhere in the Handbook text, because:

- a statutory DPO under Art 37 carries independence requirements, and Art 38(6) prohibits tasks that create a conflict of interest;
- a role combining *Customer Success* with data protection oversight would invite exactly that question, since customer-facing commercial duties can involve determining purposes and means of processing;
- as a processor D&M may well not be required to appoint one under Art 37(1) at all.

If the intention is that this role *is* the DPO, that needs deliberate consideration and probably the DK legal review already flagged for Items 7 and 8. If there is no formal DPO, remove the row from `PROJECT_STATUS.md` so the evidence set does not imply a role that does not exist.

**Not applied, by scope:** Items 3, 4, 5, 6, 7, 8, 9, 11, 12, 13, 15, 16, 17, 18.

> **Note on the TOC.** The new Document Control block sits above the title and is not a heading, so it does not affect the table of contents. The Item 19 heading fix did change a TOC entry — refresh the TOC (right-click → Update table of contents) after accepting, and again after any of the new sections in Item 12 go in.

---

## Consistency check — document as it stands, 15 October 2026

Run against the live text with Items 1/2/10/14/19 accepted. Split into inconsistencies **introduced by this work** and **pre-existing** ones still open.

### Introduced by this work — fix these

**C-1 — Heading rename without its body.** ✅ **Resolved 15 October.** The rename was accepted and Variant A's full body is now suggested beneath it, so title and content match. The mangled splice in the old body is removed by the same change.

**C-2 — The tab is still named `v4`.** The Drive file is `DAM__Staff_Handbook  v5`, the new Document Control block now says **Version 5.0**, and the single tab inside is still titled `DAM__Staff_Handbook  v4`. Three version identifiers, two of which now agree. Rename the tab.

**C-3 — "Compliance team" vs one Compliance Manager.** ✅ *Naming resolved* — now reads *"evaluated every quarter by the Compliance Manager and your manager"* (pending suggestion), which preserves the two-party review. **The substantive point is still open:** with one person holding the compliance role, confirm the employee's own manager genuinely participates in each quarterly access review, because a review performed and approved by the same person is a weak control and this is a sampled test for Control B.6.

**C-4 — "G-drive" vs "shared drive".** 🟡 **Still open.** *Policies and documents* says policies are on the *"D&M G-drive"*; the review section says *"the D&M shared drive."* Same place, two names. `G-Suite` → Gmail is now suggested, but G-drive is untouched pending Item 13's platform confirmation.

**C-5 — Reporting route stated at two levels of detail.** ✅ **Resolved 15 October.** All three places — *Security incidents and IT readiness*, Variant A section 7, and the receipt form — now state the same obligation: notify management by phone, immediately and within 1 hour, including out of hours. The circular self-reference in the incident section is removed.

### Pre-existing and still live

| Ref | Inconsistency | Item |
|---|---|---|
| C-6 | Probation: 3-month period, "initial" review at 6 months | 3 |
| C-7 | *"staff members based on locations in and outside the EU"* vs transfers closed as not applicable | 6 |
| C-8 | Private email use invited, then unlimited right to *"open and read and/or delete"* on resignation | 7 |
| C-9 | *"required to undergo a background check"* vs *"We do not collect information regarding criminal records"* | 8 |
| C-10 | Calendars in **Outlook**, spam via **G-Suite**, policies on **G-drive** | 13 |
| C-11 | BYOD permission covers *"mobile devices"* only, while *"All employees' laptops must be encrypted"* leaves laptop ownership unstated | 5 / 12 |
| C-12 | *"our available erasure policy"* — still unnamed and unlocated | 11 |

### Housekeeping

**Refresh the table of contents** (right-click → Update table of contents). The accepted pandemic-heading fix changed an entry, and the pending section rename will change another. The Document Control block sits above the title and is not a heading, so it will not appear in the TOC — correct.

---

## ⚠️ Read before applying

**1. Do not paste the BYOD section as-is.** Item 12 contains two variants of the new BYOD text: **Variant A (current state)** and **Variant B (post-remediation)**. [`BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md:27-37`](BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md) records VPN-only access, device health verification, real-time monitoring, BYOD incident response and the revocation SLA as **not yet implemented**. A handbook that promises those controls today would create a control-description mismatch — an auditor who tests the claim finds a deviation, which is a worse outcome than the current silence. Apply Variant A now; hold Variant B until the remediation actions land.

**2. Three items are factual questions I cannot answer from the documents.** Items 3 (probation review interval), 6 (staff outside the EU) and 12 (which laptops are company-owned vs. employee-owned) need your confirmation. Proposed wording for those is marked `[CONFIRM]`.

**3. Probation and notice are contract terms.** Item 3 touches the employment contract, not just the handbook. If the written statement of particulars says something different, the contract governs and the handbook must follow it — not the reverse.

**4. Danish-law points need a DK-qualified reviewer.** Items 7 (email monitoring) and 8 (criminal records) involve *funktionærloven*, Datatilsynet guidance and GDPR Art 10. My wording is a drafting starting point aimed at reducing exposure; it is not a legal opinion.

---

## Summary of items

| # | Item | Severity | Type |
|---|---|---|---|
| 1 | No version, date, owner or approval on the document | 🚨 Critical | Document control |
| 2 | Four cross-references to contact details that do not exist | 🚨 Critical | GDPR Art 13 |
| 3 | Probation period contradicts itself | 🚨 Critical | Contract |
| 4 | Incident reporting has no deadline, named role or out-of-hours route | 🚨 Critical | Control / Art 33 |
| 5 | BYOD coverage is one sentence, scoped to mobile devices only | 🚨 Critical | Control A.1 |
| 6 | "Staff outside the EU" contradicts the closed transfers gap | 🔴 High | Consistency |
| 7 | Email monitoring clauses are broader than defensible | 🔴 High | DK law / GDPR |
| 8 | Criminal-records sections contradict each other | 🔴 High | GDPR Art 10 |
| 9 | Receipt form records no handbook version | 🔴 High | Evidence integrity |
| 10 | No annual review or approval statement | 🔴 High | ISO A.5.1 |
| 11 | Dangling reference to an unnamed erasure policy; DPA not named | 🟡 Medium | GDPR Art 13 |
| 12 | **New section: Remote Work and Personal Devices** | — | New text |
| 13 | Mixed Outlook / G-Suite / G-drive platform references | 🟡 Medium | Staleness |
| 14 | Duplicated mobile-PIN paragraph | 🟡 Medium | Editorial |
| 15 | Training section states no frequency | 🟡 Medium | Control C.3 |
| 16 | SAR routing conflates employee and client data subjects | 🟡 Medium | Art 28(3)(e) |
| 17 | Access-rights table: typos, inconsistent marks, currency unverified | 🟡 Medium | Control B.6 |
| 18 | Vestigial COVID and on-premises text in an all-remote company | 🟢 Low | Staleness |
| 19 | Typos and language | 🟢 Low | Editorial |
| 20 | **Three cross-references to a disciplinary procedure that does not exist** — (a) suggested, (b)–(d) held | 🔴 High | ISO A.6.4 / DPA |

---

## Item 1 — 🚨 The document has no version, date, owner or approval

**Severity: critical — self-contradictory, and the cheapest finding on this list to avoid**

### Current text (verbatim, final section)

> **Changes to this Policy**
> We will correct the date and version at the beginning of this Policy if we make any updates or amendments.

### Problem

There is no date or version at the beginning of this Policy. The document opens with a title, a welcome letter and an unsigned `Signed:_________________________________ Chief Executive` block. Meanwhile:

- the Drive file is named `DAM__Staff_Handbook v5`
- the only tab inside it is named `DAM__Staff_Handbook v4`

So the document promises version control, does not implement it, and the two version numbers it does carry disagree. For a company whose product is compliance tooling, an auditor noticing this on page 1 sets the tone for everything after it.

### Proposed insertion (new table, immediately after the title, before the welcome letter)

> | | |
> |---|---|
> | **Document** | D&M Staff Handbook |
> | **Version** | 5.0 |
> | **Effective date** | `[date of approval]` |
> | **Supersedes** | Version 4.0 |
> | **Document owner** | Compliance Manager |
> | **Approved by** | Management, `[date]` |
> | **Review cycle** | Annually, or on material change to employment terms or security controls |
> | **Next review due** | `[effective date + 12 months]` |
> | **Classification** | Internal |

### Why

ISO 27001:2022 A.5.1 expects policies to be defined, approved, published, communicated and reviewed at planned intervals. [`ISO_27001_2022_ISAE_3000_Mapping.md`](ISO_27001_2022_ISAE_3000_Mapping.md) carries that through to the ISAE control set. A policy document with no approval record cannot evidence any of those five verbs. Also rename the tab to match the file so the two version numbers agree.

---

## Item 2 — 🚨 Four cross-references point to contact details that do not exist

**Severity: critical — straight GDPR Art 13 transparency failure**

### Current text (verbatim, four separate places)

> …you can always withdraw your consent by contacting us at **the contact details listed at the end of this Policy**.

> Please use **the contact details at the end of this Policy** if you have any questions about our retention of your personal data.

> Please use **the contact details at the end of this document** if you wish to make use of your rights as described above.

> …if you wish to file a complaint, you can do so by contacting **the national Data Protection Agency**.

### Problem

The document ends with Appendix 1, the receipt form. There are no contact details anywhere in it. Every route the GDPR sections offer an employee — withdraw consent, ask about retention, exercise data subject rights — terminates in a reference to information that was never written. The complaint route names no authority.

An employee cannot exercise rights the handbook grants them. That is the substance of Art 13(1)(a)–(b) and 13(2)(b)–(d), and it is visible without the auditor having to test anything.

### Proposed insertion (new section, immediately before Appendix 1)

> ## Contact details
>
> **For questions about your employment, your terms, or anything in this Handbook**
> Your line manager, in the first instance.
>
> **For questions about how we process your personal data, to exercise your data subject rights, or to withdraw a consent**
> Compliance Manager, Data & More ApS
> `[postal address]`
> `[email]` · `[phone]`
>
> We will respond to requests concerning your rights without undue delay and in any event within one month of receipt.
>
> **To report a security incident, a suspected incident, or a lost or stolen device**
> See *Security incidents and IT readiness* — use the reporting route given there, which is monitored outside business hours. Do not wait to raise an incident through your line manager if they are unavailable.
>
> **If you wish to complain about our processing of your personal data**
> You may contact the Danish Data Protection Authority:
> Datatilsynet, Carl Jacobsens Vej 35, 2500 Valby, Denmark
> `dt@datatilsynet.dk` · +45 33 19 32 00 · `www.datatilsynet.dk`
>
> Employees based outside Denmark may instead contact the supervisory authority in their country of residence or place of work.

### Why

Closes all four dangling references at once. Naming Datatilsynet satisfies Art 13(2)(d), which requires the right to lodge a complaint *with a supervisory authority* to be communicated meaningfully. The last line matters given Item 6.

---

## Item 3 — 🚨 Probation period contradicts itself

**Severity: critical — the stated sequence is impossible**

### Current text (verbatim)

> All new staff are subject to a probationary period of **3 months**. An initial informal review will take place after **6 months** with your line manager. Your appointment will be confirmed on satisfactory completion of the **3 month** period.

### Problem

The "initial" review falls three months after probation has already ended and the appointment has already been confirmed. One of the two numbers is wrong, and an employee reading this cannot tell when they are being assessed or when they become permanent.

### Proposed replacement `[CONFIRM]`

> All new staff are subject to a probationary period of 3 months. An initial informal review will take place after **6 weeks** with your line manager, so that you have a clear picture of your progress while there is still time to act on it. Your appointment will be confirmed on satisfactory completion of the 3-month period. During this probationary period you will be given appropriate support and development opportunities to help you reach the required standards.

### Why

A mid-probation review is the only reading that makes the sentence coherent, and 6 weeks is the natural midpoint of a 3-month probation — but **this is a guess**. The alternative is that probation is genuinely 6 months and "3 months" is the error. Check the written statement of particulars issued to employees: whichever the contract says is the one that governs, and the handbook must be conformed to it rather than the other way round. Under *funktionærloven* the probation and notice interaction has consequences, so do not resolve this by editing the handbook alone.

---

## Item 4 — 🚨 Incident reporting cannot meet your own detection target

**Severity: critical — the control as written is unachievable**

### Current text (verbatim, and three similar instances elsewhere)

> If an employee detects threats to, or breaches of, information security, or suspects it, he or she must immediately notify **management** of this.
>
> The person responsible for the day-to-day management of D&M Information Security shall carry out an assessment of the reported security incidents **as soon as possible** after they have been notified.

Elsewhere: *"contact your manager immediately"* (viruses), *"report… immediately to your line manager"* (data breach), *"refer this immediately to your line manager"* (SAR).

### Problem

Every reporting route in the Handbook is a person — "management", "your line manager" — with no named role, no contact method, no out-of-hours channel and no deadline. "Immediately" and "as soon as possible" are not testable.

[`BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md:147-180`](BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md) rates absent BYOD incident response as **CRITICAL** and sets out the failure case explicitly: infection Friday 17:00, exfiltration over the weekend, noticed Monday morning — *"~16 hours of undetected compromise"* against a target of *"Detection within 1 hour (not 16 hours)"*. A reporting chain that depends on a line manager reading a message cannot deliver one-hour detection on a Friday evening.

GDPR Art 33's 72-hour clock also starts when the **controller** becomes aware. As a processor you owe notification to the client "without undue delay" — so the internal lag between an employee noticing and the Compliance Manager knowing is pure deduction from the time available to the client.

### Proposed replacement

> ## Security incidents and IT readiness
>
> ### Your duty to report
>
> If you detect, suspect, or are merely unsure about a threat to or breach of information security, you must report it. This includes:
>
> - malware, ransomware or unexpected behaviour on any device you use for work
> - a lost or stolen device, or a device out of your control for any period
> - a phishing message you clicked, replied to, or entered credentials into
> - credentials you believe may have been exposed, including SSH keys and access tokens
> - personal data sent to, or accessible by, the wrong recipient
> - anyone asking you for access or information in a way that feels wrong
>
> **Report within 1 hour of becoming aware, including outside working hours and at weekends.**
>
> ### How to report
>
> | | |
> |---|---|
> | **Primary route** | `[incident email / channel]` — monitored `[hours]` |
> | **Out of hours** | `[on-call phone number]` |
> | **If you cannot reach either** | Any member of management, by phone |
>
> Report to the channel first and your line manager second. Do not wait for your line manager to be available, and do not wait until the next working day.
>
> ### You will not be penalised for reporting
>
> You will never be disciplined for reporting an incident in good faith, including one you caused yourself — a mistake reported in the first hour is a manageable problem, and the same mistake reported on Monday may not be. Failing to report, or delaying a report, is a disciplinary matter.
>
> ### What happens next
>
> The Compliance Manager assesses every reported incident, and records it in the incident log with the time of report, the time of assessment and the action taken. Where a client's data may be affected, D&M notifies that client without undue delay under the terms of the relevant Data Processing Agreement; the Compliance Manager owns that communication. You may be asked to disconnect a device, change credentials, or stop work on a system while the assessment is carried out — do so immediately, even if you believe the report will turn out to be a false alarm.

### Why

Gives employees a named channel, a deadline, and an explicit out-of-hours route — the three things that convert "immediately" into something an auditor can test against the incident log. The no-penalty clause is there for a practical reason: the Friday-evening scenario only works if the developer who clicked the link is willing to say so at 17:05 on a Friday.

---

## Item 5 — 🚨 BYOD coverage is one sentence, and it covers the wrong devices

**Severity: critical — this is the largest gap between the Handbook and your own control documentation**

### Current text (verbatim — the entire BYOD treatment)

> PCs and mobile devices that connect to your company's network and systems remotely must comply with company guidelines.
>
> All employees' laptops must be encrypted and use vpn certificates when accessing the company's data, network and customer systems.
>
> Employees may use their own **mobile devices** (Bring Your Own Device, BYOD) as long as they comply and can document that security measures are maintained.

Plus, under *Working from home*, in full:

> D&M work from home policy applies to all our employees.
> **All employees work from home.**
> All employees work from home, and we only provide office space if their job duties permit it. For example, if people are obliged to come in direct physical contact with customers. But employees must carry out most of their work on a computer off-site.

### Problem

Three defects, compounding:

**The BYOD permission is scoped to "mobile devices" only.** [`BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md`](BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md) describes a **25-developer BYOD environment** — laptops, with SSH keys on them. The Handbook's BYOD sentence does not reach laptops at all.

**The laptop sentence is ambiguous about ownership.** *"All employees' laptops must be encrypted"* — company-issued laptops, or the employees' own? If BYOD laptops are in scope, this is an unenforced requirement on personal property; if they are not, the 25 developers are working on devices the Handbook never addresses. "Must comply with company guidelines" does not say which guidelines or where to find them.

**"Comply and can document that security measures are maintained" puts the burden on the employee and defines nothing.** [`BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md:109-143`](BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md) anticipates exactly this exchange:

> **Your Current Answer:** "They signed an agreement to maintain antivirus."
> **Auditor:** "That's a policy statement, not proof. Show me technical evidence."

Measured against the Control A.1 requirements at [`BYOD_REMOTE_WORK_ISAE3000_CONTROLS.md:132-157`](BYOD_REMOTE_WORK_ISAE3000_CONTROLS.md), the Handbook omits: allowed devices and minimum OS versions; what data may be accessed from a personal device; the auto-lock interval (specified as 5 minutes there, the Handbook says "screen lock" with no number); authorised locations and the public-WiFi restriction; what to do if a device is lost or stolen; and employee acknowledgement of device health verification. It also never mentions SSH key handling, which is the lead finding of the gap analysis.

Finally, *Working from home* is three lines, one of which repeats its own heading. Remote work is not a perk here — it is the **primary control context** for the entire ISAE engagement, and it gets less space than online meeting etiquette.

### Proposed fix

Replace the *Working from home* section and the three BYOD sentences with the new section drafted at **Item 12**. Delete the three sentences from *Communication and security* and cross-reference the new section instead, so there is one authoritative statement rather than two partial ones.

---

## Item 6 — 🔴 "Staff outside the EU" contradicts the closed transfers gap

**Severity: high — two audit documents disagree on a fact**

### Current text (verbatim, *About the Company*)

> We have a workforce of dedicated staff members based on locations **in and outside the EU**.

### Problem

[`PROJECT_STATUS.md:41`](PROJECT_STATUS.md) closes the international transfers gap as:

> | International Transfers (Art 44-49) | ✅ Closed | **Not applicable** - Hetzner EU + on-prem | No action needed |

The Handbook's GDPR section also defers the question rather than answering it: *"If you have any questions about… transfer of data to countries or international organizations outside the EU/EEA, please contact us for more information or documentation of our legal basis."*

An auditor holding both documents will ask how transfers are "not applicable" when staff outside the EU access systems containing client personal data. Remote access from a third country is a transfer. The gap closure may well be correct — but it is justified on infrastructure location (Hetzner EU, on-premises) and does not address personnel location at all.

### Proposed approach `[CONFIRM]`

Do not redraft the sentence until the underlying position is settled. Two possible resolutions:

**If non-EU staff do not access client personal data** — say so explicitly in both documents:

> We have a workforce of dedicated staff members based in and outside the EU. Access to systems containing client personal data is restricted to personnel located within the EU/EEA; roles based outside the EU/EEA do not have such access, and the access rights table in *Data Protection and Access to Information* reflects this.

**If they do access it** — the `PROJECT_STATUS.md` gap closure is wrong and needs reopening, with a transfer basis (SCCs plus a transfer impact assessment) documented per country. That is a materially larger piece of work than a handbook edit, which is why this item is flagged rather than drafted.

### Why

Of everything in this redline, this is the item most likely to generate an audit finding that cannot be closed by editing text, because it is a question about what actually happens. Worth resolving early.

---

## Item 7 — 🔴 The email-monitoring clauses are broader than defensible

**Severity: high — DK employment law and GDPR exposure**

### Current text (verbatim, three separate places)

> If the employee is absent, **the head of department may allow others to access the mailbox** to ensure continuous case handling.

> It is accepted that employees use work email for private correspondence. These should be marked with Private or Personal to ensure that there is no improper reading of private emails.

> **Upon resignation**
> D&M reserves the right to open and read and/or delete e-mail messages sent to the employee.

### Problem

Taken together these three invite private correspondence into the mailbox, then reserve an unlimited right to read it. The resignation clause has no stated purpose, no authorising role, no time limit, no carve-out for the "Private" marking the Handbook itself told employees to use, and no retention period for the mailbox. "Messages **sent to** the employee" also reaches inbound mail from third parties who never consented to anything.

Datatilsynet's published guidance on employee email runs the other way: on departure, close the account and use an auto-reply or a limited redirect, rather than reading the contents; any access needs a defined purpose and proportionality, and the employee should be informed in advance. The absence clause has the same defects in a milder form — "the head of department may allow others" names no criteria and leaves no record.

### Proposed replacement

> ### Access to your mailbox
>
> Your work mailbox is a D&M working tool and D&M property. In narrow and defined circumstances we may need to access it. This section tells you when, who decides, and what we will not do — so that you can rely on it.
>
> **While you are employed.** If you are absent and a case cannot wait, the Compliance Manager may authorise a named colleague to access your mailbox for the sole purpose of continuing that case. Access is limited to what is necessary, is logged (who, when, why), and you are informed on your return, or sooner where practicable. Messages marked *Private* or *Personal* are not opened.
>
> **When you leave.** Your mailbox is closed on your last working day. For up to `[3]` months afterwards:
>
> - an auto-reply directs senders to a named colleague;
> - inbound mail may be redirected to your line manager **for the purpose of continuing business correspondence only**;
> - messages marked *Private* or *Personal*, and messages that are evidently private in nature, are not opened, and are deleted unread.
>
> At the end of that period the mailbox and its contents are deleted, except for individual messages that must be retained as business records (for example, contractual correspondence) or to comply with a legal obligation. Retained messages are held under our erasure policy, not indefinitely.
>
> **What we do not do.** We do not read your mailbox for general monitoring, performance assessment, or curiosity. We do not read messages marked *Private* or *Personal*. Access outside the circumstances above requires a documented decision by management and a specific lawful basis — for example, a credible suspicion of serious misconduct or a legal obligation — and you will be informed unless doing so would defeat the purpose.
>
> **Private use.** You may use your work email for occasional private correspondence. Mark such messages *Private* or *Personal*, which is what keeps them outside the access described above. We recommend keeping genuinely private correspondence in a personal account.

### Why

Keeps the business capability — case continuity, business records — while adding the four things the current text lacks: purpose limitation, a named authoriser, a retention cap, and a carve-out that gives the "Private" marking actual effect. The last point is the most important: the current Handbook invites private use, instructs employees to mark it, and then reserves a right that ignores the marking entirely. **A DK-qualified reviewer should confirm the retention window and the misconduct carve-out.**

---

## Item 8 — 🔴 The criminal-records sections contradict each other

**Severity: high — GDPR Art 10 is strict about this category**

### Current text (verbatim, two sections ~95 paragraphs apart)

> **Criminal Records Checks**
> **All employees of D&M are required to undergo a background check** which could be a criminal record check. Due to the nature that we are working with vulnerable data. Should this be a problem, we will discuss the situation with you prior to confirming your appointment (or relevant change to your job).

> **We do not collect information regarding criminal records** and similar from you but you have to show it to your line manager in the hiring process. We reserve the right to collect such data at a later stage, in which situation we will collect your consent hereto.

### Problem

One section requires a check; the other says the data is not collected. Both can be true at once — inspect the certificate, record only the outcome, retain nothing — but the Handbook never says that, so a reader cannot tell which applies, and an auditor cannot tell what the control is. The second sentence is also garbled (*"Due to the nature that we are working with vulnerable data"* is not a sentence), and relying on **consent** for criminal-record data in an employment relationship is weak, because consent must be freely given and an employee is rarely in a position to refuse.

### Proposed replacement (merge into the *Criminal Records Checks* section; delete the duplicate paragraph from the GDPR section and cross-reference)

> ## Background and criminal record checks
>
> Because D&M processes personal data on behalf of its clients, all candidates are asked to present a criminal record certificate (*straffeattest*, or the equivalent in your country of residence) to their prospective line manager before appointment is confirmed, and again on a material change of role.
>
> **What we retain.** Your line manager inspects the certificate and records only the date of inspection and whether the outcome was satisfactory. **We do not take a copy of the certificate and we do not record its contents.** The certificate is returned or destroyed immediately after inspection.
>
> **Legal basis.** We carry out this check in reliance on our legitimate interest in ensuring that personnel with access to client personal data are suitable for that access (Art 6(1)(f) GDPR), and within the limits that Art 10 GDPR and Danish law place on the processing of criminal-record data. We do not rely on your consent for this check, because we recognise that consent given to an employer may not be freely given.
>
> **If something comes up.** A record does not automatically bar you from employment. We will discuss the situation with you before any decision is taken, and we will consider what the record relates to, how long ago it was, and its relevance to the role you have applied for.

### Why

Makes the inspect-but-do-not-retain position explicit, which is the defensible reading of what you already do, and removes the reliance on employee consent. **Confirm with a DK-qualified reviewer** that the legitimate-interest basis holds for your roles and that Art 10's "authorised by law" condition is met — this is the point on which the drafting is most likely to need adjustment.

---

## Item 9 — 🔴 The receipt form records no handbook version

**Severity: high — undermines the only acknowledgement evidence you have**

### Current text (verbatim, Appendix 1)

> | Name: | |
> | Designation: | |
> | Place of Work: | |
> | Line Manager: | |
>
> I confirm I have received a copy of the D&M Staff Handbook and that I have read this and understood the contents.
>
> I also confirm that I have sought clarification from my line manager on any issues outlined in the Handbook which I am not clear about.
>
> Signed: ___ Date: ___

### Problem

The form proves that an employee signed *a* handbook, not *which* handbook. With no version field, and with the document itself carrying no version (Item 1), you cannot demonstrate which text any employee actually accepted. [`BYOD_REMOTE_WORK_ISAE3000_CONTROLS.md:159-164`](BYOD_REMOTE_WORK_ISAE3000_CONTROLS.md) lists *"Employees acknowledge (signatures)"* as a thing the auditor will check — and the check is only meaningful if the signature ties to a version.

It also does not acknowledge the BYOD and remote-work terms, which is the acknowledgement that actually matters: device health verification against personal property needs a documented, signed basis.

### Proposed replacement

> # Appendix 1 — Confirmation of Receipt of Handbook
>
> **Data & More ApS**
>
> | | |
> |---|---|
> | Name | |
> | Job title | |
> | Place of work | |
> | Line manager | |
> | **Handbook version acknowledged** | **5.0** |
>
> I confirm that:
>
> 1. I have received, read and understood the D&M Staff Handbook, version 5.0.
> 2. I have sought clarification from my line manager on any point I was not clear about.
> 3. I understand and accept the requirements in *Remote Work and Personal Devices (BYOD)*, including the device security requirements, the restrictions on where and how I may access D&M and client data, and my obligation to report a lost or stolen device and any suspected security incident within 1 hour.
> 4. **Where I use a device I own to access D&M or client systems**, I understand that D&M verifies the security posture of that device as a condition of access, that access may be restricted or withdrawn if it cannot be verified, and that D&M may require me to remove D&M and client data from the device. I understand what D&M can and cannot see on my device, as set out in that section.
> 5. I understand that these requirements may be updated, that I will be notified of material changes, and that I may be asked to re-acknowledge a later version.
>
> Signed: ______________________  Date: ______________
>
> Please return this form, completed and signed, to your line manager. A copy is retained in your personnel file as a record of acknowledgement.

### Why

Point 4 is the operative addition. You cannot run pre-connect antivirus and patch checks on someone's personal laptop on the strength of a sentence saying they "can document that security measures are maintained". Signed acknowledgement of the specific intrusion is what makes Option C at [`BYOD_REMOTE_WORK_ISAE3000_CONTROLS.md:212-230`](BYOD_REMOTE_WORK_ISAE3000_CONTROLS.md) — your recommended approach — enforceable rather than aspirational.

Re-acknowledgement will be needed from all staff on publication of v5. That is also the cleanest way to produce a complete, dated evidence set for Control A.1 in one pass.

---

## Item 10 — 🔴 No annual review or approval statement

**Severity: high — ISO 27001 A.5.1**

### Current text (verbatim)

> **Changes to this Policy**
> We will correct the date and version at the beginning of this Policy if we make any updates or amendments.

### Problem

The only commitment is to update a version number that does not exist. There is no review cycle, no approver, no owner, and no mechanism for telling employees that something changed. The Handbook elsewhere promises that *"D&M reserves the right to change its terms & conditions and employment policies from time to time. You will be notified at the earliest opportunity"* — but nothing connects that promise to a process.

### Proposed replacement

> ## Review and changes to this Handbook
>
> This Handbook is owned by the Compliance Manager and approved by management. It is reviewed at least **annually**, and additionally whenever there is a material change to employment terms, to our security controls, or to applicable law. The version, effective date and approval are recorded in the table at the front.
>
> When we make a material change we notify all affected employees, publish the new version on the D&M shared drive, and where the change affects your obligations we ask you to acknowledge the new version using the form at Appendix 1. Minor corrections — typographical fixes, updated contact details — are made without re-acknowledgement and recorded in the change log below.
>
> ### Change log
>
> | Version | Date | Summary of changes | Approved by |
> |---|---|---|---|
> | 5.0 | `[date]` | Document control added; contact details added; Remote Work and Personal Devices (BYOD) section added; incident reporting route and 1-hour deadline added; mailbox access clarified; background check clarified; receipt form extended | `[name]` |
> | 4.0 | `[date]` | `[prior version — details if known]` | |

### Why

The change log is what lets an auditor reconcile a signed receipt form against the text that was in force on the date of signature. Without it, Item 9's version field has nothing to point at.

---

## Item 11 — 🟡 Dangling erasure-policy reference

**Severity: medium**

### Current text (verbatim)

> We refer to **our available erasure policy** for the specific retention periods.

### Problem

The erasure policy is neither named nor located, and the Handbook does not say how an employee would find it. The same section also says *"D&M IT security policy, classification, and other guidelines, as well as guides are available on D&M G-drive"* — so there is a location convention, just not applied here.

### Proposed replacement

> We refer to the **D&M Erasure and Retention Policy**, available on the D&M shared drive alongside our other policies, for the specific retention periods that apply to each category of employee data. If you would like to be shown the retention period for a particular category, ask the Compliance Manager.

### Why

Retention periods are a routine audit request and a routine employee question. Also verify the policy exists under that name — if it does not, the Handbook is referring to a document that was never written, which is a larger problem than the wording.

---

## Item 12 — New section: Remote Work and Personal Devices (BYOD)

This replaces the *Working from home* section in its entirety, and the three BYOD/laptop sentences currently sitting in *Communication and security*.

> ### ⚠️ Apply Variant A now. Variant B is for after remediation.

The gap analysis records the following as **not yet in place**: VPN-only access, device health verification, real-time monitoring, BYOD incident response, access revocation SLA. Variant A states only what is true today. Variant B adds the enforcement language once the controls exist. Publishing B early would mean the Handbook describes controls that testing would not find.

---

### Variant A — current state (apply now)

> # Remote Work and Personal Devices
>
> D&M is a remote-first company. Almost all work is done away from a D&M office, and for many colleagues on a device they own themselves. That makes the security of your working environment a shared responsibility in a way it would not be in an office, and this section sets out your part of it.
>
> It applies to every device you use to access D&M systems, D&M data, or client data — whether D&M provided it or you own it.
>
> ## 1. Where you work
>
> You may work from home or from another private location of your choosing. When you do:
>
> - **Position your screen so that others cannot read it.** This applies to family members and housemates as well as strangers.
> - **Lock your screen whenever you step away**, even briefly, and even at home.
> - **Treat public and semi-public spaces as unsuitable for client data.** You may work from a café, co-working space, train or airport, but **do not open, download or discuss client personal data there**. General work — writing, internal documents, meetings without client data on screen — is fine.
> - **Do not use public or untrusted Wi-Fi for access to D&M or client systems.** Use your home network, a trusted network, or your phone's mobile hotspot.
> - **Take calls and meetings where you cannot be overheard** when client matters, personal data or commercially sensitive topics are discussed.
> - **Do not print client personal data** on a home or public printer. If you believe you need to, speak to the Compliance Manager first.
>
> If you intend to work from outside your usual country of residence for more than a few days, tell your line manager and the Compliance Manager **before** you travel. This is not about where you choose to be — it is that access to client personal data from outside the EU/EEA raises data protection questions we must resolve in advance.
>
> ## 2. Your home network
>
> - Change the default administrator password on your router.
> - Use WPA2 or WPA3 encryption on your Wi-Fi, with a password you have set yourself.
> - Keep your router's firmware up to date where your provider does not do this automatically.
> - Do not place work devices on a guest network shared with unknown users.
>
> ## 3. Devices you use for work
>
> Any device you use for D&M or client work — yours or ours — must meet all of the following. If a device cannot meet them, do not use it for work.
>
> | Requirement | Detail |
> |---|---|
> | **Supported operating system** | Receiving security updates from the vendor. Devices past end-of-support may not be used for work. |
> | **Updates applied promptly** | Security updates for the OS and for your browser, within **14 days** of release. Enable automatic updates where you can. |
> | **Full-disk encryption** | BitLocker (Windows), FileVault (macOS), LUKS (Linux), or equivalent. **On at all times** — not merely available. |
> | **Antivirus / anti-malware** | Installed, running, and receiving definition updates. The OS built-in product is acceptable where it is current and enabled. |
> | **Host firewall** | Enabled. |
> | **Screen lock** | Automatic lock after **no more than 5 minutes** idle, requiring a password, PIN, or biometric to unlock. |
> | **Account separation** | Work is done in your own user account. Not a shared account, not a guest account, not an administrator account used for day-to-day work. |
> | **No shared use** | Nobody else — family included — uses the account you work in. |
>
> Phones and tablets used for work email or messaging must additionally have a **PIN of at least 6 digits** (or biometric unlock) and device encryption enabled.
>
> ## 4. Credentials, keys and tokens
>
> - **MFA** is required on every D&M account and service that supports it. Do not disable it.
> - Use a **unique passphrase for every D&M account**. Use the password manager D&M provides to make that practical — do not reuse passphrases, and do not keep them in a notes app, spreadsheet, or browser profile synced to a personal account.
> - **SSH keys, personal access tokens and API keys are credentials and deserve the same care as your password.** Specifically:
>   - protect every SSH private key with a passphrase;
>   - do not copy keys between devices, do not email them, and do not store them in cloud sync folders;
>   - generate a separate key per device, so that one device can be revoked without affecting the others;
>   - tell `[incident channel]` **within 1 hour** if a device holding a key is lost, stolen, or possibly compromised, so the key can be revoked.
> - Never share an account or credential with a colleague. If someone needs access, they get their own.
>
> > **Why keys get their own paragraph.** MFA protects you when you log in to a web interface. It does not protect a private key sitting in a folder on your laptop — malware that reads that key can clone and push to repositories without ever meeting an MFA prompt. On a personal device, that key is the single most valuable thing an attacker can take.
>
> ## 5. Keeping work data off your own device
>
> Where D&M provides a remote or browser-based way to do a task, use it rather than copying data locally.
>
> - **Do not store client personal data on a device you own.** Work on it in the systems D&M provides.
> - **Do not move D&M or client data into personal accounts or services** — personal cloud storage, personal email, personal note-taking apps, personal AI assistants or chatbots.
> - As stated under *Information*, you may not store company data in a private cloud repository such as Dropbox unless D&M provides it or management has approved it for corporate use.
> - **Do not use removable media** (USB sticks, external drives) for D&M or client data without the Compliance Manager's approval.
> - If you find you have a local copy of client data you no longer need, delete it, and tell the Compliance Manager if it had been there a while or you are unsure what it contained.
>
> ## 6. What D&M can and cannot see on a device you own
>
> If you use your own device for work, you are entitled to know where the boundary sits.
>
> **D&M may:**
>
> - verify that your device meets the requirements in section 3 before granting or continuing access;
> - log your access to D&M and client systems — who, when, from which network, and what was accessed;
> - require you to remove D&M and client data from your device, and to confirm that you have done so;
> - restrict or withdraw your access if a requirement is not met or cannot be verified;
> - require the return or destruction of D&M and client data when you leave.
>
> **D&M does not:**
>
> - read your personal files, photos, messages, or browsing history;
> - monitor your device outside its use of D&M systems;
> - track your location;
> - remotely wipe your personal device, or any part of it other than D&M and client data;
> - install software that gives D&M general control of a device you own.
>
> If you would prefer not to use your own device on these terms, speak to your line manager about a D&M-provided device. Using your own device is a convenience offered to you, not a condition of your employment.
>
> ## 7. If a device is lost, stolen, or you think something is wrong
>
> **Report within 1 hour** — see *Security incidents and IT readiness* for the channel, including out of hours.
>
> Report a device that is lost or stolen, that was out of your control for a period (left in a repair shop, a hotel room, a checked bag), that is behaving oddly, or on which you clicked something you should not have. Report it even if you are not sure, and even if you expect to find it later. We would far rather revoke a key unnecessarily than discover on Monday that we should have revoked it on Friday.
>
> You will not be penalised for an honest report. Not reporting is the disciplinary matter.
>
> ## 8. When you leave
>
> Before your last working day, if you have used your own device for work:
>
> - delete all D&M and client data from it, including local repository clones, downloads, and cached files;
> - remove D&M accounts from your mail, calendar and messaging applications;
> - delete SSH keys and access tokens relating to D&M systems;
> - confirm to your line manager that you have done so.
>
> D&M revokes your access on your last working day. See *Leaving the Company* for D&M-owned equipment.

---

### Variant B — additions once remediation lands

Fold these in as each control goes live. Each is tied to the gap it closes.

**Add to section 1** *(closes the VPN-only gap,* [`:76-105`](BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md)*)*

> **All access to D&M and client systems, including source code repositories, goes through the D&M VPN.** Connect to the VPN first; access from outside it is blocked rather than discouraged. This is why the public Wi-Fi restriction above is enforceable rather than advisory: on the VPN, your traffic is encrypted regardless of the network you are on.

**Add to section 3** *(closes device health verification,* [`:109-143`](BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md)*)*

> **These requirements are verified automatically, not self-declared.** When you connect, D&M checks that your antivirus is running, your OS patches are current, your firewall is enabled and your disk is encrypted. If a check fails you are not locked out — you get read-only access with no download, and a message telling you what to fix. Access is restored once the check passes. The check records the device, the time and the result; it does not inspect your files.

**Add to section 7** *(closes revocation SLA,* [`:846-882`](BYOD_REMOTE_WORK_ISAE3000_CONTROLS.md)*)*

> **What happens when you report.** We act on these timescales:
>
> | | |
> |---|---|
> | Credentials and keys suspended | within **5 minutes** of your report |
> | Initial assessment, and contact with you | within **1 hour** |
> | Full investigation and decision on restoring access | within **24 hours** |
>
> You may be without access for a period while this runs. That is the intended behaviour, not an overreaction.

**Add to section 4** *(closes monitoring,* [`:173-180`](BYOD_AUDIT_GAP_REMEDIATION_UPDATED.md)*)*

> Access to D&M systems is monitored for unusual patterns — access from an unexpected location, impossible travel, unusually large downloads, access at unusual hours. You may be contacted to confirm that an access was genuinely yours. If so, answer promptly; a quick "yes, that was me" closes an alert that would otherwise be treated as a possible compromise.

---

## Item 13 — 🟡 Mixed platform references

**Severity: medium — staleness, and an auditor will ask which it is**

### Current text (verbatim, three places)

> All appointments/meetings in **Outlook** (private appointments can be marked private)

> Use the '**Junk**' button in **G-Suite** to clean up spam

> …available on D&M **G-drive**.

### Problem

Calendars are in Outlook, spam is handled in G-Suite, policies live on G-drive. At most one of these is right. "G-Suite" has been Google Workspace since 2020, so that reference is at least five years stale. The Handbook is cited as evidence for access control and awareness; an auditor who cannot tell which platform you run cannot tell what the controls apply to.

### Proposed fix

Settle on the actual stack and apply it consistently. Assuming Google Workspace:

> All appointments and meetings in **Google Calendar** (private appointments can be marked private)

> Use the **"Report spam"** button in Gmail to clean up spam

> …available on the **D&M shared drive** (Google Drive).

If calendars really are in Outlook while mail is in Gmail, say so explicitly rather than leaving the reader to infer it.

---

## Item 14 — 🟡 Duplicated mobile-device paragraph

**Severity: medium — editorial, visible**

### Current text (verbatim, consecutive paragraphs under *Technical Controls*)

> D&M mobile devices (mobile phones and tablets) are protected with a **6-digit PIN** and use of encryption.
> Your participation in adhering to these enhanced security measures is key to protecting D&M and our customers' data.
>
> D&M **other** mobile devices (mobile phones and tablets) are protected with a **6 digit PIN** and use of encryption.

### Problem

The same requirement twice, the second time after the section's closing sentence, with "other" inserted and the hyphen dropped. It reads as a leftover from the password-section rewrite.

### Proposed fix

Delete the second paragraph. The device requirements now live in the table at Item 12 section 3; keep the *Technical Controls* list for D&M-owned infrastructure and cross-reference the new section for personal devices.

---

## Item 15 — 🟡 Training section states no frequency

**Severity: medium — Control C.3 evidence is untestable without one**

### Current text (verbatim)

> Awareness training ensures that new employees and all users have the necessary IT knowledge, including those who do not have an IT education, as well as good security behavior in terms of access to information. This also applies when an employee changes roles in the company. It is the responsibility of the individual manager that this happens.

### Problem

No frequency, no completion requirement, no record-keeping. The password section separately promises *"Ongoing employee security awareness training"* on phishing and social engineering — but "ongoing" is not a schedule. [`PROJECT_STATUS.md:246-250`](PROJECT_STATUS.md) expects "Training records / Training materials / Competence verification / Employee acknowledgments" as evidence; records can only be tested against a stated expectation.

### Proposed replacement

> ### Security awareness training
>
> Security awareness training ensures that everyone — including colleagues without a technical background — has the knowledge to handle information safely.
>
> | When | What |
> |---|---|
> | **Within your first 2 weeks** | Induction security training, before you are granted access to client data |
> | **Annually** | Refresher training, covering changes to our controls and current threats |
> | **On a change of role** | Additional training where your new role carries different access |
> | **Periodically** | Simulated phishing exercises. If you click one, you get a short follow-up module — not a reprimand. |
>
> Training completion is recorded. Your line manager is responsible for ensuring you complete it; the Compliance Manager maintains the records and reports completion rates to management.

### Why

Turns an aspiration into something the auditor can sample. The phishing-simulation line matters because the password section already promises training on phishing — this is what delivers it, and the no-reprimand framing is consistent with Item 4's no-penalty clause.

---

## Item 16 — 🟡 SAR routing conflates employee and client data subjects

**Severity: medium — processor-model obligation, Art 28(3)(e)**

### Current text (verbatim)

> If you receive a **subject access request**, you should refer this immediately to your line manager.

### Problem

Two very different requests are collapsed into one route. A request from an employee about their own employment data is for D&M to answer as controller. A request from a **client's** data subject is one D&M must not answer at all — it has to be passed to the client, who is the controller. [`PROJECT_STATUS.md:37`](PROJECT_STATUS.md) relies on exactly this distinction to close the Art 12-13 gap: *"Processor model - DSRs via clients"*.

Routing both to a line manager risks the worst outcome: a well-meaning employee answering a data subject directly on behalf of a client, which is a breach of the DPA and potentially of Art 28(3)(e).

### Proposed replacement

> ### Requests from individuals about their personal data
>
> Which route applies depends on **whose** data is involved.
>
> **A request about D&M employee data** — your own, or a colleague's — goes to the Compliance Manager. D&M is the controller and answers it. See *Your rights as a data subject*.
>
> **A request from anyone about data we process for a client** — including that client's customers, employees, or anyone whose data is in a client system — **must not be answered by you.** D&M is a processor, not the controller: only the client may decide how to respond. Forward it to the Compliance Manager immediately and do not reply to the requester, not even to confirm whether we hold data about them. The Compliance Manager notifies the client within the timescales in the relevant Data Processing Agreement.
>
> If you are unsure which applies, treat it as the second and ask.

### Why

The "do not reply, not even to confirm" instruction is the operative part — confirming or denying that a client's system holds a given person's data is itself a disclosure the client has not authorised.

---

## Item 17 — 🟡 Access-rights table

**Severity: medium — this table will be tested against actual access**

### Current text (verbatim, extract)

> | Position \ Access | Demo | Development | Hosted | Cust. On-Prem | Masterdata | Stage / Test | VPN On-prem |
> | **Sale** | x | | | | | | |
> | **UX/IU designer** | x | x | x | | | x | |
> | Language team | **X** | **X** | | | **X** | | |

### Problem

Editorial: "Sale" should be "Sales"; "UX/IU designer" should be "UX/UI designer"; the Language team row uses capital `X` where every other row uses lowercase `x`; the meaning of `(x)` in the Data scientist row is never explained.

Substantive: this is a control description that an auditor will test by pulling actual access lists. Two things to verify before the audit — that the roles listed still match the roles you employ, given the Handbook now needs to account for 25 developers; and that nobody's real access exceeds their row. A table that is *stricter* than reality is worse than no table, because it documents a control you are not operating.

### Proposed fix

Correct the typos, normalise the marks, add a legend:

> `x` = access granted · `(x)` = access granted on approval for a specific task, time-limited · blank = no access

Then reconcile the table against actual access as part of the quarterly review the Handbook already commits to (*"Your role and access rights will be evaluated every quarter by the Compliance team and your manager"*) — and keep the output of that reconciliation, because it is the evidence for Control B.6. Consider adding a column recording whether the role's access is permitted from a personal device, which would connect this table to Item 12.

---

## Item 18 — 🟢 Vestigial COVID-era and on-premises text

**Severity: low — but it reads as a document nobody has maintained**

### Current text (verbatim, extracts)

> **Behaviour during an pandemic** … If a physical meeting is necessary, all participants should have a recent negative test. … if traveling to a "red" country the employee when returning to their home again must follow the guidelines from authorities

> **Personal Safety** … arrange to meet the person in Company premises. Always ring back the telephone number you have been given to confirm that it is legitimate. If a mobile number is given you should always ask for an alternative fixed line number.

> You must not remove Company property from the organization's premises unless prior authority from your line manager has been given.

### Problem

The pandemic section is written to 2021 conditions — "red" countries and negative tests were specific public-health regimes, not standing practice. The Personal Safety advice assumes an office you can bring visitors to, in a company whose own Handbook says *"All employees work from home"*, and the fixed-line request is dated. The premises clause sits oddly when the equipment is already off-premises by default.

### Proposed fix

Keep the pandemic section but generalise it: replace the test and "red country" specifics with *"follow the guidance issued by the Danish authorities, or those of your country of residence, at the time"* — the decision-making structure (partners decide per area, inform their teams, employees report illness to their team lead) is sound and worth keeping. Rewrite Personal Safety around meeting strangers at neutral or client locations, and verifying identity before attending, rather than around bringing people to an office. Reframe the premises clause as a general custody-of-equipment obligation, which is what it is now trying to say.

---

## Item 19 — 🟢 Typos and language

**Severity: low**

| Location | Current | Proposed |
|---|---|---|
| Value statement | "We are here for our **college** and help them be their best." | "…for our **colleagues**…" |
| Conflict of Interest | "prevent the employee **form** devoting proper attention" | "**from** devoting" |
| Health and Safety | "Behaviour during **an** pandemic" | "**a** pandemic" |
| Calendar and mails | "**Alle** employees in Data and More" | "**All** employees" |
| Criminal Records Checks | "Due to the nature that we are working with vulnerable data." | Sentence fragment — see Item 8 |
| Processing in accordance with instructions | "You shall always process data in accordance which is applied by a Data Processing Agreement" | "…in accordance with the instructions given in the Data Processing Agreement with our client" |
| Health and Safety | "other persons who may affected by its' activities" | "who may **be** affected by **its** activities" |
| Technical Controls | "vpn certificates" | "VPN certificates" |

> **Correction (13 October 2026).** An earlier version of this redline stated that the `Index` heading had no index beneath it. **That was wrong** — the document contains a proper 72-entry table of contents with page numbers. The error came from my text extraction, which skipped `tableOfContents` structural elements. No action is needed on the index.
>
> One consequence worth noting: because the TOC reproduces heading text, **any change to a heading also needs the TOC refreshed** (right-click → Update table of contents). The `Behaviour during a pandemic` fix below touched both the heading and its TOC entry.

---

## Item 20 — 🔴 Three cross-references to a disciplinary procedure that does not exist

**Severity: high — the Handbook threatens a procedure the company has never written, and the DPA promises one to clients**

**Added:** 26 October 2026, alongside [`EMPLOYEE_SANCTIONS_AND_DISCIPLINARY_PROCEDURE.md`](EMPLOYEE_SANCTIONS_AND_DISCIPLINARY_PROCEDURE.md).

### Current text (verbatim, three separate places)

*Hours of Work*, page 9:

> "Persistent poor timekeeping means that colleagues are put under pressure to cover your duties. This is not acceptable and will therefore be treated as a potential disciplinary offence **under our disciplinary procedures**."

*Smoking and Other Substances at Work*, page 11:

> "Any such instances will be dealt with **under the disciplinary procedure** and may lead to your summary dismissal."

*Bribery and other Corrupt Behavior*, page 27:

> "In these circumstances you will be subject to formal investigation **under the Company's disciplinary procedures**, and disciplinary action up to and including dismissal may be applied."

### Problem

All three cite a document that does not exist. There is no disciplinary procedure in the Handbook's
contents, none in the policy set on the G-drive, and none in the audit evidence folder. The Handbook
is the only place that states consequences at all, and it does so in nine separate sections without
ever saying who decides, what the steps are, or what is recorded.

This is the same class of defect as Item 2 (contact details that do not exist) and Item 11 (the
dangling erasure-policy reference), and it is worse than either, because here the dangling reference
is attached to a threat of dismissal. An employee told they face "formal investigation under the
Company's disciplinary procedures" cannot read those procedures, and a dismissal relying on a
procedure the employer never wrote is a weak position in a Danish employment case.

For the audit it is a two-sided problem:

- The Danish DPA commits, under *Organisatoriske sikkerhedsforanstaltninger* item 1, to policies
  defining **"ansvar og sanktioner i tilfælde af overtrædelser"**. Three cross-references to an absent
  document do not satisfy that, and **C.2** is where it surfaces.
- ISO 27001:2022 **A.6.4 Disciplinary process** was recorded in our own mapping as *LOW / NOT
  COVERED* until this week.

### Proposed fix

**(a) Name the document in all three places.** ✅ **Applied 26 October 2026 as pending suggestions.**
Three `replaceAllText` operations in one `batchUpdate` with `writeControl.writeMode: "SUGGEST"`, each
returning `occurrencesChanged: 1` — so nothing was over-matched. Index-free by design: the stale-offset
failure recorded further down this document came from `deleteContentRange` calls computed against a
read that went stale, and `replaceAllText` cannot reproduce it.

Inserted as plain text. The document title is **not** italicised, because italicising it would need an
`updateTextStyle` call with explicit indices, which is the one technique this item avoids.

Note that the third phrasing uses a curly apostrophe (`Company’s`, U+2019) and the first two differ from
each other, so the three cannot be done with a single replacement.

| Page | Search text (matchCase) | Replaced with | Occurrences |
|---|---|---|---|
| 9 | `under our disciplinary procedures` | `under the Employee sanctions and disciplinary procedure` | 1 |
| 11 | `under the disciplinary procedure` | `under the Employee sanctions and disciplinary procedure` | 1 |
| 27 | `under the Company’s disciplinary procedures` | `under the Employee sanctions and disciplinary procedure` | 1 |

Resulting sentences, for review in the document:

> "…will therefore be treated as a potential disciplinary offence **under the Employee sanctions and disciplinary procedure**."

> "Any such instances will be dealt with **under the Employee sanctions and disciplinary procedure** and may lead to your summary dismissal."

> "In these circumstances you will be subject to formal investigation **under the Employee sanctions and disciplinary procedure**, and disciplinary action up to and including dismissal may be applied."

**(b) Add a short section** at the end of *Standards of Performance and Behavior at Work*, so the
Handbook states the ladder once rather than implying nine different ones:

> ### If you do not follow these rules
>
> The rules in this Handbook are conditions of your employment, and some of them are commitments
> D&M has made to its clients in writing. Where they are not followed, D&M applies the *Employee
> sanctions and disciplinary procedure*, which is available on the G-drive alongside this Handbook.
>
> That procedure sets out six steps, from an informal conversation through a reminder, a written
> warning and a final written warning, to dismissal with notice and — for gross misconduct — summary
> dismissal. Which step applies depends on how serious the breach was, what harm it caused or
> risked, whether it was deliberate, whether it has happened before, and whether you reported it
> yourself. Serious conduct starts at the step it deserves rather than working up from the bottom.
>
> No step above an informal conversation is decided before you have been told what is alleged, shown
> what it is based on, and given a real opportunity to respond. You may bring a colleague or a trade
> union representative. You may object in writing to any decision, and the objection is reviewed by
> someone who did not take it.
>
> **You will not be penalised for reporting an incident in good faith, including one you caused
> yourself.** Failing to report, or delaying a report, is a disciplinary matter. Where access to a
> system or a device is suspended while something is looked into, that is a precaution and not a
> sanction, and it says nothing about fault.

**(c) Add the document to the contents list**, and to the *Policies and documents* section on page 25,
which currently names the IT security policy and classification but not this one.

**(d) Add a sixth point to the acknowledgement form** (Appendix 1):

> 6. I understand that the rules in this Handbook are conditions of my employment, that D&M applies
>    the *Employee sanctions and disciplinary procedure* where they are not followed, and that I know
>    where to find it.

### Why

Item 9 already rewrites the acknowledgement form and Item 10 already adds a review statement, so
this rides on work that is going out anyway. Doing (a) alone would be a 10-minute fix that removes
the dangling reference; doing (a) through (d) is what makes the Handbook internally consistent with
the procedure and with the DPA.

### Dependencies and sequencing

- **Blocked on approval of the sanctions procedure.** Naming a document in the Handbook before the
  Partner has approved it would reproduce the same defect in the opposite direction.
- **Conflicts with Item 9** if applied separately: Item 9's replacement acknowledgement form is still a
  pending suggestion with five points. Add point 6 to Item 9's text before it is accepted, rather than
  editing the form twice.
- **The employment-law review** recorded as the first open point in the sanctions procedure should
  land before (b) goes into a document every employee signs. The hearing rights and warning
  expiry periods in that paragraph are drafting, not legal advice.

---

## Suggested sequence

**Before the auditor sees the document** — Items 1, 2, 10, 14, 19. Mechanical, no decisions needed, removes the "unmaintained document" impression.

**Needs a decision from you** — Items 3 (check the contract), 6 (the EU question, and it may reopen a closed gap), 12 (which laptops are company-owned).

**Needs DK legal review** — Items 7, 8.

**The substantive work** — Items 4, 5, 9, 12 Variant A, 15, 16. This is the set that closes the real gap between the Handbook and the control documentation, and it should go out as one version with fresh acknowledgements from all staff (Item 9).

**After remediation lands** — Item 12 Variant B, in increments, as each control becomes testable.

**Verify rather than draft** — Item 11 (does the erasure policy exist under that name?), Item 17 (does the access table match reality?), Item 13 (which platform?).

**Blocked on the sanctions procedure** — Item 20. Part (a), naming the document in the three places
that already cite it, goes in as soon as the Partner approves the procedure. Parts (b) and (d) should
wait for the Danish employment-law review, and part (d) must be folded into Item 9 rather than
applied on top of it.
