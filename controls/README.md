# Controls

This directory holds the Idowu Ajiri Foundation's control framework. Controls are the specific activities and safeguards the foundation maintains to satisfy its legal and regulatory obligations in the US and Nigeria.

## Structure

```
controls/
├── README.md
├── control-index.md          # Master list of all controls, cross-referenced by jurisdiction
├── us/                       # Controls specific to US obligations
│   ├── us-ctrl-001-ofac-sanctions-screening.md
│   ├── us-ctrl-002-irs-public-disclosure.md
│   └── us-ctrl-003-state-charity-registration.md
└── ng/                       # Controls specific to Nigerian obligations
    ├── ng-ctrl-001-scuml-registration-renewal.md
    ├── ng-ctrl-002-cac-annual-return.md
    └── ng-ctrl-003-cbn-ngo-reporting.md
```

## Control Record Format

Each control file uses the template at `templates/control-record-v1.md`. Key fields:

| Field | Description |
|---|---|
| Control ID | Unique identifier (e.g., `US-CTRL-001`) |
| Regulatory citation | Specific rule or statute the control addresses |
| Jurisdiction | US, NG, or GLOBAL |
| Control owner | Named individual responsible for operation and testing |
| Control type | Preventive / Detective / Corrective |
| Testing frequency | Continuous / Monthly / Quarterly / Annual |
| Last tested | Date of most recent test |
| Test result | Pass / Fail / Exception noted |
| Evidence reference | Path or URL to supporting evidence |

## Control Numbering

- `US-CTRL-NNN` — US-jurisdiction controls
- `NG-CTRL-NNN` — Nigeria-jurisdiction controls
- `GL-CTRL-NNN` — Global / cross-jurisdiction controls

Add new controls by incrementing the sequence within each prefix. Never reuse a retired control ID; mark it `[RETIRED]` in the index instead.
