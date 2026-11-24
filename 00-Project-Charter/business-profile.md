# MediCore Health Technologies
## Business Profile & Discovery Assessment

**Document Type:** Business Discovery  
**Project:** Enterprise Healthcare AI Security & Governance Assessment  
**Prepared By:** IT Risk & Cybersecurity Analyst  
**Assessment Status:** Initial Discovery  
**Classification:** Simulated Portfolio Project  
**Version:** 1.0

---

## 1. Business Overview

MediCore Health Technologies is a fictional healthcare technology company that provides cloud-based Software-as-a-Service (SaaS) solutions to healthcare organizations.

The company's platform supports healthcare-related workflows and information management. Its technology environment is hosted on Amazon Web Services (AWS) and incorporates an external generative artificial intelligence (AI) provider to support selected platform capabilities.

MediCore's business depends on the availability, confidentiality, and integrity of its technology platform and the sensitive information it processes.

The purpose of this business discovery assessment is to understand MediCore's operations, technology dependencies, information assets, stakeholders, and potential business risks before conducting a detailed cybersecurity assessment.

## 2. Company Profile

The following information represents the simulated business environment established for this assessment.

| Business Attribute | Description |
|---|---|
| Organization | MediCore Health Technologies |
| Industry | Healthcare Technology |
| Employees | 180 |
| Healthcare Customers | 35 |
| Healthcare Professional Users | 8,000 |
| Annual Revenue | $32 million |
| Business Model | Business-to-Business SaaS |
| Cloud Provider | Amazon Web Services |
| AI Integration | External generative AI model provider |
| Data Classification | Includes sensitive healthcare information and potentially ePHI |
| Business Priority | Enterprise customer expansion |

MediCore is preparing for a potential $4 million hospital enterprise contract. The prospective customer requires a security assessment within 30 days before proceeding with the agreement.

This creates a business incentive to evaluate security controls, identify deficiencies, and demonstrate the organization's ability to manage cybersecurity and third-party risks.

## 3. Products, Services & Business Operations

MediCore provides healthcare organizations with access to a cloud-hosted software platform.

Its business operations depend on:

- Hosting and maintaining its SaaS application.
- Managing healthcare customer accounts and user access.
- Processing and maintaining healthcare-related information.
- Operating cloud infrastructure and databases.
- Integrating external technology providers.
- Maintaining platform availability and reliability.
- Protecting customer information and fulfilling contractual security obligations.

The company's technology platform is a critical business asset. Disruptions, unauthorized access, or failures affecting the platform could directly impact customer operations and revenue.

## 4. Customers & Stakeholders

MediCore operates a business-to-business model.

Its primary customers are healthcare organizations, including hospitals, clinics, and other healthcare providers.

The platform's users include healthcare professionals who access the software to perform authorized business and healthcare-related activities.

The relevant stakeholder groups include:

| Stakeholder | Relationship to MediCore |
|---|---|
| Healthcare Organizations | Contracting customers |
| Healthcare Professionals | Platform users |
| Patients | Individuals whose information may be processed |
| AWS | Cloud infrastructure provider |
| External AI Provider | Third-party AI service provider |
| Software Vendors | Supporting technology providers |
| Employees | Internal platform and business users |
| Regulators and Contractual Partners | External compliance and assurance stakeholders |

Understanding these relationships is necessary to identify who owns information, who accesses it, who processes it, and who is responsible for protecting it.

## 5. Information Assets & Data Sensitivity

MediCore may collect, process, store, or transmit several categories of information.

| Information Category | Examples | Potential Sensitivity |
|---|---|---|
| Patient Information | Names and identifying details | High |
| Healthcare Information | Diagnoses and treatment-related information | High |
| Healthcare Records | Medical record information | High |
| User Information | Employee and healthcare professional accounts | Moderate to High |
| Authentication Data | Credentials and access tokens | High |
| Business Information | Contracts and customer records | Moderate to High |
| System Information | Logs, configurations, and security events | Moderate to High |
| Financial Information | Billing and payment-related records, if processed | High |

Some information handled by MediCore may qualify as electronic protected health information (ePHI) under HIPAA.

ePHI generally refers to individually identifiable health information that is created, received, maintained, or transmitted electronically by a HIPAA covered entity or business associate, subject to applicable definitions and exclusions.

The confidentiality, integrity, and availability of this information must be considered throughout the assessment.

The analyst must confirm which information categories are actually processed, where they are stored, how they are transmitted, and which parties can access them.

## 6. Regulatory & Business Considerations

Because MediCore provides services to healthcare organizations and may handle ePHI on their behalf, its contractual and regulatory responsibilities require further investigation.

If MediCore meets the definition of a HIPAA business associate, applicable HIPAA requirements and contractual obligations may apply.

The assessment should investigate:

- Whether MediCore acts as a business associate.
- Whether business associate agreements (BAAs) are in place where required.
- How ePHI is protected.
- Whether administrative, physical, and technical safeguards are appropriately implemented.
- Whether third-party vendors receive or maintain ePHI.
- Whether vendor agreements address applicable privacy and security obligations.
- Whether incident reporting and breach notification responsibilities are documented.

HIPAA applicability must be determined from MediCore's actual activities and relationships rather than assumed solely because it operates in healthcare technology.

## 7. Technology Dependencies

MediCore's business relies on several technology components and external services.

### AWS Cloud Infrastructure

AWS provides the infrastructure used to host and operate MediCore's SaaS platform.

Potential security responsibilities include:

- Identity and access management.
- Secure resource configuration.
- Data protection and encryption.
- Logging and monitoring.
- Network security.
- Backup and recovery.
- Vulnerability management.

AWS operates under a shared responsibility model. AWS manages security of the cloud, while MediCore remains responsible for security in the cloud according to the services and configurations it uses.

### External AI Provider

MediCore integrates an external generative AI service.

The assessment must determine:

- What information is transmitted to the AI provider.
- Whether ePHI or other sensitive information is included.
- How submitted information is retained and deleted.
- Whether submitted data may be used for model training.
- Which subprocessors support the service.
- What security and privacy commitments exist.
- Whether appropriate contractual agreements are in place.

### Third-Party Technology Providers

Additional vendors may support infrastructure, software development, monitoring, data processing, or other business operations.

These dependencies introduce potential risks if vendor security controls are inadequate or if MediCore lacks sufficient oversight.

## 8. Preliminary Business Risk Assessment

Based on the initial business profile, three areas warrant priority investigation.

These are preliminary risk hypotheses and have not yet been validated through evidence collection or technical testing.

### Risk 1: Unauthorized Access to Sensitive Healthcare Information

**Business concern:** Exposure of sensitive healthcare information.

Weak identity and access management controls, excessive privileges, or inadequate authentication could allow unauthorized individuals to access sensitive information.

Potential business consequences include:

- Unauthorized disclosure of patient information.
- Patient privacy harm.
- Regulatory and contractual exposure.
- Investigation and remediation expenses.
- Loss of customer confidence.
- Potential damage to MediCore's reputation.

**Initial investigation:** Evaluate multifactor authentication, privileged access, access reviews, user provisioning, and data access controls.

### Risk 2: Ransomware and Business Interruption

**Business concern:** Loss of platform availability and operational continuity.

A ransomware incident could disrupt MediCore's technology environment, restrict access to critical information, or result in the theft of sensitive data.

Potential business consequences include:

- SaaS platform downtime.
- Disruption to healthcare customers.
- Recovery and incident response expenses.
- Potential data exposure.
- Contractual and regulatory consequences.
- Lost revenue and customer relationships.

**Initial investigation:** Evaluate backup isolation, recovery testing, incident response procedures, centralized logging, and disaster recovery capabilities.

### Risk 3: Third-Party AI and Vendor Security Exposure

**Business concern:** Loss of control over sensitive information and external technology dependencies.

Insufficient vendor oversight or unclear AI data-handling practices could expose sensitive information or introduce weaknesses into MediCore's environment.

Potential business consequences include:

- Unauthorized disclosure of sensitive information.
- Inadequate contractual protections.
- Privacy and regulatory exposure.
- AI-related security incidents.
- Loss of enterprise customer confidence.
- Delays or failure in securing the prospective hospital contract.

**Initial investigation:** Review vendor security documentation, SOC 2 reports, BAAs where applicable, data retention practices, subprocessors, security incident notification terms, and AI security safeguards.

## 9. Business Impact & Assessment Priorities

MediCore's most important business assets include its SaaS platform, customer relationships, sensitive healthcare information, cloud infrastructure, and third-party technology integrations.

The initial assessment will prioritize risks that could significantly affect:

1. Confidentiality of sensitive healthcare information.
2. Availability of critical business services.
3. Integrity and reliability of healthcare-related information.
4. Regulatory and contractual obligations.
5. Revenue and enterprise customer relationships.
6. Operational resilience and business continuity.

The potential $4 million hospital contract makes security assurance an important business priority.

Security deficiencies may create commercial consequences even when they have not resulted in a confirmed security incident.

## 10. Assessment Stakeholders

The following departments and roles should participate in the assessment.

| Department | Primary Contribution |
|---|---|
| Information Security | Assessment coordination and security risk oversight |
| IT | Enterprise systems and technology operations |
| Cloud Engineering | AWS architecture and configuration evidence |
| Security Operations | Monitoring, detection, and incident response |
| Compliance | Regulatory and control requirements |
| Privacy | Sensitive information handling and privacy practices |
| Legal | Contractual and legal obligations |
| AI Engineering | AI architecture, data flows, and safeguards |
| Software Engineering | Application security and development practices |
| Vendor Management | Third-party relationships and due diligence |
| Business Continuity | Backup, recovery, and resilience planning |
| Product Management | Product requirements and customer impact |

The analyst will coordinate with these stakeholders to understand existing processes, obtain evidence, validate control implementation, and identify risk ownership.

## 11. Initial Assessment Questions

The following questions require further investigation:

1. What healthcare information does MediCore collect and process?
2. Which systems store or transmit ePHI?
3. Which employees and external parties can access sensitive information?
4. Are multifactor authentication requirements enforced consistently?
5. Are privileged accounts reviewed regularly?
6. Are AWS security configurations monitored?
7. Are cloud audit logs centrally collected and retained?
8. Are backups isolated from production credentials?
9. Have restoration procedures been tested?
10. What information is transmitted to the external AI provider?
11. Does the AI provider retain or use submitted information?
12. Have third-party vendors completed security assessments?
13. Are appropriate contractual agreements in place?
14. Has MediCore conducted incident response exercises?
15. Who owns the remediation of identified security deficiencies?

Answers should be supported by documentation, interviews, technical evidence, or other appropriate validation.

## 12. Analyst Conclusion

MediCore's business model depends on reliable cloud infrastructure, secure healthcare information processing, and trusted third-party technology providers.

The initial discovery identifies three priority areas for further investigation: sensitive healthcare information access, ransomware resilience, and third-party AI and vendor security.

These areas could affect MediCore's ability to maintain operations, fulfill contractual obligations, protect customer information, and secure enterprise business opportunities.

The next assessment phase will establish the formal assessment scope, identify accountable stakeholders, document assumptions and limitations, and initiate structured evidence collection.

No security control deficiencies should be considered confirmed until appropriate evidence has been obtained and evaluated.

---

## Document Control

| Field | Value |
|---|---|
| Document Owner | IT Risk & Cybersecurity Analyst |
| Organization | MediCore Health Technologies |
| Version | 1.0 |
| Status | Initial Draft |
| Classification | Simulated Portfolio Work Product |
| Last Updated | November 2026 |

**Disclaimer:** This document is part of a fictional educational portfolio project. All company information, business activities, and risk scenarios are simulated. It does not represent an actual audit, security assessment, or compliance attestation.