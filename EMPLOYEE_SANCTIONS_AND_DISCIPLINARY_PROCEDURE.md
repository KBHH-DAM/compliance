# Employee sanctions and disciplinary procedure

Data & More ApS, CVR 38185659 · 26 October 2026 · Kristian Boe Helweg Hansen, Compliance Manager

**Draft for management approval — version 0.1. Not in force until approved and issued.**

---

## Purpose and scope

Data & More tells its people what the rules are in a dozen different places, and most of those
places also name a consequence. The Staff Handbook says a breach of confidentiality is gross
misconduct. The access policy says a shared account can cost you your job. The risk management
policy promises an escalation and penalty framework. None of them says who decides, what the
steps are, what is written down, or how long it stays on file.

This document is the single answer to "what happens if someone does not follow our rules." It does
not create new offences. Every rule it enforces already exists somewhere else, and this procedure
points at that source rather than restating it.

It exists for three reasons, in this order:

1. **It is a contractual commitment.** The Danish Data Processing Agreement signed with clients
   states, under *Organisatoriske sikkerhedsforanstaltninger*, item 1, that Data & More develops and
   implements clear security policies defining *"acceptable brugspraksisser, adgangsniveauer,
   dataklassifikationer, ansvar og **sanktioner i tilfælde af overtrædelser**"*. Until this document
   exists, that sentence is not true, and ISAE 3000 control **C.2** is the row where an auditor finds
   the mismatch.
2. **It closes a known control gap.** ISO 27001:2022 **A.6.4 Disciplinary process** is currently
   recorded in our own mapping as *LOW / NOT COVERED*.
3. **It protects the employee as much as the company.** A ladder that is written down is a ladder
   that is applied the same way to everyone, and that cannot be skipped because someone is
   annoyed on a Tuesday.

**Who it covers.** Everyone on the register of appointments who is employed by Data & More.
Contractors and students are covered by a different route — see *Contractors, students and
suppliers* below — because they have no employment relationship to sanction.

**What it does not cover.**

- The employment-law validity of a dismissal, which runs under the employment contract,
  funktionærloven and Danish law generally. This procedure sets out how Data & More reaches a
  decision; it does not determine whether that decision is lawful.
- Complaints *by* an employee about harassment, discrimination or treatment. Those run under
  *Dignity at Work* and the Grievance Procedure. This procedure is what happens to the person
  complained about, once a complaint is upheld.
- The assessment of whether an incident is a personal data breach, which runs under *Procedure
  for Personal Data Breach* (I.2) and is a separate question from whether anyone is at fault.
- Performance that is simply not good enough, absent any rule being broken. That is a
  performance conversation, not a sanction.

---

## Four principles that govern every case

**1. Reporting is never punished. Not reporting is.**

This is the most important sentence in the document and it is already in the Staff Handbook twice
(pages 14 and 27): *"You will not be penalised for reporting an incident in good faith, including one
you caused yourself. Failing to report, or delaying a report, is a disciplinary matter."*

A company that punishes honest reports stops receiving them, and then finds out about its
incidents from its clients. An employee who clicks a phishing link and reports it within the hour has
done the right thing and will be treated as having done the right thing — including where the
clicking itself broke a rule. The same mistake concealed until Monday is a different case entirely.

**2. Proportionality.** The sanction matches the seriousness of what happened, what harm it caused
or risked, whether it was deliberate or careless, whether it has happened before, and whether the
person reported it themselves. A first careless mistake and a deliberate act are not the same thing
and do not get the same answer.

**3. Nobody is sanctioned without being heard.** No step above an informal conversation is decided
before the employee has been told what is alleged, shown what it is based on, and given a real
opportunity to respond. They may bring a colleague or a trade union representative.

**4. The security response is not a sanction and does not wait for one.** Revoking a credential,
suspending access, wiping a device, requiring a password change or requiring re-training are
containment measures. They are taken immediately, by the Service Owner, on the facts available,
and they carry no implication of fault. A person whose access is suspended during an investigation
has not been found guilty of anything.

---

## What can be sanctioned, by area

Every row points at the rule as it already exists. The starting point is where a case normally opens,
not where it ends — the ladder below can move in either direction on the facts.

### A. Confidentiality and client data

| Rule source | Examples of breach | Normal starting point |
|---|---|---|
| Staff Handbook p. 15; Employee Confidentiality Agreement | Discussing client or company confidential matters with an outside organisation or the media | Gross misconduct |
| Confidentiality Agreement; Offboarding and departure procedure | Retaining copies of company or client material after a request to return or delete it | Final written warning to dismissal |
| Staff Handbook p. 15 | Careless disclosure — wrong recipient, open screen in public, discussing a client in a café | Reminder to written warning |

The Handbook's own wording is that a breach of confidentiality *"would be deemed as gross
misconduct … and could lead to your dismissal."* That remains the position. "Deemed gross
misconduct" sets the category; it does not remove the obligation to hear the person and to weigh
whether the disclosure was deliberate, careless or accidental.

### B. Security incident and breach reporting

| Rule source | Examples of breach | Normal starting point |
|---|---|---|
| Staff Handbook pp. 14 and 27; acknowledgement form item 3 (1-hour reporting obligation) | Not reporting a lost or stolen device, a suspected phishing click, or a suspected compromise | Written warning |
| Staff Handbook p. 27 | Delaying a report beyond the point where it could still be contained | Written warning to final written warning |
| — | Deliberately concealing an incident, or giving false information during an assessment | Gross misconduct |
| Staff Handbook p. 27 | Refusing an instruction to disconnect a device, change credentials or stop work on a system during an assessment | Final written warning to dismissal |
| Staff Handbook p. 27 | Contacting a client directly about an incident instead of leaving it to the Compliance Manager | Reminder to written warning |

### C. Access, credentials and administrator rights

| Rule source | Examples of breach | Normal starting point |
|---|---|---|
| Access management and password policy §5.2 | Using a shared account without authorisation, or not following shared-account controls | Written warning; policy already states *"up to and including termination of employment"* |
| Staff Handbook p. 13 | Sharing an account or credential with a colleague | Written warning |
| Staff Handbook p. 13 | Disabling MFA on a service that supports it | Written warning |
| Staff Handbook p. 13 | Reusing passphrases, keeping them in a notes app or spreadsheet, or in a browser profile synced to a personal account | Reminder to written warning |
| Staff Handbook p. 13 | Copying SSH keys or tokens between devices, emailing them, or storing them in a cloud sync folder | Written warning |
| Access management and password policy | Using administrator rights for anything other than a legitimate business purpose | Access removal plus written warning |
| Access management and password policy | Suspected misuse of administrator rights | Immediate revocation and investigation; outcome decides the step |
| — | Accessing client personal data with no business need — curiosity, or looking someone up | Gross misconduct |
| — | Attempting to circumvent access controls, logging or monitoring | Gross misconduct |

### D. Devices, remote work and BYOD

| Rule source | Examples of breach | Normal starting point |
|---|---|---|
| Staff Handbook, *Remote Work and Personal Devices* §3; acknowledgement item 4 | Accessing D&M or client systems from a device that does not meet the device requirements, or that cannot be verified | Access withdrawn; reminder to written warning |
| Staff Handbook §3 | Unencrypted laptop, no screen lock, antivirus or firewall disabled, out-of-date operating system | Reminder to written warning |
| Staff Handbook §5 | Copying client data onto a personal device where a remote or browser-based route was available | Written warning |
| Staff Handbook §1 | Working with client data on an untrusted network or in a place where screens can be overlooked | Reminder to written warning |
| Staff Handbook §8; Offboarding procedure | Not removing D&M and client data from a personal device on leaving, or not confirming it was done | Written warning; and a confidentiality matter if data is retained |
| Staff Handbook p. 25 | Storing company data in a private cloud repository without approval | Written warning |

### E. Acceptable use of systems, email and internet

| Rule source | Examples of breach | Normal starting point |
|---|---|---|
| Staff Handbook p. 15 | Using company computers, email or internet for purposes unrelated to company business, beyond reasonable personal use | Reminder to written warning |
| Staff Handbook p. 15 | Installing unauthorised software on company equipment | Written warning |
| Staff Handbook, *Online meeting etiquette* / *Instant messaging at work* | Conduct in meetings or chat that falls below the stated standard | Reminder |
| — | Use of company systems for anything unlawful, or for material that would amount to harassment | Gross misconduct |

### F. Data protection and processing on instructions

| Rule source | Examples of breach | Normal starting point |
|---|---|---|
| Staff Handbook, *Processing in accordance with instructions*; Data Processing Agreements | Processing client personal data outside the controller's documented instructions | Written warning to dismissal, on the harm |
| Procedure for handling data subject rights (H.1/H.2) | Answering a data subject request directly instead of routing it as the procedure requires | Reminder to written warning |
| Third-country transfer procedure (G.1) | Transferring personal data outside the EEA outside the register and procedure | Written warning to final written warning |
| Erasure policy (D.1/D.3) | Keeping personal data past its retention period, or deleting records that were required to be kept | Reminder to written warning |

### G. Change management, development and test data

| Rule source | Examples of breach | Normal starting point |
|---|---|---|
| Change management policy (B.12); Risk management policy §9 | Making an unauthorised change outside the approved deviation process | Reminder to written warning, on severity — the policy already provides for *"warnings to more severe actions"* |
| Development and test data statement (B.10) | Using live client personal data in a development or test environment | Written warning |
| Secure development policy (B.10) | Bypassing code review, or deploying with known unresolved high-severity vulnerabilities | Written warning |

### H. Suppliers, subprocessors and third parties

| Rule source | Examples of breach | Normal starting point |
|---|---|---|
| Staff Handbook p. 27 | Engaging a supplier who will touch client data without an agreement and, where required, a data processor agreement | Written warning to final written warning |
| Staff Handbook p. 27 | Not consulting the Compliance Manager where there is doubt about supplier risk | Reminder |

### I. Bribery, gifts and conflicts of interest

| Rule source | Examples of breach | Normal starting point |
|---|---|---|
| Staff Handbook p. 27 | Giving or attempting to give a bribe; accepting one, or allowing another person to accept one | Gross misconduct — the Handbook already states formal investigation and *"disciplinary action up to and including dismissal"* |
| Staff Handbook, *Receipt of Gifts* | Accepting hospitality or gifts outside what the policy allows, or not declaring them | Reminder to written warning |
| Staff Handbook p. 10, *Conflict of interests* | Not declaring a conflict of interest | Reminder to written warning |

### J. Diversity, dignity at work and harassment

| Rule source | Examples of breach | Normal starting point |
|---|---|---|
| Staff Handbook p. 29, *Valuing Diversity*, Key Action 1 | Acts that breach the diversity policy — all such breaches *"will be taken seriously, be fully investigated and may be subject to disciplinary action"* | On the finding; serious cases are gross misconduct |
| Staff Handbook, *Dignity at Work* / *What and How of Harassment* | Harassment, bullying or discrimination | Final written warning to gross misconduct |
| — | Victimising someone for raising a complaint or reporting an incident | Gross misconduct |

### K. Attendance, timekeeping and sickness

| Rule source | Examples of breach | Normal starting point |
|---|---|---|
| Staff Handbook p. 9 | Absence claimed as sickness where the person is found not to have been genuinely ill — Handbook: *"disciplinary action, which could include dismissal"* | Final written warning to dismissal |
| Staff Handbook p. 9 | Persistent poor timekeeping — Handbook: *"a potential disciplinary offence under our disciplinary procedures"* | Reminder to written warning |
| Staff Handbook, *Notification of Absence* | Not notifying absence as required | Reminder |

### L. Premises, substances and personal safety

| Rule source | Examples of breach | Normal starting point |
|---|---|---|
| Staff Handbook p. 11 | Bringing or consuming alcohol or unlawful drugs at work, or arriving affected by them — Handbook: *"may lead to your summary dismissal"* | Final written warning to gross misconduct |
| Staff Handbook p. 11 | Smoking, including e-cigarettes, on company premises or in vehicles | Reminder |
| Staff Handbook, *Company Premises* / *Personal Safety* | Breaching premises or safety rules | Reminder to written warning |

---

## The ladder

| Step | What it is | When it is used | Who decides | Recorded | How long it counts |
|---|---|---|---|---|---|
| 0 | Informal conversation | A first, minor, careless matter where a conversation will fix it | Line manager | Manager's note only; not on the personnel file | Not a sanction; carries no weight later |
| 1 | Reminder (*påtale*) | A minor breach, or a repeat of something raised informally | Line manager | Confirmed to the employee in writing; on the personnel file | 6 months |
| 2 | Written warning (*advarsel*) | A breach that matters, or a repeat after a reminder | Line manager with the Compliance Manager | Written, stating the rule, the facts, what must change, and the consequence of repetition | 12 months |
| 3 | Final written warning | A serious breach, or a repeat after a written warning | Compliance Manager, approved by the Partner | As above, stating explicitly that a further breach may end the employment | 12 months |
| 4 | Dismissal with notice (*opsigelse*) | A further breach after a final written warning, or a serious breach not amounting to gross misconduct | The Partner | Written, with reasons | — |
| 5 | Summary dismissal (*bortvisning*) | Gross misconduct | The Partner | Written, with reasons | — |

Three things about the ladder:

**It can be entered at any rung.** Serious conduct starts where it belongs. Nobody works up from a
reminder to reach a dismissal for something that was gross misconduct on day one.

**It can be stepped back down.** A sanction that is appealed and found to have been too heavy is
reduced or withdrawn, and the record is corrected rather than annotated.

**Warnings expire.** After the period in the last column, a warning is spent: it is not counted towards
a later sanction and is not referred to in a later decision. It remains on the personnel file until the
retention period in the Erasure policy runs out, but it stops having effect. A spent warning being
dredged up two years later is itself a failure of this procedure.

The Handbook's existing consequence for a dismissal still applies (p. 34): termination following
disciplinary action will usually attract payment in lieu of notice, assessed case by case, while
dismissal for gross misconduct ends the employment immediately without notice or payment in
lieu.

---

## What counts as gross misconduct

Gross misconduct is conduct that destroys the trust the employment depends on. It can lead to
summary dismissal — the employment ending immediately, without notice or payment in lieu. The
list is not exhaustive, and being on it does not remove the obligation to investigate and to hear the
person.

- Breach of the duty of confidentiality (Staff Handbook p. 15)
- Giving, attempting to give, accepting or permitting a bribe (Staff Handbook p. 27)
- Deliberate unauthorised access to client personal data, or to any data the person has no business
  need to see
- Removing, copying or sending client or company data outside the company for a purpose that is
  not the company's
- Deliberately disabling, circumventing or tampering with a security control, logging or monitoring
- Concealing a security incident or a personal data breach, or giving false information during an
  assessment or investigation
- Falsifying a record, a log, an approval or a compliance document, including a record produced for
  an audit
- Serious harassment, discrimination, violence or threats
- Theft, fraud, or deliberate damage to company or client property
- Being at work unfit through alcohol or unlawful drugs, where the Handbook's summary dismissal
  provision applies (p. 11)
- Serious and deliberate breach of a controller's documented processing instructions

---

## How a case runs

| # | Step | Owner | When |
|---|---|---|---|
| 1 | Concern raised — by a colleague, a manager, a client, a monitoring alert or the person themselves | Anyone | — |
| 2 | Containment decided and carried out, independently of any question of fault | Service Owner | Immediately |
| 3 | Decide whether this is a disciplinary matter at all, or only an incident, a training need or a performance conversation | Compliance Manager | Within 2 working days |
| 4 | Fact-finding: what happened, what the rule says, what the logs and records show, who else was involved | Compliance Manager | Within 10 working days |
| 5 | Employee told in writing what is alleged, on what basis, which rung is being considered, and that they may bring a colleague or trade union representative | Compliance Manager | At least 3 working days before the hearing |
| 6 | Hearing — the employee responds, corrects the facts, and gives any mitigation | Line manager and Compliance Manager | — |
| 7 | Decision, in writing, with reasons, the rung applied, what must change, and how long the sanction counts | Per the ladder table | Within 5 working days of the hearing |
| 8 | Employee may object in writing | Employee | Within 10 working days |
| 9 | Objection reviewed by someone who did not take the decision | The Partner, or the Compliance Manager where the Partner decided | Within 10 working days |
| 10 | Record filed; any lessons fed back into the policy, the training or the control that failed | Compliance Manager | On closure |

Step 10 is not an afterthought. A breach that several people have now committed is usually telling
you that the rule is unclear, the training was thin, or the secure route was harder than the insecure
one. Sanctioning the fourth person and changing nothing is a management failure wearing a
disciplinary costume.

**Where the person deciding is the subject.** If a case concerns the Compliance Manager, the
Partner runs it. If it concerns the Partner, it goes to the other owners of the company, and the
Compliance Manager does the fact-finding.

---

## Precautionary suspension of access

Access may be withdrawn, in whole or in part, while a matter is investigated. This is not a sanction
and is not recorded as one. It is the same measure the *Offboarding and departure procedure*
applies to a departure for cause: immediately on notification, before the conversation ends.

The decision is the Service Owner's, who tells the Partner and the Compliance Manager the same
day. Where suspension means the person cannot do their job, they remain on full pay. Suspension
is reviewed every five working days and lifted as soon as it is no longer needed.

---

## Contractors, students and suppliers

There is no disciplinary ladder for someone the company does not employ, and pretending
otherwise creates a worse problem than it solves — the appearance of an employment relationship
that neither side intended.

| Who | Route |
|---|---|
| Contractors and students on the register of appointments | Instruction to correct; suspension or withdrawal of access; termination of the engagement under its own terms. The confidentiality agreement they signed is enforceable on its own terms, during and after the engagement |
| Suppliers and subprocessors | The agreement and the data processor agreement, under *Supplier management and outsourcing* and the sub-processor risk assessments. Where a supplier's own personnel breach our requirements, we raise it with the supplier, not with their staff |

Access consequences apply identically regardless of engagement type. A contractor who conceals
an incident loses access on the same day an employee would.

---

## Records, personal data and retention

A disciplinary record is personal data about the employee, and some of it is sensitive. It is handled
accordingly.

| What is kept | Where | Who can see it |
|---|---|---|
| Reminders, written warnings, final written warnings, dismissal letters | Personnel file | The employee, their line manager, the Compliance Manager, the Partner |
| Investigation notes and the evidence relied on | Case file, held by the Compliance Manager | The Compliance Manager, the Partner, and the employee on request |
| The decision and any objection | Personnel file | As above |
| Anonymised case count, by area and rung | Management report | Management |

**Lawful basis.** Performance of the employment contract and compliance with legal obligations as
an employer, Article 6(1)(b) and 6(1)(c), together with the legitimate interest in enforcing the
security commitments the company has made to its clients, Article 6(1)(f). Where health data arises
— a sickness absence case — the Handbook's health provisions and Article 9 apply.

**Retention.** Warnings are already covered by the Erasure policy v5 §6.2, employee personnel files
and registers, which expressly names warnings: erased after termination of employment once no
longer relevant, and at the latest five years after the calendar year of termination. This procedure
adds nothing to that period. The expiry of a warning's *effect* (6 or 12 months) is a different thing
from the deletion of the *record*, and the two should not be confused.

**The employee's rights.** The employee may ask for a copy of their disciplinary record, ask for a
factual error in it to be corrected, and add their own statement to the file. Procedure H.1/H.2 applies
to such a request as it does to any other.

**What is not kept.** No record is made of an informal conversation on the personnel file, and the
monitoring provisions in the Handbook are not extended by this procedure. Nothing here authorises
reading an employee's mailbox or monitoring their activity beyond what the Handbook already
permits and the conditions it already sets.

---

## Review, ownership and audit mapping

**Owner:** the Compliance Manager. **Approver:** Lars Taxgaard, Partner. Reviewed annually, or
sooner if the Staff Handbook, the access model or the employment terms change.

| Control | What it asks | Where this document answers it |
|---|---|---|
| DPA, *Organisatoriske sikkerhedsforanstaltninger* item 1 | Policies defining responsibility and sanctions in the event of violations | This document, referenced from the Information security policy |
| ISO 27001:2022 A.6.4 | A disciplinary process for personnel who have committed a security breach | The ladder, the gross misconduct list, and the case procedure |
| ISAE 3000 C.1 | An approved, reviewed information security policy | This document is part of the policy set, approved alongside it |
| ISAE 3000 C.2 | The policy does not conflict with the data processing agreements entered into | Closes the gap between the DPA's sanctions commitment and the policy set |
| ISAE 3000 C.4 | Employees introduced to the information security policy and processing procedures on appointment | Added to the induction record; acknowledgement covers this document |
| ISAE 3000 C.6 | Employees informed that confidentiality continues after departure | Section A is the in-employment enforcement of the same duty |
| ISAE 3000 C.7 | Awareness training | Sanctions are a stated topic in induction and annual refresher training |
| ISAE 3000 B.6 / B.13 | Access management | Section C, and the access consequences the access policy already states |
| ISO 27001:2022 A.5.4 | Management responsibilities for applying policy | The ladder names a decision-maker at every rung |

---

## Changes this creates elsewhere

Approving this document does not make the rest of the documentation consistent by itself. Four
things have to follow it.

| Document | Change needed | State, 26 October 2026 |
|---|---|---|
| Information security policy and objectives (C.1) | Add a *Responsibility and consequences of non-compliance* clause referring to this procedure. This is what makes the DPA's sanctions commitment true, and it is the one change that cannot be skipped | **Drafted, not applied.** The policy is generated by Cyberday and cannot be edited from the repository. Clause text, placement and the re-export steps are in [`INFOSEC_POLICY_SANCTIONS_CLAUSE.md`](INFOSEC_POLICY_SANCTIONS_CLAUSE.md), in English and Danish. Blocked on approval of this procedure |
| Staff Handbook v5 | Three sections cite *"the Company's disciplinary procedures"* (pp. 9, 11, 27) with nothing to cite. Point them at this document, and add it to the contents and to the acknowledgement form | **Part (a) applied** 26 October 2026 as pending suggestions in the Google Doc — the three cross-references now name this procedure. Parts (b) to (d) are held in Item 20 of [`STAFF_HANDBOOK_REDLINE.md`](STAFF_HANDBOOK_REDLINE.md): (b) and (c) pending the employment-law review, (d) to be folded into Item 9 rather than applied on top of it |
| ISO 27001 mapping | Record that A.6.4 is answered, without claiming an ISAE control maps to it | **Done.** A.6.4 in [`ISO_27001_2022_ISAE_3000_Mapping.md`](ISO_27001_2022_ISAE_3000_Mapping.md), plus the quick reference and the coverage summary. The ISAE column stays `—`, because no ISAE control asks for a disciplinary process; the alignment now reads *NO ISAE COUNTERPART — COVERED BY D&M DOCUMENT* |
| Description of processing (C.1–C.7 summary) | The placeholder block mislabelled C.4 as "Disciplinary procedures" | **Done.** All seven lines were wrong, not just C.4 — the list had drifted a position or more against the Elumi request list. Replaced with the request list's own wording in [`DESCRIPTION_OF_PROCESSING_ISAE3000.md`](DESCRIPTION_OF_PROCESSING_ISAE3000.md) |

---

## Open points

- [ ] **A Danish employment-law review of the ladder, the hearing steps and the notice periods.** The
      structure follows ordinary Danish practice, but whether a particular warning will support a later
      dismissal is a legal question and this document should not be relied on as the answer to it.
- [ ] Decide whether the warning expiry periods (6 and 12 months) are right for a company this size,
      or whether a single 12-month period is simpler to apply.
- [ ] Confirm who holds the Service Owner role, so the containment and suspension steps name a
      person. The same open point is recorded in the offboarding procedure.
- [ ] Decide whether contractors and students re-acknowledge this document, or whether the
      confidentiality agreement and access terms are enough.
- [ ] Agree how an existing employee acknowledges a document issued mid-employment —
      re-acknowledgement of the Handbook, or a separate signature.
- [ ] Decide whether the anonymised case count goes into the annual management review, and
      whether a nil return is stated explicitly for the audit period.

---

Version 0.1 (draft) | Date of implementation: *pending approval* | Approver: Lars Taxgaard, Partner |
Next review: one year from implementation
