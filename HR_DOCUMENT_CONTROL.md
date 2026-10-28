# HR Document Control — Standard Block and Per-Document Status

**Prepared:** 2026-10-27
**Implements:** step 8.7 of [[HR_FOLDER_CONSOLIDATION]] ("add document control to all ten" — the
set is now twelve, per §8c)

Names are omitted deliberately: role titles only. The repository is public.

---

## 1. Headline: four documents cannot be given document control yet

Step 8.7 was written as a formatting task — add owner, version, approval date and review interval
to each document. Reading them shows it is not:

**Four of the twelve are not in force**, so there is no approval to record:

| Document | State |
|---|---|
| **Whistleblower Policy** | `Effective Date: [Insert Date]` · `Approved by: [Insert Executive or Compliance Lead Name]` — **never approved** |
| **HR Management Statement 2026** | Signatory name, title, date and signature **all blank** — unsigned |
| **Obligation Act Compliance Policy** | No version, no approval date, no owner, no review date; last modified December 2024 |
| **Employee Sanctions & Disciplinary Procedure** | Self-declared: *"Draft for management approval — version 0.1. Not in force until approved and issued."* |

You cannot write "approved by X on date Y" for a document nobody has approved. **These four need a
management decision first; document control follows.** The remaining eight are a formatting pass.

### The whistleblower policy is the urgent one

It is not only unapproved — its **reporting channel is a placeholder**:

- the portal link reads `[Insert link – e.g., https://whistleblower.dataandmore.com]`
- it routes to `whistleblower@dataandmore.com` and `compliance@dataandmore.com`
- it assigns investigation to a *"Whistleblowing Committee"*

The Danish Whistleblower Act (*lov om beskyttelse af whistleblowere*) requires employers above the
threshold to **operate** reporting channels, not to have drafted a policy describing them. Three
things need confirming, in this order:

1. Does the portal exist, and what is its real URL?
2. Do those two mailboxes exist, and who monitors them?
3. Does the Whistleblowing Committee exist, and who sits on it?

If the answer to any is no, the gap is a live legal exposure, not a documentation nit. Note this is
the **second** committee asserted by an unapproved policy — the Obligation Act policy claims a
*"dedicated Ethics and Compliance Committee"*. Worth confirming both exist, or amending both
policies to name roles that do.

### The management statement evidences nothing while unsigned

`HR Management Statement 2026` is a management confirmation addressed to the auditor: recruitment
complies with the hiring policy, background checks are carried out, records are maintained. Every
signature field is empty, and despite the title there is no date anywhere in it.

An ISAE 3000 auditor asking for management's confirmation and receiving an unsigned template has
received nothing. **Get it signed and dated.**

---

## 2. The standard block

Copy the pattern `Employee Confidentiality Agreement_v2` already uses — it is the only document in
the set with complete, correct control. Place it as the last line of every policy and procedure:

```
Version <n> | Date of implementation: <DD Month YYYY> | Approved by: <role>
Next review: <DD Month YYYY> | Owner: <role>
```

Four rules, each of which something in this set currently breaks:

1. **An absolute next-review date**, not "one year from implementation" — a relative date cannot be
   reported on, and a reviewer cannot tell whether it has lapsed.
2. **A named role for owner and approver.** A role is acceptable and more durable than a person's
   name; what is not acceptable is leaving it blank.
3. **Version on the document, not only in the filename.** `DM_..._v1.0` carries its version in the
   title; if the file is renamed or exported the version is lost.
4. **Superseded versions named.** The confidentiality agreement does this well — it states which
   earlier versions it replaces and that holders of the old one must re-sign. Carry that forward
   wherever a v2 exists.

### Registers are different

`C3-C4 Register of appointments` is a live record, not a document with versions. It needs:

```
Owner: <role> | Updated: on each appointment and departure | Last reviewed: <DD Month YYYY>
```

A version number on a register is meaningless and invites someone to "freeze" it.

---

## 3. Per-document status

| # | Document | Current control | Action |
|---|---|---|---|
| 1 | Employee Confidentiality Agreement v2 | **Complete** — version, date, approver, next review | None. Use as the model |
| 2 | C5 C6 Offboarding and departure procedure | Version 1, date, approver, next review, owner | None for control. 5 open points remain in the document |
| 3 | Consent to use my data for test purpose v2 | Version 2, date, approver — but **relative** review date | Set an absolute next-review date. Also fill the body placeholders (§4) |
| 4 | C4 Onboarding and induction procedure | **Approval block empty**; the appended hiring-policy section carries its own version | Approve and date the document itself, or state which approval the appended block covers |
| 5 | DAM Staff Handbook v5 | Not verified | Check; the redline carries unfilled `[date]` placeholders in three places |
| 6 | DM Health and Safety Policy ISO45001 v1.0 | Version in **filename only** | Move the version into the document, add approver, date, owner, review date |
| 7 | DM DSE Self-Assessment Checklist v1.0 | Version in **filename only** | As above |
| 8 | C3-C4 Register of appointments | Not verified | Apply the register form (§2) |
| 9 | **Whistleblower Policy** | `[Insert Date]` / `[Insert Name]` | **Confirm the channels exist, then approve.** See §1 |
| 10 | **HR Management Statement 2026** | Unsigned, undated | **Sign and date it** |
| 11 | **Obligation Act Compliance Policy** | None at all | **Approve it, and confirm the committee it asserts exists** |
| 12 | **Employee Sanctions & Disciplinary Procedure** | Draft v0.1, explicitly not in force | **Management approval**, then v1.0 |

Items 9–12 are decisions. Items 1–8 are a formatting pass of maybe an hour.

---

## 4. Unfilled placeholders found while checking

These sit inside documents otherwise treated as current:

| Document | Placeholder |
|---|---|
| Consent to use my data v2 | retention period for work-account documents; contact `[ name, role, email ]`; Datatilsynet address; the `[ 30 ]` day erasure window; the optional health-data row left blank |
| C4 Onboarding and induction | `[retention period]` for the induction record; who inducts the hiring manager |
| C5 C6 Offboarding | retention period (must match C4) |
| Staff Handbook redline | `[date]` in three places |

The consent form's are the ones that matter: it is a **signed GDPR consent** relied on as the
Article 49(1)(a) basis for access from Serbia. A consent whose retention period and withdrawal
contact are blank is weak evidence of informed consent. It also contains a typo in the withdrawal
clause — *"Erasing the tes no t copies"* — in the sentence allocating responsibility for erasure.

---

## 5. Order of work

1. **Confirm the whistleblower channels exist** (§1). Legal exposure, not documentation.
2. **Sign the management statement.** One signature; unblocks an ISAE 3000 request row.
3. **Approve the sanctions procedure and the Obligation Act policy**, then version both 1.0.
4. **Fix the consent form's placeholders** before it is signed again — it is already being relied on.
5. **Apply the block to items 1–8**, settling the retention period once for C4 and C5/C6 together.
6. **Set the review dates as absolute dates**, and put them in a calendar. Twelve documents with
   review dates nobody diarises is the state this consolidation set out to escape.

---

*Caveat: items 5, 7 and 8 were not opened — the Staff Handbook is large and the register is a
sheet. Verify their current control before applying the block. Items 1–4, 6 and 9–12 were read.
This document records what the control blocks should say; it does not change any Drive document,
which the connector cannot do.*
