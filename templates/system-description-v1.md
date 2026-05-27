# System Description Template
**Document ID:** TPL-SYS-001
**Version:** 1.0
**Classification:** Internal
**Owner:** GRC Analyst
**Review Cycle:** Annual or upon material system change

---

## How to Use This Template

This template produces a SOC 2 System Description as required by AICPA AT-C Section 205 and the Trust Services Criteria. The system description is Section III of the SOC 2 report and is management's responsibility — the auditor attests to whether the description fairly presents the system as designed and implemented.

Complete all sections. Replace bracketed placeholders with organization-specific content. Sections marked [VERIFY] contain assertions that require confirmation against live evidence before the document is finalized.

---

## Section 1: Overview of the Organization

**Organization Name:** [Legal entity name]
**Organization Type:** [e.g., US 501(c)(3) nonprofit / NGO / private company]
**Headquarters:** [City, State, Country]
**Operational Jurisdiction(s):** [List all jurisdictions where services are delivered or data is processed — e.g., United States, Federal Republic of Nigeria]
**Primary Service(s):** [Plain-language description of what the organization does and for whom]

**Service Commitments:** The organization commits to the following with respect to the services covered by this description:

- Availability: [Describe any uptime or access commitments made to users or beneficiaries]
- Confidentiality: [Describe commitments regarding confidential information]
- Data Integrity: [Describe commitments regarding accurate and complete processing]
- Security: [Describe commitments to protect information against unauthorized access]

---

## Section 2: Principal Service Commitments and System Requirements

### 2.1 Service Commitments

| Commitment Area | Commitment Statement | Applicable Trust Services Category |
|----------------|---------------------|-------------------------------------|
| Security | The organization protects information assets against unauthorized access, use, disclosure, modification, and destruction | Security (CC) |
| Availability | [State availability commitment if applicable — e.g., "Systems supporting programme delivery are available during defined operating hours"] | Availability (A1) |
| Confidentiality | [State confidentiality commitment if applicable — e.g., "Donor and beneficiary information is treated as confidential and disclosed only as required by law or with explicit consent"] | Confidentiality (C1) |
| Privacy | [State privacy commitment if applicable — e.g., "Personal data of beneficiaries is collected, used, retained, and disclosed in accordance with the organization's Privacy Notice"] | Privacy (P series) |

### 2.2 System Requirements

The following requirements must be met for the system to deliver on its commitments:

- **Regulatory:** [List applicable regulatory requirements — e.g., IRS 501(c)(3) annual reporting, NDPR (Nigerian Data Protection Regulation), SCUML AML/CFT registration, OFAC sanctions screening]
- **Contractual:** [List relevant contractual obligations — e.g., donor grant conditions, programme partner agreements]
- **Operational:** [List operational requirements — e.g., availability of volunteer staff, functioning donor management system]

---

## Section 3: Components of the System

### 3.1 Infrastructure

| Component | Description | Location | Owner |
|-----------|-------------|----------|-------|
| [e.g., Donor Management System] | [e.g., Cloud-hosted platform for recording donor information and grant disbursements] | [e.g., AWS us-east-1] | [e.g., Technology Lead] |
| [e.g., Email System] | [e.g., Google Workspace for organizational communications] | [Cloud] | [e.g., Operations Lead] |
| [e.g., Document Repository] | [e.g., Google Drive for policy and evidence storage] | [Cloud] | [e.g., GRC Analyst] |

### 3.2 Software

| Application | Purpose | Hosting | Critical? |
|-------------|---------|---------|-----------|
| [Application name] | [Brief description] | [Cloud / On-premise] | [Yes / No] |

### 3.3 People

| Role | Responsibilities Relevant to the System | Access Level |
|------|-----------------------------------------|-------------|
| Executive Director | Approves policies; accepts residual risks above defined appetite | Administrative |
| GRC Analyst | Maintains risk register, controls, policies, and audit evidence | Administrative |
| Operations Lead | Manages day-to-day system access and donor relationships | Standard |
| [Other roles as applicable] | | |

### 3.4 Processes

Key processes that constitute the system and are within the scope of this description:

| Process | Frequency | Owner | Evidence Produced |
|---------|-----------|-------|------------------|
| Access provisioning and deprovisioning | Per personnel change | GRC Analyst / Operations Lead | JML records |
| Quarterly access review | Quarterly | GRC Analyst | Access review report |
| Risk register review | Quarterly | GRC Analyst | Risk committee minutes |
| Policy review and approval | Annual | GRC Analyst + Executive Director | Approved policy version |
| Incident detection and response | As triggered | GRC Analyst | Incident log |
| Donor data handling | Continuous | Operations Lead | Transaction records |
| Security awareness training | Annual | GRC Analyst | Training completion records |

### 3.5 Data

| Data Category | Classification | Storage Location | Retention Period | Personal Data? |
|---------------|---------------|-----------------|-----------------|---------------|
| Donor information (name, contact, giving history) | Confidential | [System name] | [Retention period] | Yes |
| Beneficiary programme records | Confidential | [System name] | [Retention period] | Yes |
| Financial records | Confidential | [System name] | 7 years | Partially |
| Policy and governance documents | Internal | Document Repository | Current + 2 prior versions | No |
| Audit evidence | Internal | Document Repository | 7 years | No |

---

## Section 4: Boundaries of the System

### 4.1 In Scope

The following are within the boundary of this system description:

- [List systems, processes, and data in scope — e.g., donor management system, GRC programme, volunteer access management]
- [Include all locations and entities where in-scope data is processed]

### 4.2 Out of Scope

The following are explicitly outside the boundary of this system description:

- [e.g., Third-party payment processing (handled by [vendor]; covered by their own SOC 2 report)]
- [e.g., Personal devices used by volunteers (not managed by the organization)]

### 4.3 Subservice Organizations

The following subservice organizations perform functions relevant to this system:

| Subservice Organization | Function | Carve-Out or Inclusive? | SOC Report Available? |
|------------------------|----------|------------------------|----------------------|
| [e.g., Google LLC] | [e.g., Cloud infrastructure for document storage and email] | Carve-out | [Yes — SOC 2 Type II available] |
| [Other vendors] | | | |

*Carve-out method: the subservice organization's controls are excluded from the scope of this description. Inclusive method: the subservice organization's controls are included.*

---

## Section 5: Relevant Aspects of the Control Environment

### 5.1 Governance and Oversight

[Describe the governance structure: board composition, oversight mechanisms, how the board exercises oversight of management and the GRC programme. Reference the relevant policies.]

Example: The organization is governed by a Board of Directors that meets [quarterly / semi-annually]. The Board reviews and approves the annual risk register summary and is briefed on material incidents and compliance obligations. Day-to-day GRC oversight is the responsibility of the GRC Analyst, who reports to the Executive Director.

### 5.2 Risk Assessment Process

[Describe how the organization identifies, evaluates, and responds to risks. Reference the Risk Management Policy.]

Example: The organization maintains a formal risk register updated quarterly. Risks are scored using a 5x5 likelihood-impact matrix. Risks rated HIGH or CRITICAL require documented treatment plans with named owners and target dates. Residual risks above the defined risk appetite require Executive Director sign-off.

### 5.3 Control Activities

[Describe the control activities in place. Reference the policy library.]

Example: The organization maintains [number] policies covering [list key areas: access control, incident response, data classification, acceptable use, TPRM, BC/DR]. All policies are reviewed annually, version-controlled, and approved by the Executive Director.

### 5.4 Communication

[Describe how security and compliance requirements are communicated internally and externally.]

Example: All staff and volunteers with system access receive annual security awareness training and acknowledge the Acceptable Use Policy. External communications regarding data handling are governed by the published Privacy Notice.

### 5.5 Monitoring

[Describe the monitoring activities that assess whether controls are operating effectively.]

Example: The GRC Analyst conducts quarterly control effectiveness reviews. Findings are documented in the risk register. Material control failures are escalated to the Executive Director within [defined timeframe].

---

## Section 6: Complementary User Entity Controls

The following controls must be implemented by user entities (e.g., programme partners, major donors with system access) for the overall system to meet its commitments:

| Control | Rationale |
|---------|-----------|
| User entities must manage their own access credentials and report suspected credential compromise promptly | The organization cannot prevent unauthorized access resulting from compromised credentials held by user entities |
| User entities must notify the organization of changes in authorized personnel with system access | Timely notification enables the organization to deprovision access as part of the JML process |
| [Add additional CUECs as applicable] | |

---

## Section 7: Changes to the System During the Period

*Complete this section for Type II reports covering a defined audit period.*

| Date | Change Description | Impact on Controls |
|------|-------------------|-------------------|
| [Date] | [Describe material system or process change] | [Describe any impact on controls or evidence collection] |

*If no material changes occurred during the period, state: "No material changes to the system occurred during the period covered by this description."*

---

## Document Control

| Attribute | Value |
|-----------|-------|
| Template ID | TPL-SYS-001 |
| Version | 1.0 |
| Status | Active |
| Author | GRC Analyst |
| Approved By | [Executive Director name] |
| Effective Date | [Date] |
| Next Review | [Date + 1 year] |

---

*TPL-SYS-001 v1.0 | Idowu Ajiri Foundation GRC Programme | System Description Template*
