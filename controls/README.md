# Controls

Policies define what the foundation must do. Controls are how the foundation proves it is doing it.

A policy can state that OFAC screening is required before every transaction. That obligation is unverifiable without a control that defines who runs the screen, which lists are checked, what tool is used, what a pass looks like, and what happens when a hit is found. This directory is that layer: the operational bridge between regulatory obligation and audit evidence.

Each control record links to the specific regulation it satisfies, names its owner, defines the testing procedure, specifies the cadence, and records the current status. Together they form the testable layer beneath the policy framework. When IRS, SCUML, or any other regulator asks "how do you demonstrate compliance," these records are part of the answer.

---

## Control Index

| Control ID | Control | Governing Policy | Cadence |
|---|---|---|---|
| [US-CTRL-001](us/us-ctrl-001-ofac-sanctions-screening.md) | OFAC Sanctions Screening | [OFAC Sanctions Compliance Policy](../policies/us/POL-US-002-ofac-sanctions-compliance.md) | Quarterly + at onboarding |
| US-CTRL-002 | IRS Public Disclosure (Form 990) | [Document Retention Policy](../policies/us/POL-US-003-document-retention.md) | Annual |
| US-CTRL-003 | State Charity Registration Renewal | [Document Retention Policy](../policies/us/POL-US-003-document-retention.md) | Annual |
| [NG-CTRL-001](ng/ng-ctrl-001-scuml-registration-renewal.md) | SCUML Registration and Annual Return | [SCUML AML/CFT Program](../policies/ng/POL-NG-001-scuml-aml-cft-program.md) | Annual (due 30 June) |
| NG-CTRL-002 | CAC Annual Return Filing | [CBN NGO Fund Management Policy](../policies/ng/POL-NG-002-cbn-ngo-fund-management.md) | Annual |
| NG-CTRL-003 | CBN NGO Reporting | [CBN NGO Fund Management Policy](../policies/ng/POL-NG-002-cbn-ngo-fund-management.md) | As triggered |
| GL-CTRL-001 | Board Governance and Meeting Quorum | [Code of Conduct](../policies/global/POL-GL-001-code-of-conduct.md) | Quarterly |
| GL-CTRL-002 | Conflict of Interest Annual Disclosure | [Conflict of Interest Policy](../policies/global/POL-GL-003-conflict-of-interest.md) | Annual |

---

## Control Directory Structure

```
controls/
├── README.md
├── control-index.md          # Master list: all controls, owners, status, and last test date
├── us/                       # Controls specific to US obligations
│   ├── us-ctrl-001-ofac-sanctions-screening.md
│   ├── us-ctrl-002-irs-public-disclosure.md
│   └── us-ctrl-003-state-charity-registration.md
└── ng/                       # Controls specific to Nigerian obligations
    ├── ng-ctrl-001-scuml-registration-renewal.md
    ├── ng-ctrl-002-cac-annual-return.md
    └── ng-ctrl-003-cbn-ngo-reporting.md
```

---

## What Each Control Record Specifies

Every control file uses the template at `templates/control-record-v1.md` and records:

| Field | Purpose |
|---|---|
| Control ID | Unique identifier traceable to the master index |
| Regulatory citation | The specific rule, statute, or section the control satisfies |
| Jurisdiction | US, NG, or GLOBAL |
| Control owner | Named individual accountable for operation and testing |
| Control type | Preventive / Detective / Corrective |
| Testing frequency | How often the control must be tested and documented |
| Last tested | Date of most recent test |
| Test result | Pass / Fail / Exception noted |
| Evidence reference | Path or URL to the supporting evidence record |

---

## Control ID Convention

- `US-CTRL-NNN`: US-jurisdiction controls
- `NG-CTRL-NNN`: Nigeria-jurisdiction controls
- `GL-CTRL-NNN`: Global and cross-jurisdiction controls

Never reuse a retired control ID. Mark retired controls `[RETIRED]` in the index with the date of retirement and the reason.

---

## Related Documentation

| Document | Description |
|---|---|
| [Control Index](control-index.md) | Master list of all controls with current status |
| [Evidence](../evidence/README.md) | Evidence records produced by running these controls |
| [Policies](../policies/README.md) | The policies these controls operationalise |
| [Risk Register](../risk-register/README.md) | Risks where control effectiveness is a key residual rating factor |
