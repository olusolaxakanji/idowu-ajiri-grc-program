# Idowu Ajiri Foundation — GRC Programme

**Live compliance programme. Dual jurisdiction. Active programme.**

The Idowu Ajiri Foundation is a pre-operational nonprofit in IRS 501(c)(3) formation in the United States, registered under Nigerian (CAC/SCUML) regulatory frameworks. This repository contains the full governance, risk, and compliance programme I built and maintain as Compliance Officer. The conflict-of-interest disclosure memo in this repository is in my name.

This is not a simulation. Every policy, control, screening log, and board report reflects the foundation's actual regulatory obligations.

---

## The Compliance Problem This Programme Solves

A nonprofit operating across US and Nigerian regulatory regimes does not face two separate compliance tracks. It faces a single set of operations subject to two sets of rules that sometimes conflict, often overlap, and always run on different calendars.

The Nigerian entity is active under CAC registration with live SCUML AML/CFT obligations. The US entity is in pre-operational IRS 501(c)(3) formation. The programme covers both jurisdictions proactively: governance infrastructure was built before US operations became active, not after the first compliance failure.

The specific problems this programme addresses:

- A single donor can appear on both OFAC's SDN list and EFCC/SCUML watch lists. Screening against one list is not sufficient.
- SCUML classifies Nigerian nonprofits as Designated Non-Financial Businesses and Professions, which triggers formal AML/CFT reporting and record-keeping obligations most NGOs are not aware of.
- Cross-border fund flows between the US and Nigerian entities create simultaneous CBN fund management and FinCEN BSA exposure.
- Donor PII collected in Nigeria is governed by NDPR. Transfer of that data to the US creates dual-jurisdiction data protection exposure.
- IRS 501(c)(3) status depends on annual Form 990 compliance. Missing or inaccurate filings can result in automatic revocation.

---

## Programme Structure

```
idowu-ajiri-grc-program/
├── policies/           # Governance policies by jurisdiction
│   ├── global/         # Cross-jurisdiction policies (Code of Conduct, Anti-Bribery, COI, Whistleblower, Data Protection)
│   ├── us/             # US-specific policies (AML/CFT, OFAC sanctions, Document Retention)
│   └── ng/             # Nigeria-specific policies (SCUML AML/CFT, CBN Fund Management, NDPR)
├── controls/           # Control framework mapped to US and Nigerian obligations
├── risk-register/      # Master risk register with inherent/residual ratings and board escalation rules
├── screening/          # Donor, vendor, and grantee due-diligence records
├── evidence/           # Audit evidence, attestations, and compliance artifacts
├── reports/            # Board compliance reports and regulatory filing support
└── templates/          # Reusable blank templates for all document types
```

---

## Regulatory Scope

| Framework | Governing Body | Jurisdiction | Obligation Type |
|---|---|---|---|
| IRS 501(c)(3) | Internal Revenue Service | United States | Tax-exempt status, Form 990 annual filing |
| Corporate Affairs Commission (CAC) | CAC Nigeria | Nigeria | Legal registration, CAC annual return |
| SCUML / NFIU AML/CFT | Nigerian Financial Intelligence Unit | Nigeria | AML/CFT programme, suspicious transaction reporting |
| CBN NGO Circular | Central Bank of Nigeria | Nigeria | Cross-border fund management, bank account controls |
| EFCC Act | Economic and Financial Crimes Commission | Nigeria | Anti-corruption, financial crime prevention |
| FCPA | U.S. Department of Justice | United States | Anti-bribery for international operations |
| NDPR / Nigeria Data Protection Act 2023 | Nigeria Data Protection Commission | Nigeria | Donor PII, cross-border data transfer |
| OFAC Sanctions | U.S. Department of the Treasury | United States (cross-border) | Donor, vendor, and grantee screening |
| FinCEN BSA / 31 CFR Part 1010 | Financial Crimes Enforcement Network | United States | AML/CFT for cross-border fund flows |

---

## Policies

### Global (Cross-Jurisdiction)

| Policy | What it governs |
|---|---|
| [Code of Conduct](./policies/global/POL-GL-001-code-of-conduct.md) | Baseline standards of behaviour for all staff, volunteers, and board members across both jurisdictions. Anchors the disciplinary framework referenced in all other policies. |
| [Anti-Bribery and Corruption Policy](./policies/global/POL-GL-002-anti-bribery-corruption.md) | FCPA and Nigerian anti-corruption law apply simultaneously to the foundation's international operations. This policy defines prohibited conduct, gift and hospitality limits, and the reporting path for suspected violations. |
| [Conflict of Interest Policy](./policies/global/POL-GL-003-conflict-of-interest.md) | Board members and staff with financial interests in foundation vendors or grantees create legal and reputational exposure. This policy requires annual disclosure, defines recusal procedures, and governs how conflicts are documented and resolved. |
| [Whistleblower Protection Policy](./policies/global/POL-GL-004-whistleblower-protection.md) | Staff who identify compliance violations need a protected channel to report them. This policy establishes the anonymous reporting mechanism and prohibits retaliation, addressing the specific vulnerability of small nonprofit governance structures. |
| [Data Protection and Privacy Policy](./policies/global/POL-GL-005-data-protection-privacy.md) | Donor PII collected in Nigeria falls under NDPR. The same records transferred to the US create exposure under applicable state privacy laws. This policy defines the lawful basis for collection, cross-border transfer conditions, retention periods, and data subject rights procedures for both regimes. |

### United States

| Policy | What it governs |
|---|---|
| [AML/CFT Programme (US)](./policies/us/POL-US-001-aml-cft-program.md) | The foundation cannot accept contributions without a defensible AML risk assessment. This policy establishes the risk-based approach, customer due diligence standards, and SAR filing obligations under FinCEN 31 CFR Part 1010. |
| [OFAC Sanctions Compliance Policy](./policies/us/POL-US-002-ofac-sanctions-compliance.md) | One confirmed sanctions hit can result in civil monetary penalties, asset freezing, and reputational damage that threatens the foundation's operating capacity. This policy sets the screening cadence, escalation path, and fund-blocking procedures for donors, vendors, and grantees. |
| [Document Retention Policy](./policies/us/POL-US-003-document-retention.md) | IRS audits and OFAC investigations both require the ability to produce records on demand. This policy defines retention periods by document type, secure disposal procedures, and litigation hold protocols. |

### Nigeria

| Policy | What it governs |
|---|---|
| [SCUML AML/CFT Programme (Nigeria)](./policies/ng/POL-NG-001-scuml-aml-cft-program.md) | SCUML classifies Nigerian nonprofits as DNFBPs, which triggers formal registration, annual return, and suspicious transaction reporting obligations that most NGOs are not structured to meet. This policy addresses each obligation specifically. |
| [CBN NGO Fund Management Policy](./policies/ng/POL-NG-002-cbn-ngo-fund-management.md) | The CBN circular on NGO fund management creates bank account designation requirements and cross-border fund transfer controls for foreign-linked nonprofits. This policy operationalizes those requirements for the foundation's US-Nigeria fund flows. |
| [NDPR Data Handling Policy](./policies/ng/POL-NG-003-ndpr-data-handling.md) | Donor and beneficiary records collected in Nigeria are governed by the Nigeria Data Protection Act 2023. This policy defines the lawful basis, data subject rights, retention schedules, and the specific obligations that apply when records are transferred to the US entity. |

---

## Risk Register

The [master risk register](./risk-register/master-risk-register.md) tracks 10 risks across compliance, financial, operational, and reputational categories.

**Two risks are currently rated HIGH and receive board attention quarterly:**

- **RISK-001:** Foundation receives funds from an OFAC-sanctioned entity due to incomplete screening. Inherent rating 25 (Critical). Residual rating 10 (HIGH) after OFAC screening controls. OFAC violations carry civil monetary penalties and potential criminal referral.
- **RISK-003:** SCUML annual return filed late, triggering regulatory sanction or deregistration. Inherent rating 15 (HIGH). Residual rating 10 (HIGH). SCUML deregistration would suspend the foundation's legal authority to operate in Nigeria.

Each register entry carries: risk description, category, jurisdiction, inherent rating (likelihood x impact), current controls, residual rating, risk owner, and next review date.

---

## Screening Programme

The foundation screens all donors, vendors, and grantees before engagement and on a defined re-screening cycle.

| Log | Lists Checked | Cadence |
|---|---|---|
| [Donor Screening Log](./screening/logs/donor-screening-log.md) | OFAC SDN, OFAC Consolidated, SCUML/EFCC | At onboarding; annual re-screen |
| [Vendor Screening Log](./screening/logs/vendor-screening-log.md) | OFAC SDN, OFAC Consolidated, SCUML/EFCC | At onboarding; annual re-screen |
| [Grantee Screening Log](./screening/logs/grantee-screening-log.md) | OFAC SDN, OFAC Consolidated, SCUML/EFCC, CAC | At onboarding; annual re-screen |

Each screening record logs: entity name, screen date, lists checked, tool or source used, result, approver, and re-screen due date. The [exception log](./screening/exceptions/exception-log.md) captures false positives and confirmed hits with full disposition records.

---

## Board Reporting

The [Q2 2026 Board Compliance Report](./reports/board/2026-Q2-compliance-report.md) is the most recent quarterly report. The [Q1 2026 Board Compliance Report](./reports/board/2026-Q1-compliance-report.md) is also available. Both follow the standard format for quarterly board reporting. Each report covers:

- Control testing results for the quarter, with pass/fail status and open exceptions
- Risk register movement: count by level and any changes from the prior quarter
- Screening activity: screens completed, clear results, false positives, and confirmed hits
- Policy updates effective during the quarter
- Regulatory developments requiring board awareness
- Upcoming compliance deadlines with owner and current status
- Recommendations requiring board decision or approval

Reports are reviewed by the Board Treasurer before distribution. Approval signatures are required before the report is marked final.

---

## Controls

The [control index](./controls/control-index.md) maps each control to the regulatory obligation it satisfies, the control owner, testing frequency, and current status. Controls are organized by jurisdiction.

Key controls include:

- **US-CTRL-001:** OFAC Sanctions Screening (quarterly)
- **NG-CTRL-001:** SCUML Registration and Annual Return (annual)
- **GL-CTRL-001:** Board Governance and Meeting Quorum (quarterly)
- **GL-CTRL-002:** Conflict of Interest Annual Disclosure (annual)

---

## Templates

All document types used in this programme have version-controlled blank templates in [`/templates/`](./templates/). When creating a new control record, risk entry, policy, evidence log, screening record, or board report, copy the relevant template rather than drafting from scratch. Templates carry version numbers in their filenames.

---

---

**Compliance Officer:** Olusola B. Akanji
**Last programme review:** 2026-Q2
**Next scheduled review:** 2026-Q3 (October 2026)
