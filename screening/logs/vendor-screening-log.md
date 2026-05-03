# Vendor Screening Log

Running log of all OFAC, sanctions, and CDD screens performed on vendors and service providers. Add a new row for each screen. Individual records are filed in `screening/records/vendors/`.

| Screen ID | Entity Name | Screen Date | Lists Checked | Tool / Source | Result | Approved By | Next Re-screen Due | Record Link |
|---|---|---|---|---|---|---|---|---|
| SCR-2026-0002 | [Example Vendor Name] | 2026-01-15 | OFAC SDN, OFAC Consolidated, CAC registry | OFAC SDN portal, CAC public search | Clear | [Approver Name], Finance Lead | 2027-01-15 | `screening/records/vendors/SCR-2026-0002.md` |

---

## Result Key

- **Clear** — No match found; engagement may proceed.
- **False Positive** — Initial match investigated and confirmed not to be the same entity; documented in `exceptions/exception-log.md`.
- **Hit — Escalated** — Confirmed match; escalated to Compliance Officer; engagement on hold. See `exceptions/exception-log.md`.
