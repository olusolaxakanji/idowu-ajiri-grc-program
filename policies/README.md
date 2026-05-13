# Policies

Eleven governance policies across three tiers. Each one exists because a specific regulatory obligation requires it: the global tier covers conduct standards that apply in both jurisdictions, the US tier covers IRS, OFAC, and FinCEN obligations, and the Nigerian tier covers SCUML, CBN, and NDPR obligations.

The three-tier structure is not an aesthetic choice. A single-jurisdiction policy document cannot govern both US and Nigerian operations simultaneously. OFAC and SCUML have different screening requirements. FinCEN and NDPR have different data handling rules. CBN fund management requirements have no US equivalent. Each tier exists because the regulatory regime it covers is distinct.

---

## Policy Directory

```
policies/
├── README.md
├── global/                          # Policies applying in both jurisdictions
│   ├── POL-GL-001-code-of-conduct.md
│   ├── POL-GL-002-anti-bribery-corruption.md
│   ├── POL-GL-003-conflict-of-interest.md
│   ├── POL-GL-004-whistleblower-protection.md
│   └── POL-GL-005-data-protection-privacy.md
├── us/                              # US-specific policies
│   ├── POL-US-001-aml-cft-program.md
│   ├── POL-US-002-ofac-sanctions-compliance.md
│   ├── POL-US-003-document-retention.md
│   └── conflict-of-interest-disclosure-memo-akanji.md
├── ng/                              # Nigeria-specific policies
│   ├── POL-NG-001-scuml-aml-cft-program.md
│   ├── POL-NG-002-cbn-ngo-fund-management.md
│   └── POL-NG-003-ndpr-data-handling.md
└── archive/                         # Superseded versions (never deleted)
```

---

## Policy Index

### Global (Cross-Jurisdiction)

| Policy | What regulatory obligation it addresses |
|---|---|
| [POL-GL-001 Code of Conduct](global/POL-GL-001-code-of-conduct.md) | Baseline conduct standards anchoring the disciplinary framework referenced in all other policies. Required by IRS governance best practices for 501(c)(3) organizations and consistent with CAC governance expectations. |
| [POL-GL-002 Anti-Bribery and Corruption](global/POL-GL-002-anti-bribery-corruption.md) | FCPA applies to the foundation's international operations. Nigerian anti-corruption law (EFCC Act, ICPC Act) applies to Nigerian operations. This policy defines prohibited conduct, gift and hospitality limits, and the reporting path for suspected violations under both regimes. |
| [POL-GL-003 Conflict of Interest](global/POL-GL-003-conflict-of-interest.md) | IRS Form 990 Part VI asks whether the organization has a written conflict of interest policy and whether it is followed. This policy defines the disclosure requirement, recusal procedures, and documentation standards that answer yes to both questions. |
| [POL-GL-004 Whistleblower Protection](global/POL-GL-004-whistleblower-protection.md) | IRS Form 990 Part VI asks whether the organization has a written whistleblower policy. This policy establishes the protected reporting channel and anti-retaliation provisions. |
| [POL-GL-005 Data Protection and Privacy](global/POL-GL-005-data-protection-privacy.md) | Donor PII collected in Nigeria falls under NDPR. The same records transferred to the US create exposure under applicable US state privacy laws. This policy defines the lawful basis, cross-border transfer conditions, data subject rights, and retention periods for both regimes. |

### United States

| Policy | What regulatory obligation it addresses |
|---|---|
| [POL-US-001 AML/CFT Program](us/POL-US-001-aml-cft-program.md) | FinCEN 31 CFR Part 1010 requires nonprofit organizations involved in cross-border fund transfers to maintain a risk-based AML/CFT programme. This policy establishes that programme: risk assessment methodology, customer due diligence standards, and SAR filing obligations. |
| [POL-US-002 OFAC Sanctions Compliance](us/POL-US-002-ofac-sanctions-compliance.md) | OFAC prohibits US persons from transacting with sanctioned parties. A confirmed hit without a documented screening process exposes the foundation to civil monetary penalties. This policy sets the screening cadence, tool requirements, escalation path, and fund-blocking procedures. |
| [POL-US-003 Document Retention](us/POL-US-003-document-retention.md) | IRS audits and OFAC investigations both require the ability to produce records on demand. This policy defines retention periods by document type, secure disposal procedures, and litigation hold protocols consistent with IRS guidance for 501(c)(3) organizations. |

### Nigeria

| Policy | What regulatory obligation it addresses |
|---|---|
| [POL-NG-001 SCUML AML/CFT Program](ng/POL-NG-001-scuml-aml-cft-program.md) | SCUML classifies Nigerian nonprofits as Designated Non-Financial Businesses and Professions. That classification triggers formal registration, suspicious transaction reporting, and annual return obligations. This policy addresses each obligation specifically. |
| [POL-NG-002 CBN NGO Fund Management](ng/POL-NG-002-cbn-ngo-fund-management.md) | The CBN circular on NGO fund management creates bank account designation requirements and cross-border fund transfer controls for foreign-linked nonprofits. This policy operationalises those requirements for the foundation's US-Nigeria fund flows. |
| [POL-NG-003 NDPR Data Handling](ng/POL-NG-003-ndpr-data-handling.md) | Donor and beneficiary records collected in Nigeria are governed by the Nigeria Data Protection Act 2023. This policy defines the lawful basis, data subject rights, retention schedules, and the specific obligations triggered when records are transferred to the US entity. |

---

## Policy Document Standard

Every policy uses `templates/policy-v1.md` and must include:

| Field | Required content |
|---|---|
| Policy ID | e.g., `POL-GL-001` |
| Title | Plain-language name |
| Jurisdiction | GLOBAL / US / NG |
| Effective date | Date the board approved this version |
| Next review date | No more than 12 months from effective date |
| Approving authority | Board / Executive Director / Compliance Officer |
| Regulatory basis | Specific laws or regulations this policy addresses |
| Policy owner | Named individual responsible for maintenance |
| Version | Semantic version: `1.0`, `1.1`, `2.0` |

---

## Policy Lifecycle

1. **Draft:** Policy owner drafts using the template.
2. **Review:** Compliance Officer and relevant jurisdiction lead review.
3. **Approval:** Approving authority signs off, recorded in the document header.
4. **Publish:** Merged to `main` and communicated to all staff.
5. **Review:** Triggered annually or by a material regulatory change.
6. **Archive:** Superseded versions moved to `archive/` with a pointer to the replacement. Old versions are never deleted.

---

## Policy Numbering

- `POL-GL-NNN`: Global policies
- `POL-US-NNN`: US-specific policies
- `POL-NG-NNN`: Nigeria-specific policies

---

## Related Documentation

| Document | Description |
|---|---|
| [Controls](../controls/README.md) | Controls that operationalise these policies |
| [Risk Register](../risk-register/README.md) | Risks that these policies are designed to reduce |
| [Reports](../reports/README.md) | Board reports that summarise policy compliance status |
