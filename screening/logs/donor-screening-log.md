# Donor Screening Log

Running log of all OFAC, sanctions, and CDD screens performed on donors. Add a new row for each screen. Individual screening records are filed in `screening/records/donors/`.

| Screen ID | Entity Name | Screen Date | Lists Checked | Tool / Source | Result | Approved By | Next Re-screen Due | Record Link |
|---|---|---|---|---|---|---|---|---|
| SCR-2026-0001 | [Example Donor Name] | 2026-01-10 | OFAC SDN, OFAC Consolidated, SCUML/EFCC | OFAC SDN portal, manual EFCC check | Clear | [Approver Name], Compliance Officer | 2027-01-10 | `screening/records/donors/SCR-2026-0001.md` |

---

## Result Key

- **Clear** — No match found; transaction may proceed.
- **False Positive** — Initial match investigated and confirmed not to be the same entity; documented in `exceptions/exception-log.md`.
- **Hit — Escalated** — Confirmed match; escalated to Compliance Officer; funds on hold. See `exceptions/exception-log.md`.
