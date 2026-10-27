# HR Folder — Consolidation Plan

**Prepared:** 2026-10-27
**Scope:** Google Drive HR folder [`1_9T5utUueJ2...`](https://drive.google.com/drive/folders/1_9T5utUueJ2Lj3AF4V-tv8AbQh4x6sX1)
**Companion to:** [[POLICY_CONSOLIDATION_RECOMMENDATION]] (ISMS folder)

**41 files today → 10 live documents.** Breakdown: 16 files in the root, 5 in `Arbejdsmiljø/`,
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
| 1 | **DAM Staff Handbook v5** — employee-facing | A.6.2, A.6.3, A.6.7 | `Ethical Conduct and Human Rights Commitments` · `Obligation Act Compliance Policy` · `Management Pandemic policy.docx` |
| 2 | **Employee Lifecycle Procedure** — HR-facing | A.6.1, A.6.3, A.6.5 | `C4 Onboarding and induction procedure` + `C5 C6 Offboarding and departure procedure` + `Hiring Policy Isae` (3 formats in `X Old`) |
| 3 | **Employee Sanctions & Disciplinary Procedure** | A.6.4 | `Where sanctions are defined` (as its appendix) |

**Why 1 and 2 stay apart.** Different audiences and different authors. The handbook tells an
employee what is expected of them; the lifecycle procedure tells HR and IT what steps to execute
and who owns each. Merging them produces a document employees will not read and HR cannot work
from. Keep the split; add an Annex A mapping table to each.

**Why onboarding and offboarding merge.** They are the two halves of one lifecycle with the same
owners and the same asset/access checklists in mirror image. Carry the `C4` / `C5` / `C6` control
references into section headings so the ISAE 3000 request list still resolves.

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

---

## 9. Before / after

| | Now | After |
|---|---|---|
| Files in the HR tree | 41 | 10 live documents + dated archive |
| Policies/procedures to review | ~13 | 3 (+ whistleblower) |
| Misfiled commercial contracts | 3 | 0 |
| Format duplicates | 14 files across 7 documents | 0 |
| Confidentiality agreement versions in play | 3 | 1 |

---

*Caveat: documents 1–3 were assessed from titles, sizes and dates; `Where sanctions are defined`,
`Employee retirement procedure`, `Employee Confidentiality Agreement_v2` and the Kyocera NDA were
opened and read. Before folding anything into the handbook, confirm the absorbed text adds no
obligation the handbook contradicts — the sanctions note already shows handbook content is
scattered rather than absent.*
