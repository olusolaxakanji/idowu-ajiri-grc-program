# Risk Register

This directory tracks the Idowu Ajiri Foundation's identified risks, their assessed likelihood and impact, the controls currently in place, and each risk owner's treatment plan.

## Structure

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

## Risk Rating Scale

### Likelihood

| Score | Label | Description |
|---|---|---|
| 1 | Rare | May occur only in exceptional circumstances |
| 2 | Unlikely | Could occur but not expected |
| 3 | Possible | Might occur at some point |
| 4 | Likely | Will probably occur in most circumstances |
| 5 | Almost certain | Expected to occur in most circumstances |

### Impact

| Score | Label | Description |
|---|---|---|
| 1 | Negligible | No material effect on operations or finances |
| 2 | Minor | Minor disruption; manageable within existing resources |
| 3 | Moderate | Significant disruption; requires management attention |
| 4 | Major | Severe impact on program delivery or finances |
| 5 | Critical | Threatens foundation viability or legal standing |

### Residual Risk Rating

`Residual Rating = Likelihood × Impact`

| Score | Level |
|---|---|
| 1–4 | LOW |
| 5–9 | MEDIUM |
| 10–19 | HIGH |
| 20–25 | CRITICAL |

Risks rated HIGH or CRITICAL are escalated to the board at the next quarterly meeting.

## Risk Entry Format

Each risk entry uses the template at `templates/risk-entry-v1.md`. Key fields: Risk ID, description, category, jurisdiction, inherent rating, current controls, residual rating, treatment plan, risk owner, and next review date.

## Risk Numbering

`RISK-NNN` in sequence across all categories. Never reuse a retired ID.
