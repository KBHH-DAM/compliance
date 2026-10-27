# `Load files` — Inventory and Map Against B1–B5

**Prepared:** 2026-10-27
**Folder:** `4. ISAE3000_ISO27001` → `Load files`
([19iimUpKkqoHRzmdOI5lBBH5_dwAjaBrC](https://drive.google.com/drive/folders/19iimUpKkqoHRzmdOI5lBBH5_dwAjaBrC))
**Companion to:** [[POLICY_CONSOLIDATION_RECOMMENDATION]] §9 · [[HR_FOLDER_CONSOLIDATION]]

**~60 items.** The ISAE 3000 submission pack, named by control reference (A1–A3, B1–B15, C1–C7,
D1–D3, E1–E2, F1–F6, G1, H1–H2, I1–I4).

---

## 1. Headline: four of the five policies already exist

§2 of [[POLICY_CONSOLIDATION_RECOMMENDATION]] said to write five topic-specific policies, B1–B5.
Having now inventoried this folder:

| Proposed | Verdict | Already exists as |
|---|---|---|
| **B1** Access Control & Identity | **ADOPT** | `B6 B13 Access management and password policy — Cyberday` |
| **B2** Asset, Endpoint & Physical | **GAP — write this one** | only `B15 Physical access safeguards` (physical half only) |
| **B3** Operations & Network | **ADOPT** (5 documents) | `B4 B5 Network and communications security`, `B3 B8 Encryption`, `B3 Malware protection`, `B7 B9 Log management and security system`, `B12 Change management` |
| **B4** Incident & Continuity | **ADOPT** | `I1 I4 Continuity management policy` + `I2 Procedure for Personal Data Breach` |
| **B5** Supplier & Data Protection | **ADOPT** | `E1 F1 Data processing partners and DPAs — Cyberday` + `D1 D3 Erasure policy` + `G1 Third-country transfer` + `H1 H2 Data subject rights` |

**So the drafting work is one policy, not five.** Everything in Tier A is also already here:

| Tier A target | Exists as |
|---|---|
| A2 Information Security Policy & Objectives | `C1 Information security policy and objectives` |
| A3 Risk Management | `B2 Risk management policy — Cyberday` + `B2 Risk management procedure and result preview — Cyberday` |
| A5 Secure Development & Vulnerability Mgmt | `B10 Secure development and technical vulnerability management policy` |

Plus coverage this plan had assigned elsewhere: `B3 Personnel security guidelines and acceptance
procedure — Cyberday`, `C7 Trainings and exercises — Cyberday`, `C3 Privacy policy for job
applications and recruitment`, `B1 B14 Organizational cyber security measures — Cyberday`.

### The one real gap

**No asset management, information classification, or acceptable-use policy exists anywhere** —
not in this pack, not in the ISMS folder as a policy. What exists is scattered and in the wrong
form:

- `ISAE 3402 pkt 9 HW Asset management 2025` — a **PowerPoint deck**, in the ISMS folder
- `Process: Prohibition of Using Portable Storage Devices` — ISMS folder
- `B15 Physical access safeguards` — here, physical only

That covers ISO 27001:2022 **A.5.9–5.14** (inventory, acceptable use, return of assets,
classification, labelling, transfer) and **A.8.1** (user endpoint devices). A deck is not a policy
and will not satisfy A.5.1's requirement for a topic-specific policy.

**This is the only document worth drafting.** Scope it as *Asset, Classification, Endpoint &
Physical Security Policy*, absorbing `B15` so physical security does not become a twelfth
standalone file.

---

## 2. Duplicates provable from file size alone

Byte-identical copies, from the metadata — no need to open them:

| Document | Copies | Size | Names in use |
|---|---|---|---|
| Hetzner security and data protection | **4** | 163,464 | `F4 F5 Hetzner security and Data protection with D&M` · `F4 Hetzner security … (1)` · `F4 Hetzner security …` **×2** |
| Continuity management policy | **2** | 5,483,758 | `I1 I4 Continuity management policy` · `I4 Continuity management policy` |
| Data processing partners and DPAs (Cyberday) | **2** | 479,826 | `E1 F1 …` · `A2 …` |
| Hetzner ISO certificate | **2** | 364,476 | `F4 Hetzner ISO-Certificate` · `F4 F6 Hetzner ISO-Certificate` |

Near-duplicates needing a look before either is retired:

- `F5 Sub-processor risk assessment — Hetzner Online GmbH` (222,406) vs `F6 Sub-processor risk
  assessment — Hetzner Online GmbH` (234,164) — same title, different content.
- `E2 clients_export` — two Sheets (8,347 / 8,173).
- `C5 C6 Offboarding and departure procedure` exists in **three** places: a PDF here, a Google Doc
  here, and the Google Doc in the HR folder. Only the HR one should be editable.

**10 files removable** from the four byte-identical sets alone.

### Why the duplication happened

The control prefix is being used as a *tag*, but Drive filenames are not tags. A document serving
two controls gets copied and re-prefixed instead of referenced once — hence `F4`/`F4 F5`/`F4 F6`
of one Hetzner page, and `E1 F1`/`A2` of one Cyberday export. Any document serving more than one
control will keep multiplying under this scheme.

---

## 3. A third mis-titled document

`B14 READ ME FIRST` is **not** an index to this pack, despite the name and despite being the only
document that looks like one.

It is an **end-user VPN setup guide** — Tunnelblick and OpenVPN install steps, SMS enrolment codes,
single sign-on, internal ssh access, and a warning never to run the old and new VPN at once.
Useful operational content, filed here with a `B14` prefix as evidence for the organizational
measures control.

So **there is no map of this folder.** That is the gap that let three folders each look complete:
nothing indexes the pack, and the one file named as though it does, does not.

Joining the two earlier cases, that is three documents whose titles actively mislead:
`Employee retirement procedure` (one person's completed checklist), `Where sanctions are defined`
(a working note), and now `B14 READ ME FIRST` (a VPN guide).

---

## 4. Policies and records are mixed together

The pack interleaves the policy set with named individuals' personnel records:

- Three `C3`-prefixed screening and reference records, each naming an individual employee in its
  filename, plus two `C3` hiring screenshots and `C7 Skill tests`
- `B13` screenshots ×5 · `D1` screenshot — access-control and erasure evidence
- `A1` signed client DPAs ×3 (two named clients and one DocuSign copy)
- `B12 ldap_users` · `E2 clients_export` ×2 — registers

Fine for a submission pack, wrong as a filing system. Three named employees' screening records sit
beside the information security policy as peers. Separate into `policies/`, `registers/` and
`evidence/` subfolders, with personnel records under restricted access — they are personal data
about employees, and the folder inherits domain-wide reader access.

---

## 5. Revised step 6

Replacing §9's instruction in [[POLICY_CONSOLIDATION_RECOMMENDATION]]:

1. **Adopt, do not write, B1 / B3 / B4 / B5.** Record in the SoA which document answers each
   Annex A control. No drafting.
2. **Draft one policy:** Asset, Classification, Endpoint & Physical Security (§1 above). The only
   genuine gap found across all four folders.
3. **Delete the 10 byte-identical duplicates** (§2), then compare the two sub-processor risk
   assessments and the two client exports before retiring either.
4. **Write the index this folder lacks** — one sheet, control reference → document → where the
   editable master lives. Not named "READ ME FIRST", which is taken.
5. **Split policies from records** (§4) and restrict the personnel records.
6. **Stop prefixing copies.** One master per document; the index carries the control mapping. This
   is what prevents the duplication recurring.

### Revised counts

| | Before | After |
|---|---|---|
| Policies to draft from scratch | 5 (B1–B5) | **1** |
| Files removable from `Load files` | — | 10 provable + 3 pending comparison |
| Documents indexing the pack | 0 | 1 |

---

*Caveat: this is a metadata inventory. Duplicate claims in §2 rest on byte-identical file sizes,
which is strong but not proof of identical content — confirm before deleting. The documents read
in full were `B14 READ ME FIRST` only; the policy documents here were identified by title and
control prefix, so confirm each adopted document actually covers its Annex A controls before
recording it in the SoA. The `A.5.9–5.14` gap in §1 is asserted from the absence of any
asset-or-classification-titled policy across all four folders reviewed — worth one search of the
wider Drive before writing a new one.*
