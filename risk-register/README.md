# Risk Register

The risk register gives the board and the Compliance Officer a current, documented picture of the foundation's risk posture. Without it, risk decisions are informal, treatment responsibilities are unclear, and there is no baseline to measure improvement against.

The register is the document that answers: what risks does the foundation face, how severe are they with and without current controls, who owns each risk, and what is being done about it?

---

## Current Posture

10 active risks across four categories. Two are currently rated HIGH and receive board attention at each quarterly meeting.

| Risk ID | Description | Level | Jurisdiction | Owner |
|---|---|---|---|---|
| RISK-001 | Foundation receives funds from OFAC-sanctioned entity due to incomplete screening | HIGH | US | Compliance Officer |
| RISK-002 | Late or missed IRS Form 990 filing results in penalty or automatic revocation of 501(c)(3) status | MEDIUM | US | Finance Lead |
| RISK-003 | SCUML annual return filed late, triggering regulatory sanction or deregistration | HIGH | NG | Compliance Officer |
| RISK-004 | Misappropriation of program funds by staff or implementing partner | MEDIUM | GLOBAL | Finance Lead |
| RISK-005 | Adverse foreign exchange movement reduces NGN-denominated program budget | MEDIUM | NG | Finance Lead |
| RISK-006 | Key-person dependency: loss of Compliance Officer creates regulatory blind spots | MEDIUM | GLOBAL | Executive Director |
| RISK-007 | Data breach exposes donor PII, triggering NDPR or state-law notification obligations | MEDIUM | GLOBAL | Compliance Officer |
| RISK-008 | Negative media coverage of a grantee partner damages foundation reputation | MEDIUM | GLOBAL | Executive Director |
| RISK-009 | Failure to renew state charity registration results in unlawful solicitation exposure | LOW | US | Compliance Officer |
| RISK-010 | CAC annual return filing missed, leading to penalty or loss of legal status | MEDIUM | NG | Finance Lead |

**RISK-001 and RISK-003 require board attention every quarter.** RISK-001 carries inherent impact of 5 (Critical): an OFAC violation can result in civil monetary penalties, asset freezing, and reputational damage that threatens the foundation's operating capacity. RISK-003 carries an inherent impact of 5: SCUML deregistration would suspend the foundation's legal authority to operate in Nigeria.

---

## Directory Structure

```
risk-register/
├── README.md
├── master-risk-register.md    # Consolidated view of all active risks
├── archive/                   # Closed or retired risk entries
├── operational/               # Program delivery and staffing risks
├── financial/                 # Fraud, misappropriation, FX, and funding risks
├── compliance/                # Regulatory and legal exposure risks
└── reputational/              # Brand, media, and partner-relationship risks
```

---

## Rating Scale

### Likelihood

| Score | Label | Meaning |
|---|---|---|
| 1 | Rare | May occur only in exceptional circumstances |
| 2 | Unlikely | Could occur but not expected |
| 3 | Possible | Might occur at some point |
| 4 | Likely | Will probably occur in most circumstances |
| 5 | Almost certain | Expected to occur in most circumstances |

### Impact

| Score | Label | Meaning |
|---|---|---|
| 1 | Negligible | No material effect on operations or finances |
| 2 | Minor | Minor disruption, manageable within existing resources |
| 3 | Moderate | Significant disruption, requires management attention |
| 4 | Major | Severe impact on program delivery or finances |
| 5 | Critical | Threatens foundation viability or legal standing |

### Rating Levels

`Residual Rating = Likelihood × Impact`

| Score | Level | Board escalation |
|---|---|---|
| 1-4 | LOW | No |
| 5-9 | MEDIUM | No |
| 10-19 | HIGH | Yes: quarterly board report |
| 20-25 | CRITICAL | Yes: immediate notification |

---

## Risk Entry Format

Each risk entry uses `templates/risk-entry-v1.md`. Required fields: Risk ID, description, category, jurisdiction, inherent rating (likelihood × impact before controls), current controls, residual rating (likelihood × impact after controls), treatment plan, risk owner, and next review date.

Documenting both the inherent and residual rating is what allows the register to show what controls are doing. The gap between the two is the demonstrated value of each control. A register that shows only one rating cannot answer "what would happen if these controls failed."

---

## Risk Numbering

`RISK-NNN` in sequence across all categories. Never reuse a retired ID. Close retired risks in the master register with a close date and reason, then move the entry record to `archive/`.

---

## Related Documentation

| Document | Description |
|---|---|
| [Master Risk Register](master-risk-register.md) | Consolidated view of all 10 active risks |
| [Controls](../controls/README.md) | Controls that reduce inherent ratings to residual ratings |
| [Reports](../reports/README.md) | Board reports where HIGH and CRITICAL risks are escalated quarterly |
| [Policies](../policies/README.md) | Policies that govern the areas each risk falls within |
