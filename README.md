# Idowu Ajiri Foundation — GRC Program

Governance, Risk, and Compliance repository for the Idowu Ajiri Foundation, a dual-jurisdiction nonprofit operating under US (IRS 501(c)(3)) and Nigerian (CAC/SCUML) regulatory frameworks.

---

## Repository Structure

```
idowu-ajiri-grc-program/
├── controls/           # Control framework mapped to US and Nigerian obligations
├── risk-register/      # Identified risks, likelihood/impact ratings, and treatment plans
├── policies/           # Organizational policies and procedures
├── evidence/           # Audit evidence, attestations, and compliance artifacts
├── screening/          # Donor, vendor, and partner due-diligence records
├── reports/            # Board compliance reports, regulatory filings, and audit summaries
└── templates/          # Reusable blank templates for all above categories
```

---

## Folder Descriptions

### `controls/`
Contains the control framework linking each control to the regulatory requirement it satisfies, the control owner, testing frequency, and current status. Organized by jurisdiction (`us/`, `ng/`) with a shared cross-jurisdiction index.

**Key regulations covered:**
- US: IRS 501(c)(3) public charity rules, OFAC sanctions, FinCEN 31 CFR Part 1010, FCPA, state charity registration requirements
- Nigeria: CAC (Companies and Allied Matters Act 2020), SCUML registration and AML obligations, EFCC Act, CBN NGO circular, CAMA filing requirements

### `risk-register/`
Tracks the foundation's risk universe across operational, financial, reputational, and compliance categories. Each entry records risk description, inherent rating, current controls, residual rating, risk owner, and next review date. A master register links both jurisdictions; sub-folders hold working files per risk domain.

### `policies/`
Approved policies governing foundation operations. Each policy document states its scope, effective date, review date, approving authority, and the regulatory obligation it addresses. Sub-folders separate US-specific, Nigeria-specific, and global (cross-jurisdiction) policies.

### `evidence/`
Stores artifacts that demonstrate control operation: screenshots, signed attestations, test results, third-party certifications, and correspondence with regulators. Organized by control ID and calendar year so evidence can be quickly retrieved during audits.

### `screening/`
Due-diligence records for donors, vendors, grantees, and partners. Includes OFAC SDN/OFSI checks, PEP (politically exposed person) screening, and CAC entity verification results. Each record captures the screening date, tool used, outcome, and approver.

### `reports/`
Finalized compliance reports presented to the board or submitted to regulators. Includes quarterly compliance summaries, annual IRS Form 990 support files, SCUML annual returns support files, and external audit findings with management responses.

### `templates/`
Blank, version-controlled templates for every document type used in this program. When starting a new control record, policy, evidence log, screening form, or report, copy the relevant template rather than creating from scratch. Templates carry a version number in their filename.

---

## Jurisdiction Quick Reference

| Topic | US Authority | Nigerian Authority |
|---|---|---|
| Legal registration | IRS / State AG | CAC |
| AML / CFT | FinCEN / OFAC | SCUML / EFCC |
| Anti-corruption | DOJ (FCPA) | EFCC / ICPC |
| Data privacy | State laws (CCPA etc.) | NDPR (NITDA) |
| Annual filing | IRS Form 990 | CAC Annual Return |
| Banking | FinCEN BSA rules | CBN NGO circular |

The Nigerian entity is active under CAC registration; the US entity is currently in the pre-operational formation phase under the IRS 501(c)(3) framework. The GRC program covers both jurisdictions proactively to ensure compliance readiness precedes full US operational activity.

---

## Getting Started

1. Clone this repository.
2. Read `CONTRIBUTING.md` for review cadence and ownership rules.
3. All substantive changes require a pull request reviewed by the Compliance Officer before merging to `main`.
4. Evidence files larger than 10 MB should be stored in the designated secure drive and linked by URL in the evidence record — do not commit large binaries here.
