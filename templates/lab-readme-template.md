# Lab XX - Lab Title

## Objective

Describe the primary technical and learning objectives of the lab.

By completing this lab, I will:

- Objective one
- Objective two
- Objective three
- Objective four

---

## Business Problem Solved

Explain:

- The current business or technical challenge
- The operational risk created by the challenge
- The Azure capability that addresses the requirement
- The expected business outcome

---

## Scenario

Monroe Redstone Technology Group is evaluating Microsoft Azure to support secure, governed, and cost-conscious cloud adoption.

In this lab, MRTG must:

- Requirement one
- Requirement two
- Requirement three
- Requirement four

The completed configuration will establish a foundation for subsequent Azure labs and future production planning.

---

## Azure Services Used

| Azure Service | Purpose |
|---|---|
| Service name | Explain how the service is used |
| Service name | Explain how the service is used |
| Service name | Explain how the service is used |

---

## Why These Services Were Used

### Service Name

Explain:

- What the service provides
- Why it was selected
- What requirement it satisfies
- What alternative could have been used
- Why the alternative was not selected

### Service Name

Explain:

- What the service provides
- Why it was selected
- What requirement it satisfies
- What alternative could have been used
- Why the alternative was not selected

---

## Environment

| Component | Configuration |
|---|---|
| Organization | Monroe Redstone Technology Group |
| Project | MRTG Azure Fundamentals: The Bridge |
| Lab | Lab XX |
| Azure account | Dedicated MRTG lab account |
| Subscription | `MRTG-AZ900-Lab-Subscription` |
| Primary region | `Central US` |
| Environment | Lab |
| Management interface | Azure portal |
| Authentication | Microsoft Authenticator |
| Documentation platform | GitHub |

### Resource Naming Convention

```text
<resource-type>-<organization>-<project>-<lab>-<region>-<instance>
```

### Example Resource Name

```text
rg-mrtg-az900-labxx-centralus-001
```

### Required Tags

| Tag | Value |
|---|---|
| `Project` | `MRTG-AZ900-The-Bridge` |
| `Lab` | `Lab-XX` |
| `Environment` | `Lab` |
| `Owner` | `MRTG-Cloud-Operations` |
| `CostCenter` | `Training` |
| `ManagedBy` | `Azure-Portal` |
| `DeleteAfter` | `YYYY-MM-DD` |

---

## Architecture / Concept Diagram

```text
+-------------------------------------------------------+
|              Microsoft Azure Tenant                   |
|                                                       |
|  +-------------------------------------------------+  |
|  | MRTG-AZ900-Lab-Subscription                    |  |
|  |                                                 |  |
|  |  +-------------------------------------------+  |  |
|  |  | Resource Group                            |  |  |
|  |  |                                           |  |  |
|  |  |  +-------------+    +------------------+  |  |  |
|  |  |  | Azure       |    | Azure            |  |  |  |
|  |  |  | Resource    |    | Resource         |  |  |  |
|  |  |  +-------------+    +------------------+  |  |  |
|  |  +-------------------------------------------+  |  |
|  +-------------------------------------------------+  |
+-------------------------------------------------------+
```

Update the diagram to represent the resources, identities, network paths, management scopes, or service relationships demonstrated in the lab.

---

## Steps Performed

### Step 1: Step Title

1. Open the required Azure service or management interface.
2. Navigate to the appropriate configuration page.
3. Enter the required configuration.
4. Review the configuration for accuracy.
5. Save, create, or apply the change.

Configuration:

```text
Setting: Value
Setting: Value
Setting: Value
```

![Description of the configuration](screenshots/01-descriptive-screenshot-name.png)

**Screenshot evidence:** The screenshot confirms that the required configuration was entered correctly.

---

### Step 2: Step Title

1. Perform the required action.
2. Configure the required settings.
3. Review the configuration.
4. Complete the operation.

Configuration:

```text
Setting: Value
Setting: Value
Setting: Value
```

![Description of the configuration](screenshots/02-descriptive-screenshot-name.png)

**Screenshot evidence:** The screenshot confirms that the configuration was completed successfully.

---

### Step 3: Step Title

1. Open the deployed resource or completed configuration.
2. Review its status and properties.
3. Confirm the expected values.
4. Record the validation result.

![Description of the validation](screenshots/03-descriptive-screenshot-name.png)

**Screenshot evidence:** The screenshot confirms that the expected result was achieved.

---

## Validation

| Validation Check | Expected Result | Observed Result | Status |
|---|---|---|---|
| Configuration check | Expected behavior | Observed behavior | Passed |
| Deployment check | Expected behavior | Observed behavior | Passed |
| Access check | Expected behavior | Observed behavior | Passed |
| Governance check | Expected behavior | Observed behavior | Passed |
| Cost check | Expected behavior | Observed behavior | Passed |

### Validation Procedure

1. Open the deployed resource or relevant Azure service.
2. Confirm the deployment status.
3. Review the configured properties.
4. Test the required functionality.
5. Review access permissions where applicable.
6. Confirm that the required tags are present.
7. Review the Activity Log where applicable.
8. Check Cost Management for unexpected charges.
9. Compare the observed results with the expected results.

### Validation Evidence

![Final validation result](screenshots/04-final-validation.png)

**Final validation result:** The required Azure configuration was created, reviewed, and validated successfully.

---

## AZ-900 Exam Objective Coverage

### Exam Domain

```text
Describe cloud concepts
```

or:

```text
Describe Azure architecture and services
```

or:

```text
Describe Azure management and governance
```

### Skills Measured

- Relevant Microsoft AZ-900 skill
- Relevant Microsoft AZ-900 skill
- Relevant Microsoft AZ-900 skill
- Relevant Microsoft AZ-900 skill

### How This Lab Supports the Objective

Explain:

- The Azure concepts demonstrated
- The services examined or configured
- The business requirements addressed
- The differences between similar Azure services
- The decisions an AZ-900 candidate should understand

---

## Mini Objective Coverage

By completing this lab, I can now:

- Describe the purpose of the Azure service
- Identify the business problem addressed by the service
- Explain where the service fits within Azure architecture
- Describe its security and governance considerations
- Explain its cost considerations
- Compare it with relevant alternatives
- Recognize scenarios in which the service should be selected

---

## IAM / Security Relevance

This lab relates to identity and security through:

- Authentication
- Authorization
- Role-based access control
- Least-privilege access
- Scope inheritance
- Resource ownership
- Administrative separation
- Shared responsibility
- Zero Trust
- Defense in depth
- Logging and accountability

### On-Premises Connection

| On-Premises Concept | Azure Concept |
|---|---|
| Active Directory identity | Microsoft Entra identity |
| Security group membership | Azure RBAC role assignment |
| Organizational structure | Management group, subscription, and resource-group hierarchy |
| Delegated administration | Scoped Azure role assignment |
| Group Policy | Azure Policy |
| Event logs | Azure Activity Log and Azure Monitor |
| Administrative boundaries | Azure scopes and resource organization |

### Security Analysis

Explain:

- Who can access the resource
- How access is authenticated
- How access is authorized
- Which scope controls the permission
- Whether permissions are inherited
- What the minimum required access should be
- What security controls would be added in production

---

## Governance Notes

Governance considerations include:

- Resource naming
- Resource tagging
- Subscription organization
- Resource-group placement
- Role-assignment scope
- Azure Policy applicability
- Resource-lock applicability
- Cost ownership
- Activity logging
- Compliance requirements
- Resource lifecycle management
- Cleanup responsibility

### Governance Decisions

| Decision | Implementation | Reason |
|---|---|---|
| Naming | Standard MRTG naming convention | Improves identification and consistency |
| Tagging | Standard MRTG tag set | Supports ownership, reporting, and cost tracking |
| Scope | Narrowest practical scope | Reduces unnecessary administrative access |
| Region | `Central US` unless otherwise required | Maintains lab consistency |
| Cleanup | Defined cleanup date | Reduces abandoned resources and unexpected costs |

---

## Cost Considerations

### Cost Factors

Potential cost factors include:

- Resource type
- Service tier
- Region
- Runtime
- Storage capacity
- Data transfer
- Transaction volume
- Monitoring ingestion
- Backup retention
- Licensing
- Optional premium features

### Cost Controls Applied

- Used free or low-cost services where practical
- Reviewed pricing before deployment
- Used the smallest practical resource size
- Applied cost-management tags
- Monitored subscription spending
- Confirmed that the budget remained active
- Avoided unnecessary premium features
- Defined a cleanup plan
- Removed resources when no longer required

### Budget Limitation

Azure budgets provide monitoring and notifications. They do not automatically stop resources or prevent additional charges.

### Estimated Lab Cost

```text
Estimated cost: $0.00 to $X.XX
```

Actual cost depends on the region, service configuration, usage duration, free-service eligibility, and current Azure pricing.

---

## Troubleshooting Notes

### Issue 1: Issue Title

**Symptom:**

Describe the error, unexpected behavior, or failed validation.

**Cause:**

Explain the confirmed or likely cause.

**Resolution:**

1. Troubleshooting action
2. Troubleshooting action
3. Corrective action
4. Validation action

**Result:**

Describe the final outcome.

---

### Issue 2: Issue Title

**Symptom:**

Describe the issue.

**Cause:**

Describe the cause.

**Resolution:**

Describe the corrective steps.

**Result:**

Describe the outcome.

---

## What I Would Do Differently in Production

A production implementation could include:

- Separate administrator and standard-user accounts
- Microsoft Entra groups instead of direct user assignments
- Privileged Identity Management
- Conditional Access
- Emergency access accounts
- Formal approval workflows
- Infrastructure as code
- Peer review
- Change management
- Azure Policy enforcement
- Resource locks
- Private endpoints
- Network segmentation
- Centralized logging
- SIEM integration
- Backup and disaster recovery
- High-availability design
- Defined recovery objectives
- Automated compliance reporting
- Formal cost ownership
- Separate development, testing, and production subscriptions

Explain which controls apply to this lab and why they were not required in the learning environment.

---

## Lessons Learned

Key lessons from this lab include:

- Lesson one
- Lesson two
- Lesson three
- Lesson four
- Lesson five

### Technical Takeaway

Summarize the most important technical lesson.

### Business Takeaway

Summarize the business value of the Azure service or concept.

### Security Takeaway

Summarize the identity, access, or security implication.

### Exam Takeaway

Summarize what should be remembered for the AZ-900 exam.

---

## Cleanup

### Resources Retained

| Resource | Reason |
|---|---|
| Resource name | Required for the next lab or future validation |

### Resources Removed

| Resource | Reason |
|---|---|
| Resource name | No longer required and could generate cost |

### Cleanup Procedure

1. Open the relevant resource group.
2. Review all resources and dependencies.
3. Confirm that no retained resource depends on the item being removed.
4. Delete the unnecessary resource or resource group.
5. Monitor the deletion process.
6. Confirm that the resource no longer appears.
7. Review Cost Management for remaining billable resources.

### Cleanup Validation

- [ ] Unnecessary resources were deleted
- [ ] Required resources were retained
- [ ] No unattached disks remain
- [ ] No unused public IP addresses remain
- [ ] No unnecessary premium services remain enabled
- [ ] Cost Management was reviewed
- [ ] The final resource state was documented

---

## Outcome

This lab successfully demonstrated:

- Completed capability
- Completed capability
- Completed capability
- Completed capability

The final configuration met the defined technical, security, governance, and cost-management requirements.

The lab also established a practical connection between the relevant AZ-900 concepts and their application within an Azure environment.

---

## Next Lab

The next lab is:

```text
Lab XX - Next Lab Title
```

The next lab will build on this work by:

- Next objective
- Next objective
- Next objective
- Next objective
