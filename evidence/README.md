# Evidence

This directory stores artifacts that demonstrate controls are operating as designed. Evidence is the primary basis for internal and external audits.

## Structure

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

## Evidence File Naming Convention

```
YYYY-MM-DD_short-description.md
```

Use hyphens, no spaces. Keep descriptions under 50 characters.

## What Belongs Here

- Test result summaries (pass/fail, exceptions noted, remediation taken)
- Screenshots of system checks (exported as PDF or linked to secure drive)
- Signed attestation forms
- Regulatory correspondence (confirmation of filings, acknowledgement letters)
- Third-party certifications or audit reports (linked by secure-drive URL if large)

## What Does NOT Belong Here

- Original PII (donor SSNs, passport scans, bank account numbers) — store these in the designated secure drive and reference by URL
- Files larger than 10 MB — link to secure drive instead
- Attorney-client privileged communications — these must remain outside this repository

## Evidence Record Format

Each evidence file uses the template at `templates/evidence-record-v1.md`. Key fields: control ID, test date, tester, test description, result, exceptions, remediation (if any), and secure-drive link (if applicable).

## Retention

Evidence is retained for a minimum of 7 years in line with IRS record-keeping guidance for 501(c)(3) organizations and Nigerian CAMA 2020 requirements (6 years), whichever is longer. Do not delete any year folder without Compliance Officer approval.
