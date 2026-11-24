# MediCore Health Technologies
# Assumptions and Limitations Register

## 1. Document Information

| Field | Description |
|---|---|
| Organization | MediCore Health Technologies (Fictional) |
| Assessment Name | Enterprise Cybersecurity, Cloud Security, and AI Governance Assessment |
| Document Type | Assumptions and Limitations Register |
| Assessment Classification | Simulated Educational Assessment |
| Assessment Owner | Cybersecurity Assessment Analyst |
| Version | 1.0 |
| Status | Draft |

---

## 2. Purpose

The purpose of this document is to identify the assumptions, known scenario details, outstanding information gaps, and limitations associated with the MediCore cybersecurity assessment.

Documenting these items helps ensure that assessment conclusions are transparent, appropriately qualified, and supported by available evidence.

This register will be maintained throughout the assessment as additional information is obtained and assumptions are validated, revised, or rejected.

## 3. Known Scenario Details

The following details have been established as part of the fictional MediCore business scenario.

| ID | Known Scenario Detail | Assessment Relevance |
|---|---|---|
| KD-01 | MediCore operates a healthcare technology SaaS platform. | Establishes the business and technology environment being assessed. |
| KD-02 | The platform uses AWS-hosted infrastructure. | Requires evaluation of cloud security and shared responsibility. |
| KD-03 | The environment includes managed databases and cloud storage. | Requires evaluation of data protection, access restrictions, and encryption. |
| KD-04 | MediCore integrates an external hosted LLM API. | Introduces third-party AI and information disclosure risks. |
| KD-05 | The platform serves healthcare organizations and healthcare professionals. | Establishes customer, user, and potential sensitive-data considerations. |
| KD-06 | The scenario includes concerns involving MFA, privileged access, and account management. | Establishes areas requiring IAM evidence and control testing. |
| KD-07 | The scenario includes concerns involving cloud logging and monitoring. | Establishes the need to review audit logging and security visibility. |
| KD-08 | The scenario includes concerns involving backup protection and ransomware recovery. | Establishes the need to review resilience and incident recovery. |
| KD-09 | The scenario includes an external AI provider with potentially incomplete or outdated assurance documentation. | Establishes the need for third-party due diligence. |
| KD-10 | MediCore is pursuing a prospective hospital contract with a security review requirement. | Establishes a potential business impact associated with security assurance. |

**Important:** These are details of the educational scenario, not independently verified facts about a real organization.

## 4. Assessment Assumptions

The following assumptions will be used provisionally to support assessment planning.

| ID | Assumption | Reason | Validation Method | Status |
|---|---|---|---|---|
| A-01 | MediCore's AWS environment supports production business operations. | The fictional platform depends on AWS-hosted services. | Review simulated architecture and service inventory. | Pending |
| A-02 | MediCore may process or maintain ePHI on behalf of healthcare customers. | The platform operates in the healthcare technology sector. | Review data flows, customer relationships, contracts, and applicable HIPAA definitions. | Pending |
| A-03 | Employees and customer users require authenticated access to the SaaS platform. | The platform supports organizational and professional users. | Review identity architecture and account-management documentation. | Pending |
| A-04 | Administrative accounts have elevated access to cloud or application resources. | Cloud infrastructure requires administrative management. | Review simulated IAM roles, permissions, and access exports. | Pending |
| A-05 | The external LLM provider may receive information submitted through MediCore's AI integration. | The platform uses an external hosted AI service. | Review integration architecture, API configuration, and data-flow documentation. | Pending |
| A-06 | Third-party providers may introduce operational, privacy, or security dependencies. | MediCore relies on external technology services. | Review vendor inventory, contracts, and assurance documentation. | Pending |
| A-07 | MediCore requires backup and recovery capabilities to maintain service availability. | The platform supports business-critical customer operations. | Review simulated backup policies and recovery procedures. | Pending |
| A-08 | Security policies and procedures should exist for relevant operational activities. | The assessment evaluates security governance and control maturity. | Request and review simulated policy documentation. | Pending |

Assumptions must be validated where possible before they are used to support final assessment conclusions.

## 5. Outstanding Information and Knowledge Gaps

The following information has not yet been established and requires further investigation.

| ID | Information Gap | Why It Matters | Evidence Required |
|---|---|---|---|
| U-01 | Whether MediCore qualifies as a HIPAA business associate for specific customer activities. | Determines applicable HIPAA obligations and contractual requirements. | Customer agreements, BAAs where applicable, and data-processing descriptions. |
| U-02 | Whether MFA is enforced for all privileged accounts. | Determines exposure to credential compromise. | IAM configuration exports and authentication policies. |
| U-03 | Whether administrative access is restricted using least privilege. | Excessive permissions can increase the impact of unauthorized access. | IAM role definitions, permission policies, and access reviews. |
| U-04 | Whether cloud storage prevents unauthorized public access. | Misconfigured storage may expose sensitive information. | Simulated storage configuration and public access settings. |
| U-05 | Whether CloudTrail logs are centrally collected and adequately retained. | Incomplete logging may limit incident detection and investigation. | CloudTrail configuration, logging architecture, and retention settings. |
| U-06 | Whether encryption and key-management controls are appropriately configured. | Sensitive information requires appropriate protection at rest and in transit. | Encryption configurations and key-management documentation. |
| U-07 | Whether backups are isolated from production credentials and environments. | Compromised production access could affect recovery capabilities. | Backup architecture, access permissions, and recovery procedures. |
| U-08 | Whether backup restoration has been tested successfully. | Backups alone do not prove recoverability. | Recovery test records and documented results. |
| U-09 | Whether the AI provider retains submitted information or uses it for model training. | Data handling may create privacy, confidentiality, and contractual risks. | Vendor terms, data-processing agreements, and technical documentation. |
| U-10 | Whether all relevant AI subprocessors have been identified and reviewed. | Additional providers may introduce undisclosed dependencies. | Vendor subprocessor list and due diligence records. |
| U-11 | Whether vendor security assurance reports cover the services used by MediCore. | An assurance report may not cover the relevant service or period. | SOC 2 report summary, scope, period, exceptions, and complementary controls. |
| U-12 | Whether incident notification obligations are defined in vendor agreements. | Delayed notification may affect incident response and contractual obligations. | Vendor contracts and incident notification provisions. |

These information gaps will guide evidence collection and control testing.

## 6. Assessment Limitations

The following limitations apply to this project:

### 6.1 Simulated Environment

MediCore is a fictional organization. All business details, technology configurations, security scenarios, and assessment evidence are simulated.

No conclusions should be interpreted as findings about an actual company.

### 6.2 No Production System Access

The assessment does not involve accessing or testing actual production infrastructure, databases, applications, or user accounts.

### 6.3 No Live Penetration Testing

The assessment does not include exploitation, unauthorized access attempts, destructive testing, or live vulnerability scanning against real systems.

### 6.4 Limited Evidence Availability

Assessment conclusions will depend on the simulated evidence created or provided for this project. Missing evidence may prevent confirmation of whether a control is implemented or operating effectively.

### 6.5 Third-Party Assessment Constraints

AWS and the external AI provider will not be independently audited. Their security responsibilities and documentation will be considered using available simulated evidence and publicly documented responsibility models where appropriate.

### 6.6 Regulatory Assessment Constraints

The project includes educational mapping to HIPAA and other cybersecurity frameworks. It does not establish legal compliance, provide legal advice, or constitute a formal regulatory audit.

### 6.7 Technical Validation Constraints

Technical findings will be based on the configurations, logs, architecture diagrams, and other simulated artifacts available within the project.

The absence of a simulated artifact does not establish that a real-world control is missing.

## 7. Risk of Incorrect Assumptions

Unvalidated assumptions can lead to inaccurate risk assessments and inappropriate remediation recommendations.

Examples include:

| Incorrect Assumption | Potential Consequence | Appropriate Analyst Action |
|---|---|---|
| Assuming all healthcare data is ePHI. | Incorrect regulatory classification. | Validate the information and applicable HIPAA relationships. |
| Assuming AWS secures every customer configuration. | Overlooking MediCore's cloud security responsibilities. | Apply the AWS Shared Responsibility Model. |
| Assuming a SOC 2 report proves a vendor is secure. | Overlooking report limitations and control exceptions. | Review scope, testing period, exceptions, and complementary controls. |
| Assuming backups guarantee recovery. | Overestimating ransomware resilience. | Review restoration testing and backup isolation. |
| Assuming an AI provider does not retain customer data. | Underestimating sensitive information exposure. | Review contractual terms and technical data-handling practices. |
| Assuming missing documentation proves a control is ineffective. | Creating unsupported findings. | Record the evidence gap and seek additional validation. |

## 8. Assumption and Information Gap Management

The following process will be used throughout the assessment:

1. Record each assumption or information gap in this register.
2. Identify the evidence required to validate it.
3. Request or create the relevant simulated evidence.
4. Evaluate the evidence and document the results.
5. Update the status to validated, rejected, or unresolved.
6. Record any resulting impact on the risk assessment.
7. Carry unresolved items into the final assessment report as limitations or recommendations, as appropriate.

### Status Definitions

| Status | Meaning |
|---|---|
| Pending | Validation has not yet been completed. |
| Validated | Available evidence supports the assumption. |
| Rejected | Evidence contradicts the assumption. |
| Unresolved | Available evidence is insufficient to reach a conclusion. |
| Not Applicable | The assumption or information gap does not apply to the assessed environment. |

## 9. Relationship to Other Assessment Documents

This register supports the following project deliverables:

- `business-profile.md` — Establishes the fictional company's business environment.
- `assessment-scope.md` — Defines assessment boundaries.
- `stakeholder-register.xlsx` — Identifies relevant stakeholders and responsibilities.
- `evidence-request-list.xlsx` — Tracks evidence needed to validate assumptions.
- `risk-register.xlsx` — Records and prioritizes identified risks.
- `control-evidence-log.xlsx` — Tracks evidence supporting control assessments.

Information discovered during subsequent assessment activities should be reflected in this register when it changes an existing assumption or resolves an outstanding information gap.

## 10. Analyst Conclusion

The assumptions and limitations documented in this register establish the boundaries of what can reasonably be concluded during the MediCore cybersecurity assessment.

The assessment will use an evidence-based approach to validate assumptions, investigate information gaps, and distinguish confirmed observations from unverified scenarios.

Unresolved assumptions and evidence limitations will be transparently documented to prevent unsupported conclusions and ensure that risk ratings and recommendations are appropriately justified.

---

**Document Disclaimer:** MediCore Health Technologies is a fictional organization created for educational and portfolio purposes. All company information, assumptions, security scenarios, evidence, and findings are simulated. This document does not represent an actual cybersecurity assessment, penetration test, HIPAA audit, compliance certification, or legal opinion.