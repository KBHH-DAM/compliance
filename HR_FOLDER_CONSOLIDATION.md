# HR Folder — Consolidation Plan

**Prepared:** 2026-10-27
**Scope:** Google Drive HR folder [`1_9T5utUueJ2...`](https://drive.google.com/drive/folders/1_9T5utUueJ2Lj3AF4V-tv8AbQh4x6sX1)
**Companion to:** [[POLICY_CONSOLIDATION_RECOMMENDATION]] (ISMS folder)

**41 files today → 12 live documents** (revised from 10 — see §8b and §8c). Breakdown: 16 files in the root, 5 in `Arbejdsmiljø/`,
20 in `X Old/`.

---

## 1. Read this first: HR does not merge like the ISMS folder

In the ISMS folder, nearly everything is a policy and policies merge freely. HR holds four
different *kinds* of artefact, and only the first kind merges:

| Kind | Merges? | Why |
|---|---|---|
| **Policies & procedures** | Yes | Nothing requires them to be separate files |
| **Signable templates** | **No** | Each employee signs their own copy. Fold an NDA into a handbook and you lose the signature, and with it the ISAE 3000 evidence an auditor samples per employee |
| **Registers** | **No** | Live evidence, not documents to be written |
| **Personnel records** | **No** | They belong in an individual's file, not a policy folder |

So the target is not "one HR document". It is **three policy/procedure documents**, two signable
templates, two registers/statements, and the separate `Arbejdsmiljø` pair.

---

## 2. Three things the titles get wrong

Found by opening the files, not reading the names. Each would be mis-merged by anyone working
from the folder listing:

**`NDA - Data & More.pdf` is not an HR document.** It is a signed mutual NDA with **KYOCERA
UNIMERCO TOOLING A/S**, effective 03 December 2024, covering a data-deletion-tool proof of
concept. It is a commercial contract filed in the wrong folder. Do **not** merge it with the
Employee Confidentiality Agreement — they are unrelated. Move it to the commercial contracts
folder.

**`Employee retirement procedure` is not a procedure.** It is a completed offboarding checklist
for one named individual, dated 6/12/2024, with two ticked tasks. It is a personnel record. Move
it to that employee's file. The actual procedure is `C5 C6 Offboarding and departure procedure`.

**`Where sanctions are defined` is a working note.** It maps where sanctions actually appear —
seven scattered sections of Staff Handbook v5 (pages 9, 11, 14, 15, 27, 29, 34) plus three
Cyberday policy exports. Valuable content, wrong form: it belongs as the cross-reference appendix
to `EMPLOYEE_SANCTIONS_AND_DISCIPLINARY_PROCEDURE`, not as a standalone document.

---

## 3. Target set — 10 live documents

### Policies & procedures (3)

| # | Document | ISO 27001 A.6 | Absorbs |
|---|---|---|---|
| 1 | **DAM Staff Handbook v5** — employee-facing | A.6.2, A.6.3, A.6.7 | **Nothing — revised, see §8c.** All three proposed absorptions were withdrawn after reading them |
| 2 | **C4 Onboarding and induction procedure** — HR-facing | A.6.1, A.6.3 | Already absorbs the DMCS Developer Onboarding Guide, the screening procedure (C.3) and the Hiring Policy Checklist — see §8b |
| 2b | **C5 C6 Offboarding and departure procedure** — HR-facing | A.5.11, A.6.5 | Keep separate — **recommendation revised, see §8b** |
| 3 | **Employee Sanctions & Disciplinary Procedure** | A.6.4 | `Where sanctions are defined` (as its appendix) |

**Why 1 and 2 stay apart.** Different audiences and different authors. The handbook tells an
employee what is expected of them; the lifecycle procedure tells HR and IT what steps to execute
and who owns each. Merging them produces a document employees will not read and HR cannot work
from. Keep the split; add an Annex A mapping table to each.

**Onboarding and offboarding: do not merge.** This reverses the first version of this plan. See
§8b — both documents turned out to be mature, approved and already consolidated, and merging them
would cost re-approval for no compliance gain.

### Signable templates (2) — do not merge

| # | Document | Note |
|---|---|---|
| 4 | **Employee Confidentiality Agreement v2** | Properly version-controlled already (v2, approved by Lars Taxgaard, next review 18 Oct 2027). Use it as the model for the others |
| 5 | **Consent to use my data for test purpose v2** | GDPR consent, signed per person |

### Registers & statements (2) — do not merge

| # | Document |
|---|---|
| 6 | **C3-C4 Register of appointments** |
| 7 | **HR Management Statement 2026** — dated annual management evidence |

### `Arbejdsmiljø/` (2 documents, currently 5 files)

| # | Document | Delete |
|---|---|---|
| 8 | **DM_Health_and_Safety_Policy_ISO45001_v1.0** | the `.docx` and `.pdf` copies |
| 9 | **DM_DSE_Self_Assessment_Checklist_v1.0** | the `.docx` copy |

Out of ISO 27001 scope — this is ISO 45001 and Danish arbejdsmiljø/APV law. Keep the folder, just
drop the redundant format copies. Three files deleted, nothing lost.

### Keep the Whistleblower Policy standalone (1)

| # | Document |
|---|---|
| 10 | **Whistleblower Policy for Data & More** |

Do not fold this into the handbook. The Danish Whistleblower Act (lov om beskyttelse af
whistleblowere) obliges employers above the threshold to operate a scheme with accessible,
separately communicated reporting channels. A standalone policy is easier to publish and to
evidence than a handbook section.

---

## 4. Misfiled — move out of HR

| Artefact | Destination |
|---|---|
| `NDA - Data & More.pdf` (Kyocera commercial NDA) | Commercial contracts |
| `Consultant contract Data & More Aps.docx`, `Consultant contract_ Data & More SOW no1.docx` | Commercial contracts |
| `Employee retirement procedure` (one person's completed checklist) | That employee's personnel file |
| `Policies and procedures … conserve natural resources and protect the environment` | Corporate/ESG — **and note it is already duplicated as a PDF in the ISMS folder's `Old/`** |
| `HR-list and roles` (Sheet ×2 + `.xlsx`), `Employees D&M.xlsx` | One HR register, or Cyberday personnel data |
| `HR_People_Security_Manager_RACI_Matrix` | The single RACI annex in [[POLICY_CONSOLIDATION_RECOMMENDATION]] §3 — this is the **fourth** RACI matrix found across the two folders |
| `DMCS_Developer_Onboarding_Guide` (Sheet + `.xlsx`) | Engineering documentation |
| `Data & More ApS Mail - Bekræftelse af læst dokumentation.docx` | Acknowledgement record → appointments register / personnel files |
| `Employee instruction on processing of personal data and use of IT.pdf` (2023) | Superseded by the handbook + confidentiality agreement → archive |
| `DAM__Staff_Handbook v3.0 2023.docx` | Archive |

## 5. `X Old/` — archive the whole folder

20 files, including two superseded confidentiality agreements, three formats of the hiring policy,
three copies of the HR list, and the 2023 handbook. Same reasoning as the ISMS folder: a live
subfolder named `X Old` containing documents titled "policy" and "agreement" invites an auditor to
ask which version is in force.

Move the tree to a dated read-only archive (`HR-archive-2026/`) outside the HR folder. Do not
delete — employment records carry statutory retention, and ISAE 3000 benefits from retained
history.

## 6. Format duplicates to collapse

| Document | Copies now | Keep |
|---|---|---|
| Health & Safety Policy ISO 45001 | Doc + `.docx` + `.pdf` | Doc |
| DSE Self-Assessment Checklist | Doc + `.docx` | Doc |
| Hiring Policy Isae | `.docx` + `.odt` + `.md` | none — content goes into document 2 |
| HR-list and roles | Sheet ×2 + `.xlsx` | one register |
| DMCS Developer Onboarding Guide | Sheet + `.xlsx` | Sheet, moved out of HR |
| Confidentiality Agreement Employee | Doc + `.docx` | neither — both retired by v2 (below) |
| Consent to use my data for test purpose | Doc v2 + Doc + `.docx` | the root `_v2` Doc |

---

## 7. A live compliance gap, not just filing

`Employee Confidentiality Agreement_v2` states in its own document-control section that it
supersedes two earlier versions, and that:

> Agreements already signed on an earlier version remain in force for commercial confidentiality.
> They do not carry the Article III personal data undertaking, so anyone still employed should
> sign this version as well.

Article III exists to satisfy **GDPR Art. 28(3)(b)**, under which a processor must ensure the
people it authorises to process personal data have committed themselves to confidentiality. Staff
still holding only a pre-v2 signature are therefore not covered by that undertaking.

**This is an action, not a merge:** identify who signed before 18 October 2026 and collect v2
signatures, then record them in the appointments register. An ISAE 3000 auditor sampling
confidentiality undertakings per employee would find this.

The v2 document also notes the two retired versions disagreed with each other about which group
companies existed (one named Data & More LLC, ApS and GmbH; the other only LLC and ApS). Worth
confirming the current group structure is stated correctly in v2 before it goes out for signature.

---

## 8. Sequencing

1. **Archive `X Old/`** — 20 files out of scope in one move, no drafting. **(Started 27 Oct 2026 — see §8a.)**
2. **Delete the three redundant format copies in `Arbejdsmiljø/`.** Two minutes, nothing lost.
3. **Move the misfiled items in §4** — the Kyocera NDA especially, since it is a customer contract sitting in an HR folder.
4. **Collect v2 confidentiality signatures (§7).** The only item here that is a real compliance gap rather than tidying — do it in parallel with everything else.
5. **Merge `C4` + `C5 C6` + hiring policy** into document 2.
6. **Fold the three absorbed policies into Staff Handbook v5**, and `Where sanctions are defined` into the sanctions procedure as its appendix.
7. **Add document control to all ten** — owner, version, approval date, review interval — copying the pattern `Employee Confidentiality Agreement_v2` already uses.

Steps 1–3 remove roughly 30 files without writing anything.

---

## 8a. Step 8.1 — status, 27 October 2026

**Done:**

- Archive folder **`HR-archive-2026`** created as a sibling of `HR`, inside
  `3. ISMS compliance documents`:
  [drive.google.com/drive/folders/1hVIlgAx1p3osadVz2Hd_Jr3qnwunFZk3](https://drive.google.com/drive/folders/1hVIlgAx1p3osadVz2Hd_Jr3qnwunFZk3)
- Status note **`READ ME — archive status (not in force)`** written inside it, stating that nothing
  in the archive is a current policy, why superseded versions are retained rather than deleted
  (Danish statutory retention; ISAE 3000 and GDPR Art. 5(2) accountability), the known
  supersessions per document, and which items in `X Old` are **misfiled rather than superseded**
  and so need rehoming instead of archiving.

**Remaining — one manual step:**

Move `HR/X Old` into `HR-archive-2026`. The Google Drive connector could not perform this: it
creates new items and edits what it created, but Google refuses `parentId` changes on
pre-existing files and folders it did not create. This is a connector scope limit, not an access
problem — the account holds `organizer` on the folder, which is the highest shared-drive role.

In the Drive UI this is a drag of `X Old` into `HR-archive-2026`, or right-click → Organise →
Move.

**Deliberately not attempted:** copying the 20 files into the archive and trashing the originals.
That would reset creation dates and discard revision history — the very history the archive exists
to preserve — and would mean deleting employment records to accomplish a filing move.

**After the move:** consider locking the archive with Drive's read-only lock, and rehome the
misfiled items listed in the status note (§4) rather than leaving them archived.

**Confirmed 27 Oct 2026:** `X Old` is now inside `HR-archive-2026`, alongside the status note.

---

## 8b. Step 8.5 reversed — read C4 and C5/C6, do not merge them

The first version of this plan recommended merging `C4 Onboarding and induction procedure`,
`C5 C6 Offboarding and departure procedure` and the hiring policy into one Employee Lifecycle
Procedure. That was based on titles, sizes and dates. **Having now read both documents in full,
that recommendation is withdrawn.** Keep them as two documents.

### Why

1. **C4 is already a four-into-one consolidation.** It states that it replaces the DMCS Developer
   Onboarding Guide, "whose ten technical standards are carried forward in full as the developer
   section"; it contains the screening procedure answering C.3; and the full Hiring Policy
   Checklist is appended to it verbatim. The merge this plan asked for has largely happened.
2. **Both are version 1, dated, with next-review dates set.** C5/C6 is approved by Lars Taxgaard,
   Partner, 18 Oct 2026, next review 18 Oct 2027. Merging resets an approval that already exists.
3. **They already hand off to each other explicitly and correctly.** C4: "When someone leaves, the
   offboarding procedure takes over." C5/C6 maps row C.4 back to C4. Neither duplicates the other.
4. **Different owners on different clocks.** C5/C6 splits ownership across Service Owner, hiring
   manager, Privacy Lead and Partner, with a five-case table setting when access is withdrawn
   (worked notice vs. garden leave vs. dismissal for cause vs. contract end vs. internal move).
   That detail does not survive being folded into an onboarding document.
5. **Auditors request them separately.** C.3/C.4 and C.5/C.6 are distinct rows on the ISAE 3000
   request list, and each document carries its own mapping table.

**Target count moves from 10 to 11.** Consolidating mature, approved, cross-referenced documents
is churn, not simplification.

### Defects found — and step 8.1 made two of them urgent

Archiving `X Old` was correct, but it turned two stale links in C4 into links pointing into a
folder now explicitly marked "not in force". These need fixing before the next hire:

| # | Defect | Fix |
|---|---|---|
| 1 | **C4 links to the superseded confidentiality agreement, twice** — in the pre-start checklist and in Day one step 1. The target is `Confidentiality Agreement Employee` (doc `1zOAtrla…`), now archived, which **lacks the Article III personal-data undertaking** | Repoint both to `Employee Confidentiality Agreement_v2` (doc `1_h00Hjuml…`) |
| 2 | **C4 links to the superseded test-data consent form** — `Consent to use my data for test purposes` (doc `17HKZpKpZu…`), now archived | Repoint to `Consent to use my data for test purpose_v2` (doc `1VoXL5QPxiko…`) |
| 3 | **C4's approval block is empty** — it ends "Approved by — name, role, date:" with nothing after it, while the appended hiring-policy section claims approval by Lars Taxgaard. An unapproved procedure in force is a finding in its own right | Approve and date it, or state which approval the appended block carries |
| 4 | **Two sources of truth for the hiring checklist** — C4 calls a separate Hiring Policy (doc `1qM2kGBDwHeW…`) "the reference copy" while also containing the checklist in full. That doc is in neither the HR folder nor the ISMS folder as listed | Pick one. If C4 is authoritative, archive the separate copy; if not, cut the appended section |
| 5 | **Retention period unset in both** — C4 has a literal `[retention period]` placeholder; C5/C6 lists it as an open point and says it must match C4 | One decision closes both |

Defect 1 is the serious one. Followed literally, C4 has every new joiner sign a retired agreement
that does not carry the GDPR Art. 28(3)(b) undertaking — the same gap as §7, reaching forward to
future hires rather than only back at existing staff.

### Open points the two documents already raise themselves

C5/C6 lists five; C4 adds one. Worth closing together since they overlap:

- Set the retention period for the induction and offboarding records (defect 5 above).
- **Name the Service Owner and the Privacy Lead**, so both procedures name people rather than roles.
- **Populate the register of appointments.** C5/C6 is blunt that without it neither the leaver list
  nor the nil-return confirmation asserts anything.
- Confirm whether anyone has in fact left in the period; if so, C5/C6 applies retrospectively.
- Decide whether contractors and students get the same departure notice or a shortened one.
- Decide who gives the induction when the hiring manager is the person being inducted.

**None of these are merges.** The HR documents are in better shape than the file count suggested —
the remaining work is approval, named owners, a populated register and five corrected
cross-references, not consolidation.

### Not done here

C4 and C5/C6 could not be edited: the Drive connector cannot modify files it did not create, the
same limit that blocked the move in §8a. Defects 1–5 need the Drive UI.

---

## 8c. Step 8.6 reversed — the handbook absorbs nothing

This plan said to fold `Ethical Conduct and Human Rights Commitments`, `Obligation Act Compliance
Policy` and `Management Pandemic policy.docx` into Staff Handbook v5. **All three are withdrawn.**
Each was wrong for a different reason, and none was visible from the file listing.

### 1. `Ethical Conduct and Human Rights Commitments` — not a policy

It is a **cross-reference map**, not a policy. Every row of all three of its tables points
somewhere else: "Excerpts from DAM__Staff_Handbook v5.pdf (Section: Dignity at Work)", "Excerpts
from ISAE 3000 B2 F6 … Risk management policy.pdf". It states no obligation of its own.

There is nothing to fold in — the content is **already** in the handbook, and this document is an
index of it. **Retire it**, or keep it explicitly as an audit cross-reference appendix in the same
way as `Where sanctions are defined`.

This is the second such document found (the first being the sanctions note). The pattern is worth
naming: someone has been producing "where is X defined" mapping documents and filing them beside
real policies, which is exactly what makes the folder look as though it holds more policy than it
does.

Two things in it are worth keeping before it goes — its §3 records where documents actually live:
the Cyberday ISMS report URL, and `G:\Fællesdrev\Clients\Denmark\` for the client DPA list. It
also cites three ISAE evidence PDFs held in neither folder reviewed here, so **there is a further
evidence folder not yet inventoried**.

### 2. `Obligation Act Compliance Policy` — a real standalone policy, keep it

Do **not** fold this into the handbook:

- It implements the **German Verpflichtungsgesetz**, under which covered individuals are treated as
  public officials for certain offences under §§ 331–337 of the German Criminal Code. That is a
  distinct legal regime, not general staff conduct.
- It **contains a signable declaration** (the *Verpflichtungserklärung*). By §1 of this plan,
  signable templates do not merge.
- It applies to a **subset** of people — those performing public service duties. Folding it into
  the handbook would imply it binds everyone, which overstates it.
- It names a **Compliance Officer** and an **Ethics and Compliance Committee**.

**Two questions before it is relied on:**

- Does the "dedicated Ethics and Compliance Committee" it claims actually exist, and is there a
  register of signed Verpflichtungserklärungen? A policy asserting controls that do not exist is
  worse than no policy, and it also claims alignment with ISO 37001.
- It has **no document control at all** — no version, no approval date, no named owner, no next
  review date — and was last modified December 2024, despite saying it "will be reviewed annually".

### 3. `Management Pandemic policy.docx` — not an HR document

Its actual title inside the file is **"Business Continuity Policy for Pandemic Preparedness"**. It
covers essential-function identification, remote-work capability, supply-chain contingency and
drills. That is business continuity, not HR.

**Move it to the ISMS set**, as a pandemic / staff-unavailability scenario annex to **B4 Incident
Management & Business Continuity Policy** in [[POLICY_CONSOLIDATION_RECOMMENDATION]]. It is
otherwise generic boilerplate with no version or approval block and "approved by senior management"
with no name or date — but it carries one piece of real operational content to preserve: the DM
contact list, with CEO, CTO and Compliance Manager phone numbers and the support address.

### Revised target: 12 documents

| Revision | Count |
|---|---|
| Original plan | 10 |
| §8b — C4 and C5/C6 stay separate | 11 |
| §8c — Obligation Act stays standalone; pandemic policy leaves HR for the ISMS set | **12** |

### What this actually means

The count rose at every step because the first pass worked from titles, sizes and dates. Read
properly, **the duplication in the HR folder was format copies and archive clutter, not
overlapping policies.** Of 41 files, the genuine policy-level redundancy is two documents: the
ethics cross-reference index, and the pandemic policy that belongs in another set.

The real wins were the ones that needed no drafting: 20 files archived, 14 format duplicates across
7 documents, and a handful of misfiled contracts and records. The remaining work is **approval,
named owners, document control and corrected cross-references** — not merging. Three of the twelve
documents have no version or approval block at all, and C4's is empty.

---

## 9. Before / after

| | Now | After |
|---|---|---|
| Files in the HR tree | 41 | 10 live documents + dated archive |
| Policies/procedures to review | ~13 | 5 (+ whistleblower) |
| Misfiled commercial contracts | 3 | 0 |
| Format duplicates | 14 files across 7 documents | 0 |
| Confidentiality agreement versions in play | 3 | 1 |

---

*Caveat: documents 1–3 were assessed from titles, sizes and dates; `Where sanctions are defined`,
`Employee retirement procedure`, `Employee Confidentiality Agreement_v2` and the Kyocera NDA were
opened and read. Before folding anything into the handbook, confirm the absorbed text adds no
obligation the handbook contradicts — the sanctions note already shows handbook content is
scattered rather than absent.*
