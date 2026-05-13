# Evidence

Evidence is the primary basis for any audit, regulatory inspection, or donor inquiry. A policy says what the foundation must do. A control defines how the foundation tests that it is doing it. Evidence is what proves the test was performed and what the result was.

When IRS asks to see how Form 990 data was prepared, when SCUML inspects AML/CFT programme records, or when a major donor asks how the foundation screens its grantees: this is the folder that provides the answer.

---

## Directory Structure

```
evidence/
├── README.md
├── 2026/
│   ├── US-CTRL-001/     # One folder per control ID, per year
│   ├── US-CTRL-002/
│   ├── NG-CTRL-001/
│   └── GL-CTRL-001/
└── 2025/
    └── ...
```

Each control folder contains evidence files named with the test date and a short description:

```
2026/US-CTRL-001/
├── 2026-01-15_ofac-screen-jan-donors.md
├── 2026-04-10_ofac-screen-apr-donors.md
└── 2026-04-10_ofac-screen-q1-vendors.md
```

---

## File Naming Convention

```
YYYY-MM-DD_short-description.md
```

Use hyphens, no spaces. Descriptions under 50 characters. ISO date format always.

---

## What Belongs Here

- Test result summaries: pass/fail status, exceptions noted, remediation taken
- Screenshots of system checks exported as PDF or linked to secure drive
- Signed attestation forms
- Regulatory correspondence: filing confirmations, acknowledgement letters, regulator communications
- Third-party certifications or audit reports (linked by secure-drive URL if the file is large)

## What Does NOT Belong Here

- Original PII: donor SSNs, passport scans, bank account numbers. Store these in the designated secure drive and reference by URL in the evidence record.
- Files larger than 10 MB: link to secure drive instead of committing.
- Attorney-client privileged communications: these must remain outside this repository.

---

## Evidence Record Format

Each evidence file uses `templates/evidence-record-v1.md`. Required fields: control ID, test date, tester, test description, result (Pass/Fail/Exception), exceptions noted, remediation taken (if applicable), and secure-drive link (if applicable).

---

## Retention

Evidence is retained for a minimum of **7 years** from the date of the record.

The 7-year period reflects the longer of two requirements: IRS record-keeping guidance for 501(c)(3) organizations and Nigerian CAMA 2020 requirements (6 years). When requirements conflict, the more stringent period governs.

Do not delete any year folder without Compliance Officer written approval. Deletion of evidence records without approval constitutes a compliance failure.

---

## Related Documentation

| Document | Description |
|---|---|
| [Controls](../controls/README.md) | The controls that produce these evidence records |
| [Reports](../reports/README.md) | Board and regulatory reports that summarise control testing results |
| [Screening](../screening/README.md) | Screening records, which are a specific category of evidence |
