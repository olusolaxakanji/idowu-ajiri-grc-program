# Reports

Reports are what connect the compliance programme to the people responsible for it. The board cannot govern what it cannot see. Regulators cannot audit what is not documented. This directory contains the records produced to give both groups the visibility they need.

Two types of documents live here: board compliance reports presented at each quarterly meeting, and regulatory filing support files that document how each annual return was prepared.

---

## Directory Structure

```
reports/
├── README.md
├── board/                          # Quarterly board compliance reports
│   ├── 2026-Q1-compliance-report.md
│   └── ...
├── us/                             # US regulatory filing support files
│   ├── 990/
│   │   └── 2025-form-990-support.md
│   └── state-charity/
│       └── 2025-state-registration-renewal.md
└── ng/                             # Nigerian regulatory filing support files
    ├── cac/
    │   └── 2025-cac-annual-return-support.md
    └── scuml/
        └── 2025-scuml-annual-return-support.md
```

---

## Board Compliance Reports (`board/`)

Quarterly reports presented to the board at each quarterly meeting. The board has governance responsibility for the foundation's compliance posture. Without a structured quarterly report, HIGH and CRITICAL risks go unescalated and regulatory deadlines go untracked.

Each report covers:

- **Control testing results:** Pass/fail status for each control tested during the quarter, with open exceptions and their resolution status
- **Risk register summary:** Count by level (CRITICAL / HIGH / MEDIUM / LOW) and any changes from the prior quarter, with board attention items called out specifically
- **Screening activity:** Number of screens completed, clear results, false positives investigated, and any confirmed hits with disposition
- **Policy updates:** Any policies approved or revised during the quarter
- **Regulatory developments:** Changes to US or Nigerian law or regulation requiring a policy or control response
- **Upcoming compliance deadlines:** Owner and current status for each
- **Recommendations:** Items requiring board decision, approval, or budget authority

Reports are reviewed by the Board Treasurer before distribution. Both the Compliance Officer and the Board Treasurer sign the final version. Merging to `main` signals the report is final and approved for the board record.

**Current upcoming deadlines tracked in board reports:**

| Deadline | Obligation | Owner |
|---|---|---|
| 15 May 2026 (or extension) | IRS Form 990 filing | Finance Lead |
| 30 Jun 2026 | SCUML Annual Return | Compliance Officer |
| 30 Jun 2026 | CAC Annual Return | Finance Lead |

---

## IRS Form 990 Support (`us/990/`)

The Form 990 is a public document. IRS auditors and major donors can request it. This folder holds the working documentation behind each annual filing: revenue and expense reconciliation, program accomplishment narratives, and governance questionnaire responses.

The signed return is stored in the designated secure drive. This folder holds the preparation record that shows how figures were derived and which supporting documents were relied on. If IRS asks "how did you arrive at this program service revenue figure," this file has the answer.

---

## State Charity Registration (`us/state-charity/`)

The foundation must maintain active state charity registrations in each US state where it solicits donations. Filing lapses can result in unlawful solicitation exposure. This folder tracks renewal dates, filing confirmation numbers, and correspondence for each required state registration.

---

## CAC Annual Return Support (`ng/cac/`)

Nigeria's Corporate Affairs Commission requires an annual return under CAMA 2020. This folder holds supporting documentation: financial statement attachments, officer details, and the filing confirmation. The Nigerian entity's legal standing depends on this filing being current.

---

## SCUML Annual Return Support (`ng/scuml/`)

The SCUML annual return is due by 30 June each year. Late filing can result in regulatory sanction or deregistration: RISK-003 in the master risk register, currently rated HIGH. This folder holds the AML/CFT programme summary, transaction statistics, suspicious transaction report count, and any additional documentation SCUML requires.

---

## File Naming Convention

```
YYYY-[QN|type]-short-description.md
```

Draft reports live on a feature branch until approved. Merging to `main` signals the report is final.

---

## Related Documentation

| Document | Description |
|---|---|
| [Risk Register](../risk-register/README.md) | Risk register data summarised in each board report |
| [Controls](../controls/README.md) | Control testing results reported to the board quarterly |
| [Screening](../screening/README.md) | Screening activity data included in each board report |
