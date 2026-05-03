# Policies

This directory contains all approved organizational policies of the Idowu Ajiri Foundation. Policies define the rules, standards, and expectations that govern how the foundation operates in both jurisdictions.

## Structure

```
policies/
├── README.md
├── global/                          # Policies that apply in both jurisdictions
│   ├── POL-GL-001-code-of-conduct.md
│   ├── POL-GL-002-anti-bribery-corruption.md
│   ├── POL-GL-003-conflict-of-interest.md
│   ├── POL-GL-004-whistleblower-protection.md
│   └── POL-GL-005-data-protection-privacy.md
├── us/                              # Policies specific to US operations
│   ├── POL-US-001-aml-cft-program.md
│   ├── POL-US-002-ofac-sanctions-compliance.md
│   ├── POL-US-003-document-retention.md
│   └── POL-US-004-990-public-disclosure.md
├── ng/                              # Policies specific to Nigerian operations
│   ├── POL-NG-001-scuml-aml-cft-program.md
│   ├── POL-NG-002-cbn-ngo-fund-management.md
│   └── POL-NG-003-ndpr-data-handling.md
└── archive/                         # Superseded policies (never deleted)
```

## Policy Document Standard

Every policy uses the template at `templates/policy-v1.md` and must include:

| Field | Description |
|---|---|
| Policy ID | e.g., `POL-GL-001` |
| Title | Plain-language name |
| Jurisdiction | GLOBAL / US / NG |
| Effective date | Date board approved this version |
| Next review date | No more than 12 months from effective date |
| Approving authority | Board / Executive Director / Compliance Officer |
| Regulatory basis | Specific laws or regulations this policy addresses |
| Policy owner | Named individual responsible for maintenance |
| Version | Semantic version (e.g., `1.0`, `1.1`, `2.0`) |

## Policy Numbering

- `POL-GL-NNN` — Global policies
- `POL-US-NNN` — US-specific policies
- `POL-NG-NNN` — Nigeria-specific policies

## Lifecycle

1. **Draft** — Policy owner drafts using the template.
2. **Review** — Compliance Officer and relevant jurisdiction lead review.
3. **Approval** — Approving authority signs off (recorded in the document header).
4. **Publish** — Merged to `main`; communicated to all staff.
5. **Review** — Triggered annually or by a material regulatory change.
6. **Archive** — Superseded versions moved to `archive/` with a pointer to the replacement.
