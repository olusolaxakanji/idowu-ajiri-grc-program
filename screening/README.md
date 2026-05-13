# Screening

Sanctions screening is the most operationally critical function in the foundation's compliance programme. A single undetected transaction with a sanctioned entity can result in OFAC civil monetary penalties, asset freezing, and the kind of reputational damage that ends a nonprofit's ability to fundraise. The screening programme exists to prevent that outcome and to document that prevention in a form regulators can verify.

Every donor, vendor, grantee, and partner is screened before the first transaction. All active relationships are re-screened annually. Every screen is logged. Every hit is escalated within 24 hours. No funds move until an unresolved hit is cleared.

---

## Directory Structure

```
screening/
├── README.md
├── logs/
│   ├── donor-screening-log.md       # Running log of all donor screens
│   ├── vendor-screening-log.md      # Running log of all vendor screens
│   └── grantee-screening-log.md     # Running log of all grantee and partner screens
├── records/
│   ├── donors/                      # Individual screen records by entity name
│   ├── vendors/                     # Individual screen records by vendor name
│   └── grantees/                    # Individual screen records by grantee name
└── exceptions/
    └── exception-log.md             # All hits, false positives, and escalated cases
```

---

## What Is Screened

| Party Type | Screening Trigger | Re-screen Cadence |
|---|---|---|
| Donors | Before first transaction | Annual |
| Vendors | Before contract execution | Annual |
| Grantees and partners | Before first disbursement | Annual |

---

## Screening Requirements by Jurisdiction

### United States

| Requirement | Detail |
|---|---|
| OFAC SDN List | All donors, vendors, and grantees screened before first transaction and annually. |
| OFAC Consolidated Sanctions List | Checked in the same pass as SDN. |
| PEP Screening | Required for any foreign national donor or partner contributing above $10,000. |
| FinCEN 314(a) Awareness | Staff aware of law enforcement information-sharing obligations under FinCEN 314(a). |

### Nigeria

| Requirement | Detail |
|---|---|
| SCUML Customer Due Diligence | All donors and partners subject to CDD per SCUML AML/CFT guidelines for DNFBPs. |
| CAC Entity Verification | Organizational donors and partners verified as registered entities with the Corporate Affairs Commission. |
| EFCC / ICPC Watch Lists | Checked as part of PEP and adverse media screening. |

---

## Screening Log Format

The running logs in `logs/` record every screen. Each row captures:

| Field | Description |
|---|---|
| Screen ID | Unique identifier (e.g., `SCR-2026-0042`) |
| Entity name | Full legal name of the screened party |
| Entity type | Donor / Vendor / Grantee / Partner |
| Screen date | ISO date (YYYY-MM-DD) |
| Lists checked | e.g., OFAC SDN, OFAC Consolidated, CAC, EFCC |
| Tool / source | e.g., OFAC SDN search portal, CAC registry, manual EFCC check |
| Result | Clear / Hit / False Positive |
| Approved by | Name and title of the approving Compliance Officer |
| Next re-screen due | ISO date |

Logs use `templates/screening-record-v1.md`.

---

## Handling Hits

**A hit is any positive match against a sanctions list, watch list, or PEP database.**

1. Stop all pending transactions with the screened party immediately.
2. Record the hit in `exceptions/exception-log.md` within 24 hours.
3. Notify the Compliance Officer immediately.
4. No funds are transferred to or received from the party until the hit is resolved.
5. If the hit is confirmed: follow escalation procedures in [POL-US-002](../policies/us/POL-US-002-ofac-sanctions-compliance.md) (US) or [POL-NG-001](../policies/ng/POL-NG-001-scuml-aml-cft-program.md) (Nigeria).
6. If the hit is a false positive: document the investigation in the exception log with the evidence supporting the false positive determination.

---

## Record Retention

Screening records are retained for **5 years** from the date of the last transaction with the screened party, consistent with FinCEN BSA requirements and SCUML guidance. Do not delete records without Compliance Officer approval.

---

## Related Documentation

| Document | Description |
|---|---|
| [POL-US-002 OFAC Sanctions Compliance](../policies/us/POL-US-002-ofac-sanctions-compliance.md) | Escalation procedures for OFAC hits |
| [POL-NG-001 SCUML AML/CFT Program](../policies/ng/POL-NG-001-scuml-aml-cft-program.md) | Escalation procedures for SCUML hits |
| [Exception Log](exceptions/exception-log.md) | All hits and false positives with full disposition records |
| [US AML/CFT Program](../policies/us/POL-US-001-aml-cft-program.md) | Customer due diligence standards that define screening thresholds |
| [Risk Register](../risk-register/README.md) | RISK-001 tracks OFAC sanctions exposure as a HIGH risk |
