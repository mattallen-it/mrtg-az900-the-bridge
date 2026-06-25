# MRTG Azure Fundamentals: The Bridge

A hands-on Microsoft Azure Fundamentals lab series connecting on-premises identity and access management concepts to Azure cloud services, security, governance, cost management, and administration.

## Project Overview

**MRTG Azure Fundamentals: The Bridge** documents the transition from traditional on-premises infrastructure and identity administration into Microsoft Azure.

This project is aligned with the Microsoft **AZ-900: Azure Fundamentals** certification objectives. It combines conceptual study, practical Azure portal experience, security analysis, cost awareness, governance decisions, and professional technical documentation.

Each lab approaches Azure from an operational and business perspective. The objective is not simply to deploy resources, but to understand:

- What problem the service solves
- Why an organization would use it
- How it fits into Azure architecture
- Who is responsible for securing it
- How identity and access are controlled
- What governance requirements apply
- How costs are monitored
- How the deployment would differ in production

---

## The Bridge

This project extends previous hands-on experience with:

- Active Directory Domain Services
- Organizational units
- Users and security groups
- Group Policy
- Role-based administration
- Identity lifecycle management
- Authentication and authorization
- Least-privilege access
- Windows Server administration
- Security monitoring
- Governance documentation

The series connects those concepts to Azure technologies such as:

- Microsoft Entra ID
- Azure role-based access control
- Azure subscriptions and resource groups
- Azure compute, networking, and storage
- Azure Policy
- Resource locks
- Azure Cost Management
- Azure Monitor
- Microsoft Defender for Cloud
- Infrastructure deployment tools
- Cloud governance
- Shared responsibility

The result is a documented progression from on-premises IAM foundations into cloud identity, security, governance, and administration.

---

## Business Scenario

Monroe Redstone Technology Group is evaluating Microsoft Azure as an extension of its existing technology environment.

The organization requires a structured Azure foundation that supports:

- Secure cloud adoption
- Centralized identity and access management
- Controlled resource deployment
- Cost visibility and accountability
- Standardized naming and tagging
- Governance and compliance
- Monitoring and operational awareness
- Future hybrid identity integration
- Repeatable technical documentation

This lab series documents the foundational knowledge and technical decisions required to begin that transition.

---

## Project Objectives

The objectives of this project are to:

- Build practical familiarity with the Azure portal
- Explain core cloud concepts using business scenarios
- Identify appropriate Azure services for common requirements
- Understand Azure regions, availability zones, and resource hierarchy
- Compare Azure compute, networking, and storage options
- Connect traditional IAM concepts to Microsoft Entra ID and Azure RBAC
- Apply cost-management and governance controls
- Evaluate Azure management and deployment tools
- Use monitoring and service-health features
- Document security, cost, and production considerations
- Prepare for the Microsoft AZ-900 certification
- Build a professional cloud portfolio using repeatable standards

---

## Certification Alignment

This project follows the Microsoft AZ-900 skills measured as of **January 14, 2026**.

| Exam Domain | Weight |
|---|---:|
| Describe cloud concepts | 25-30% |
| Describe Azure architecture and services | 35-40% |
| Describe Azure management and governance | 30-35% |

### Describe Cloud Concepts

- Cloud computing
- Shared responsibility
- Public, private, and hybrid cloud models
- Consumption-based pricing
- Serverless computing
- High availability
- Scalability
- Reliability
- Predictability
- Security and governance
- Infrastructure as a Service
- Platform as a Service
- Software as a Service

### Describe Azure Architecture and Services

- Azure regions and region pairs
- Availability zones
- Sovereign regions
- Azure datacenters
- Azure resources and resource groups
- Subscriptions
- Management groups
- Compute services
- Virtual machines
- Containers
- Azure Functions
- Application hosting
- Virtual networking
- Public and private endpoints
- Azure DNS
- Storage services
- Storage redundancy
- File migration
- Microsoft Entra ID
- Authentication methods
- External identities
- Conditional Access
- Azure RBAC
- Zero Trust
- Defense in depth
- Microsoft Defender for Cloud

### Describe Azure Management and Governance

- Cost factors
- Azure Pricing Calculator
- Azure Cost Management
- Resource tags
- Microsoft Purview
- Azure Policy
- Resource locks
- Azure portal
- Azure Cloud Shell
- Azure CLI
- Azure PowerShell
- Azure Arc
- Infrastructure as code
- ARM templates
- Azure Advisor
- Azure Service Health
- Azure Monitor
- Log Analytics
- Azure Monitor alerts
- Application Insights

---

## Learning Methodology

Every lab follows the same workflow:

```text
Learn -> Build -> Document -> Explain -> Map
```

### Learn

Study the Azure concepts, services, terminology, and business requirements associated with the lab.

### Build

Use the Azure portal and other approved management tools to configure or examine the required services.

### Document

Record the process with sanitized screenshots, configuration details, validation results, and troubleshooting notes.

### Explain

Describe why the technology was selected, what problem it solves, and how it would be used in a production environment.

### Map

Connect the completed work to the applicable AZ-900 exam objectives and existing IAM, infrastructure, security, or governance knowledge.

---

## Lab Roadmap

| Lab | Title | Primary Focus | Status |
|---:|---|---|---|
| 01 | Azure Environment and Cost Protection | Account security, subscription validation, budgets, naming, tagging, and resource groups | In Progress |
| 02 | Cloud Computing and Shared Responsibility | Cloud concepts, shared responsibility, consumption models, and serverless computing | Planned |
| 03 | Cloud Models, Benefits, and Service Types | Public, private, and hybrid cloud; IaaS, PaaS, and SaaS | Planned |
| 04 | Azure Architecture and Resource Hierarchy | Regions, availability zones, resources, resource groups, subscriptions, and management groups | Planned |
| 05 | Azure Compute Services | Virtual machines, containers, functions, application hosting, and compute selection | Planned |
| 06 | Azure Networking Foundation | Virtual networks, subnets, peering, endpoints, routing, security, and DNS | Planned |
| 07 | Azure Storage Services | Storage accounts, blobs, files, queues, tables, redundancy, and access tiers | Planned |
| 08 | Microsoft Entra ID, RBAC, and Zero Trust | Identity, authentication, authorization, Conditional Access, RBAC, and Zero Trust | Planned |
| 09 | Azure Cost Management and Resource Organization | Cost analysis, budgets, pricing, tags, and resource organization | Planned |
| 10 | Azure Governance, Policy, and Compliance | Azure Policy, resource locks, governance, compliance, and Microsoft Purview | Planned |
| 11 | Azure Management and Deployment Tools | Portal, Cloud Shell, CLI, PowerShell, ARM templates, IaC, and Azure Arc | Planned |
| 12 | Azure Monitoring, Health, and Optimization | Azure Monitor, Log Analytics, alerts, Service Health, Advisor, and Application Insights | Planned |
| 13 | MRTG Azure Fundamentals Capstone | Integrated architecture, service selection, security, governance, cost, and operational planning | Planned |

---

## Repository Structure

```text
mrtg-az900-the-bridge/
├── README.md
├── LICENSE
├── .gitignore
├── assets/
│   └── screenshots/
├── docs/
├── labs/
│   ├── lab-01-azure-environment-and-cost-protection/
│   │   ├── README.md
│   │   └── screenshots/
│   ├── lab-02-cloud-computing-and-shared-responsibility/
│   ├── lab-03-cloud-models-benefits-and-service-types/
│   ├── lab-04-azure-architecture-and-resource-hierarchy/
│   ├── lab-05-azure-compute-services/
│   ├── lab-06-azure-networking-foundation/
│   ├── lab-07-azure-storage-services/
│   ├── lab-08-entra-id-rbac-and-zero-trust/
│   ├── lab-09-cost-management-and-resource-organization/
│   ├── lab-10-governance-policy-and-compliance/
│   ├── lab-11-management-and-deployment-tools/
│   ├── lab-12-monitoring-health-and-optimization/
│   └── lab-13-azure-fundamentals-capstone/
└── templates/
    └── lab-readme-template.md
```

Lab directories are added as the series progresses. Git does not track empty directories, so placeholder files may be used until documentation or screenshots are added.

---

## Lab Documentation Standard

Each lab README uses the following structure:

1. Lab title
2. Objective
3. Business Problem Solved
4. Scenario
5. Azure Services Used
6. Why These Services Were Used
7. Environment
8. Architecture or Concept Diagram
9. Steps Performed
10. Validation
11. AZ-900 Exam Objective Coverage
12. Mini Objective Coverage
13. IAM and Security Relevance
14. Governance Notes
15. Cost Considerations
16. Troubleshooting Notes
17. What I Would Do Differently in Production
18. Lessons Learned
19. Cleanup
20. Outcome
21. Next Lab

This standard ensures that each lab documents both the technical work and the reasoning behind it.

---

## Screenshot Standard

Each lab stores its evidence in a dedicated folder:

```text
labs/<lab-folder>/screenshots/
```

Screenshot filenames use the following format:

```text
01-descriptive-screenshot-name
02-descriptive-screenshot-name
03-descriptive-screenshot-name
```

Screenshot requirements:

- Use sequential two-digit numbering
- Use lowercase filenames
- Separate words with hyphens
- Describe the configuration or validation being shown
- Capture only information relevant to the lab
- Crop unnecessary browser and desktop content
- Maintain a consistent image size when practical
- Place screenshots near the related README steps
- Review every screenshot before committing it

Screenshots must not expose:

- Passwords
- Authentication codes
- Recovery codes
- Authenticator QR codes
- Access tokens
- API keys
- Storage account keys
- Connection strings
- Payment-card information
- Billing addresses
- Phone numbers
- Recovery email addresses
- Subscription IDs
- Tenant IDs
- Object IDs
- Sensitive account notifications
- Public IP addresses when disclosure is unnecessary

---

## Azure Naming Standard

Azure resources use a predictable naming structure:

```text
<resource-type>-<organization>-<project>-<lab>-<region>-<instance>
```

Example:

```text
rg-mrtg-az900-lab01-centralus-001
```

Common abbreviations:

| Resource | Abbreviation |
|---|---|
| Resource group | `rg` |
| Virtual network | `vnet` |
| Subnet | `snet` |
| Network security group | `nsg` |
| Virtual machine | `vm` |
| Network interface | `nic` |
| Public IP address | `pip` |
| Storage account | `st` |
| Log Analytics workspace | `log` |

Some Azure resources have unique naming restrictions. Names may be adjusted when a service does not support the complete standard.

---

## Azure Tagging Standard

Resources are tagged where the service supports tags.

| Tag | Standard Value |
|---|---|
| `Project` | `MRTG-AZ900-The-Bridge` |
| `Lab` | Lab-specific value |
| `Environment` | `Lab` |
| `Owner` | `MRTG-Cloud-Operations` |
| `CostCenter` | `Training` |
| `ManagedBy` | `Azure-Portal` |
| `DeleteAfter` | Lab-specific cleanup date |

Tags support:

- Resource ownership
- Cost allocation
- Environment identification
- Governance
- Reporting
- Automation
- Cleanup planning

Tags are organizational metadata. They do not replace Azure RBAC, Azure Policy, resource locks, or security controls.

---

## Security Principles

The project applies the following security principles:

- Use a dedicated Microsoft account for the lab environment
- Protect the account with multifactor authentication
- Use Microsoft Authenticator where supported
- Apply least-privilege access
- Separate authentication from authorization
- Avoid unnecessary public exposure
- Review permissions before assigning roles
- Prefer role assignments at the narrowest practical scope
- Do not store credentials in the repository
- Sanitize screenshots before publishing
- Remove resources that are no longer required
- Document production security improvements
- Apply Zero Trust principles when evaluating access

This is a learning environment, but security controls are treated as operational requirements rather than optional additions.

---

## Cost-Management Principles

Every resource deployed in this project must have a clear purpose and cleanup plan.

Cost controls include:

- Reviewing estimated cost before deployment
- Using free or low-cost services when practical
- Creating subscription-level budgets and alerts
- Monitoring current and forecasted spending
- Reviewing free-service usage
- Applying ownership and cost-center tags
- Avoiding oversized resources
- Deallocating virtual machines when they are not needed
- Deleting unused disks, public IP addresses, and dependent resources
- Removing completed lab environments
- Checking Cost Management after each deployment

Azure budgets provide notifications. They do not automatically stop resources or prevent additional charges.

Premium services, paid support plans, and optional security features are not enabled unless they are required, understood, and documented.

---

## Governance Principles

The project uses foundational governance practices throughout the lab series:

- Consistent resource naming
- Standardized tagging
- Subscription and resource-group organization
- Least-privilege role assignments
- Azure Policy evaluation
- Resource-lock evaluation
- Cost monitoring
- Activity-log review
- Documentation of ownership
- Defined cleanup dates
- Production-readiness analysis

Later labs expand these practices into policy enforcement, compliance evaluation, monitoring, and operational management.

---

## Environment

The lab environment may include:

- Microsoft Azure portal
- Microsoft Entra ID
- Azure Cloud Shell
- Azure CLI
- Azure PowerShell
- Azure Resource Manager
- Windows-based administrative workstation
- GitHub for version control and documentation
- Microsoft Learn for certification-aligned reference material

The specific services used are documented inside each lab.

---

## Validation Standard

A deployment is not considered complete simply because Azure reports that it was created.

Validation may include:

- Confirming resource deployment status
- Reviewing resource properties
- Testing connectivity
- Testing authentication
- Confirming authorization behavior
- Reviewing role assignments
- Confirming tags
- Reviewing the Activity Log
- Checking monitoring data
- Reviewing cost information
- Confirming cleanup
- Verifying that documentation matches the deployed environment

Each lab records both the expected result and the observed result.

---

## Production Perspective

The labs use controlled configurations intended for learning and certification preparation. They do not automatically represent complete production architectures.

Each lab identifies production considerations such as:

- Identity separation
- Privileged access controls
- Conditional Access
- Network isolation
- Private endpoints
- High availability
- Backup and recovery
- Monitoring and alerting
- Infrastructure as code
- Change control
- Policy enforcement
- Centralized logging
- Compliance requirements
- Cost ownership
- Resource lifecycle management

This distinction prevents a successful demonstration from being mistaken for a production-ready deployment.

---

## Project Progress

| Milestone | Status |
|---|---|
| Repository initialized | Complete |
| Project standards defined | Complete |
| Azure lab account secured | In Progress |
| Azure subscription configured | Not Started |
| Cost protections configured | Not Started |
| Core cloud-concept labs completed | Not Started |
| Azure architecture labs completed | Not Started |
| Identity and security lab completed | Not Started |
| Governance and management labs completed | Not Started |
| Monitoring lab completed | Not Started |
| Capstone completed | Not Started |
| AZ-900 exam preparation review completed | Not Started |

Progress is updated as each lab is completed and validated.

---

## Expected Outcomes

By completing this series, I will be able to:

- Explain fundamental cloud concepts
- Compare cloud deployment and service models
- Describe Azure architecture and resource hierarchy
- Identify appropriate Azure compute, networking, and storage services
- Explain Microsoft Entra ID and Azure RBAC
- Describe Zero Trust and defense-in-depth concepts
- Explain Azure pricing and cost-management tools
- Describe Azure governance and compliance capabilities
- Identify Azure management and deployment tools
- Explain Azure monitoring, health, and optimization services
- Translate on-premises IAM knowledge into Azure terminology
- Discuss Azure services from technical and business perspectives
- Demonstrate certification-aligned knowledge with documented practical work

---

## Future Direction

This project establishes the foundation for more advanced Microsoft cloud work, including:

- Microsoft 365 fundamentals and administration
- Hybrid identity
- Microsoft Entra Connect
- Microsoft Entra Cloud Sync
- SC-900: Microsoft Security, Compliance, and Identity Fundamentals
- SC-300: Microsoft Identity and Access Administrator
- AZ-104: Microsoft Azure Administrator
- Conditional Access
- Privileged Identity Management
- Identity Governance
- Azure landing zones
- Infrastructure as code
- Cloud security operations

---

## Disclaimer

This repository is an independent educational and portfolio project.

It is not affiliated with, endorsed by, or sponsored by Microsoft. Microsoft Azure, Microsoft Entra, Microsoft 365, Windows Server, and related product names are trademarks of Microsoft Corporation.

Azure services, pricing, interfaces, free-service allowances, certification objectives, and product features may change. Current Microsoft documentation should always be reviewed before deploying resources or scheduling an exam.

No real production credentials, customer data, private organizational information, or intentionally sensitive account details are included in this repository.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Author

**Matthew Allen**  
**Monroe Redstone Technology Group**

Focus areas:

- Identity and access management
- Microsoft Azure
- Microsoft Entra ID
- Windows Server
- Active Directory
- Cloud security
- Governance
- Systems administration
