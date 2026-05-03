# Reports

This directory holds finalized compliance reports and the working files used to prepare regulatory filings. Reports in this folder have been reviewed and approved per the process in `CONTRIBUTING.md`.

## Structure

```
reports/
├── README.md
├── board/                          # Quarterly and annual board compliance reports
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

## Report Types

### Board Compliance Reports (`board/`)
Quarterly summaries covering: control testing results, risk register changes, screening exceptions, policy updates, and open audit findings. Presented to the board at each quarterly meeting. Format: `YYYY-QN-compliance-report.md`.

### IRS Form 990 Support (`us/990/`)
Working documentation supporting the annual Form 990 filing, including revenue and expense reconciliation, program accomplishment narratives, and governance questionnaire responses. The actual signed return is stored in the secure drive; this folder holds the preparation record.

### State Charity Registration (`us/state-charity/`)
Renewal tracking and correspondence for each US state where the foundation solicits donations. Includes filing dates, confirmation numbers, and next renewal deadlines.

### CAC Annual Return Support (`ng/cac/`)
Documentation supporting the annual return filed with Nigeria's Corporate Affairs Commission under CAMA 2020, including financial statement attachments and officer details.

### SCUML Annual Return Support (`ng/scuml/`)
Supporting documentation for the annual return filed with the Special Control Unit Against Money Laundering. Includes AML/CFT program summary, transaction statistics, and suspicious transaction report (STR) count for the year. Due by 30 June each year.

## Report File Format

Each report uses the relevant template from `templates/`. Report filenames follow the pattern:

```
YYYY-[QN|type]-short-description.md
```

Draft reports live on a feature branch until approved. Merging to `main` signals the report is final.
