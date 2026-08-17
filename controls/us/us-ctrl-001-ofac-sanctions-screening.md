# US-CTRL-001 — OFAC Sanctions Screening

| Field | Value |
|---|---|
| Control ID | US-CTRL-001 |
| Title | OFAC Sanctions Screening |
| Jurisdiction | US |
| Regulatory citation | 31 CFR Part 501; OFAC SDN List; Executive Orders under IEEPA and TWEA |
| Control owner | Compliance Officer |
| Control type | Preventive |
| Testing frequency | Per transaction (new donors/vendors/grantees) + quarterly re-screen of active relationships |
| Last tested | 2026-06-30 |
| Test result | Pass |
| Evidence reference | `evidence/2026/US-CTRL-001/` |
| Status | Active |

## Control Description

Before initiating or accepting any financial transaction with a donor, vendor, or grantee, the responsible staff member screens the entity's full legal name (and known aliases) against:

1. OFAC Specially Designated Nationals (SDN) List
2. OFAC Consolidated Sanctions List
3. Any country-specific programs relevant to Nigeria and the US

Screening is performed via the official OFAC SDN search tool (sanctionssearch.ofac.treas.gov) or an approved compliance platform. Results are recorded in the screening log (`screening/logs/donor-screening-log.md` or equivalent) and an individual screening record is filed in `screening/records/`.

All active relationships are re-screened on a quarterly basis regardless of transaction activity.

## Escalation

Any positive match (non-false-positive) must be escalated to the Compliance Officer within 24 hours. No funds move until the Compliance Officer clears the match or escalates to legal counsel. See `policies/us/POL-US-002-ofac-sanctions-compliance.md` for the full escalation procedure.

## Test Procedure

1. Pull the current active donor/vendor/grantee list from the finance system.
2. Screen each entity against OFAC lists using the approved tool.
3. Document results in the evidence record template.
4. For any new entity onboarded during the test period, confirm a pre-transaction screen was completed.
5. Note any exceptions and confirm they were escalated correctly.
