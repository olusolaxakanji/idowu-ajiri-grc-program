# Contributing to the GRC Program

This document defines how changes are proposed, reviewed, approved, and merged into the Idowu Ajiri Foundation GRC repository.

---

## Roles and Ownership

| Role | Responsibility |
|---|---|
| **Compliance Officer** | Owns the program; final approver on all policy and control changes |
| **Finance Lead** | Primary reviewer for financial controls, risk entries, and 990/SCUML filings |
| **Program Director** | Reviewer for operational risk and policy changes affecting program delivery |
| **Board Treasurer** | Approves quarterly and annual compliance reports before they are finalized |
| **External Auditor** | Read-only access; receives evidence packages via secure export |

---

## Review Cadence

### Continuous (on every change)
- All edits are made on a feature branch and submitted as a pull request.
- PR title format: `[type] short description` where type is one of `policy`, `control`, `risk`, `evidence`, `screening`, `report`, or `template`.
- At least one reviewer must approve before merging. Changes to policies or controls require the Compliance Officer as one of the approvers.

### Monthly
- **Risk register triage**: Compliance Officer reviews any risks flagged `HIGH` or `CRITICAL` and confirms residual ratings are current.
- **Screening log review**: Finance Lead confirms all active donors and vendors screened within the last 90 days have no outstanding exceptions.
- **Evidence freshness check**: Spot-check that evidence linked to controls tested on a quarterly or monthly cadence has been updated.

### Quarterly
- **Full control testing cycle**: Each control owner completes testing per the frequency defined in the control record and commits results to `evidence/`.
- **Compliance summary report**: Compliance Officer drafts the quarterly board report in `reports/` and submits it to the Board Treasurer for approval at least one week before the board meeting.
- **Risk register refresh**: All risk owners review and attest to their risk entries. Ratings are updated if circumstances have changed.

### Annually
- **Policy review**: Every policy in `policies/` is reviewed for continued accuracy against current law and foundation operations. Policies not materially changed are re-dated and re-attested. Policies requiring amendment go through the standard PR process.
- **Control framework review**: The control index is compared against any regulatory changes in the US or Nigeria during the year. New obligations are added; retired obligations are archived with an explanatory note rather than deleted.
- **IRS Form 990 and CAC Annual Return**: Finance Lead prepares support files in `reports/us/` and `reports/ng/` respectively. Compliance Officer and Board Treasurer review before filing.
- **SCUML Annual Return**: Filed by June 30 each year. Support documentation committed to `reports/ng/scuml/`.
- **Full GRC program retrospective**: Compliance Officer facilitates a review of the program's effectiveness, updates this CONTRIBUTING.md if process changes are needed, and presents findings to the board.

---

## Branch and Commit Conventions

- Branch names: `type/short-slug` — e.g., `policy/aml-update-2026`, `risk/fx-exposure-q2`.
- Commit messages: imperative mood, ≤72 characters on the first line — e.g., `Add OFAC screening log for Q1 2026`.
- Do not commit personally identifiable information (PII), passwords, API keys, or documents that are subject to attorney-client privilege. Privileged documents are referenced by a secure-drive URL.

---

## Archiving vs. Deleting

Records must never be hard-deleted from `main`. Instead:
- Superseded policies are moved to `policies/archive/` with a note referencing the replacement.
- Resolved risks are moved to `risk-register/archive/` and their final status recorded.
- Outdated evidence is retained in `evidence/` under its original control ID and year folder.

Retention periods follow US IRS record-keeping guidance (generally 7 years for financial records) and Nigerian CAMA 2020 requirements (6 years for accounting records), whichever is longer.

---

## Questions

Raise questions or flag potential compliance issues by opening a GitHub Issue with the label `compliance-question`. For urgent matters, contact the Compliance Officer directly.
