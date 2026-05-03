# Screening

This directory holds due-diligence records for all parties with whom the Idowu Ajiri Foundation has a financial or programmatic relationship: donors, grantees, vendors, and partners.

## Structure

```
screening/
├── README.md
├── logs/
│   ├── donor-screening-log.md       # Running log of all donor screens
│   ├── vendor-screening-log.md      # Running log of all vendor screens
│   └── grantee-screening-log.md     # Running log of all grantee/partner screens
├── records/
│   ├── donors/                      # Individual screen records by entity name
│   ├── vendors/                     # Individual screen records by vendor name
│   └── grantees/                    # Individual screen records by grantee name
└── exceptions/
    └── exception-log.md             # Any hit, false positive, or escalated case
```

## Screening Requirements

### US Obligations
- **OFAC SDN List** (Office of Foreign Assets Control): All donors, vendors, and grantees screened before first transaction and re-screened at least annually.
- **OFAC Consolidated Sanctions List**: Checked in the same pass as SDN.
- **PEP Screening** (Politically Exposed Persons): Required for any foreign national donor or partner contributing above $10,000.
- **FinCEN 314(a) awareness**: Staff aware of law enforcement information-sharing obligations.

### Nigerian Obligations
- **SCUML Customer Due Diligence (CDD)**: All donors and partners subject to CDD per SCUML AML/CFT guidelines.
- **CAC Entity Verification**: Organizational donors and partners verified as registered entities with the Corporate Affairs Commission.
- **EFCC / ICPC Watch Lists**: Checked as part of PEP and adverse media screening.

## Screening Log Format

The running logs in `logs/` use the template at `templates/screening-log-v1.md`. Each row records:

| Field | Description |
|---|---|
| Screen ID | Unique identifier (e.g., `SCR-2026-0042`) |
| Entity name | Full legal name |
| Entity type | Donor / Vendor / Grantee / Partner |
| Screen date | ISO date (YYYY-MM-DD) |
| Lists checked | e.g., OFAC SDN, CAC, EFCC |
| Tool / source | e.g., OFAC SDN search portal, CAC registry |
| Result | Clear / Hit / False Positive |
| Approved by | Name and title |
| Next re-screen due | ISO date |

## Handling Hits

Any positive match must be recorded in `exceptions/exception-log.md` within 24 hours. The Compliance Officer is notified immediately. No funds are transferred to or received from a screened party with an unresolved hit. Escalation procedures are defined in `policies/us/POL-US-002-ofac-sanctions-compliance.md` and `policies/ng/POL-NG-001-scuml-aml-cft-program.md`.

## Record Retention

Screening records are retained for 5 years from the date of the last transaction with the screened party, consistent with FinCEN BSA requirements and SCUML guidance.
