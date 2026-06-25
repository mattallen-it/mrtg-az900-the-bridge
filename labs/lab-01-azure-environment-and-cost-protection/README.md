# Lab 01 - Azure Environment and Cost Protection

## Objective

Establish a secure, organized, and cost-conscious Microsoft Azure lab environment for the MRTG Azure Fundamentals series.

By completing this lab, I will:

- Secure the dedicated MRTG Microsoft account
- Activate and validate an Azure subscription
- Establish subscription-level cost monitoring
- Create a monthly Azure budget
- Define resource naming and tagging standards
- Create the first governed Azure resource group
- Validate the environment before deploying billable workloads

---

## Business Problem Solved

Cloud resources can be deployed quickly, but an unmanaged Azure environment can create security, ownership, governance, and financial risks.

Monroe Redstone Technology Group requires an Azure foundation that:

- Protects the primary administrative identity
- Provides visibility into cloud spending
- Identifies resource ownership and purpose
- Uses consistent naming and tagging
- Separates lab resources from unrelated environments
- Supports reliable auditing and cleanup
- Reduces the risk of unexpected charges

This lab establishes those controls before MRTG deploys Azure workloads.

---

## Scenario

Monroe Redstone Technology Group is beginning its adoption of Microsoft Azure.

Before evaluating compute, networking, storage, identity, and governance services, MRTG must establish a controlled Azure environment.

The organization must:

- Secure its dedicated cloud-operations account
- Confirm that its Azure subscription is active
- Configure cost monitoring and budget alerts
- Establish naming and tagging standards
- Create an organized resource-group structure
- Verify that no unexpected billable resources are running

The completed environment will support the remaining labs in the series.

---

## Azure Services Used

| Azure Service or Feature | Purpose |
|---|---|
| Azure portal | Provides the primary browser-based Azure management interface |
| Azure subscription | Establishes the billing, access-control, and resource-management boundary |
| Azure Cost Management | Provides cost analysis, budgets, alerts, and spending visibility |
| Azure Resource Manager | Organizes and manages Azure resources through consistent management scopes |
| Azure resource groups | Provide logical containers for related Azure resources |
| Azure tags | Add ownership, project, environment, and lifecycle metadata |
| Azure Activity Log | Records subscription-level administrative operations |
| Microsoft Authenticator | Protects the MRTG Microsoft account with an additional verification method |

---

## Why These Services Were Used

### Azure Portal

The Azure portal provides a graphical management interface for creating, reviewing, and administering Azure resources.

It was selected because:

- It supports visual exploration of Azure services
- It is appropriate for foundational AZ-900 labs
- It exposes subscription, governance, and cost-management features
- It provides immediate configuration and validation feedback

Later labs may also use Azure Cloud Shell, Azure CLI, Azure PowerShell, and infrastructure as code.

### Azure Subscription

An Azure subscription provides:

- A billing boundary
- An access-control scope
- A resource-deployment boundary
- A cost-management scope
- A governance scope

The dedicated lab subscription separates MRTG training activity from personal or production Azure environments.

### Azure Cost Management

Azure Cost Management provides visibility into Azure usage and estimated spending.

It was selected to:

- Establish a cost baseline
- Create a monthly budget
- Configure threshold notifications
- Identify unexpected resource charges
- Support cost-conscious deployment decisions

Azure budgets provide alerts. They do not automatically stop resources or prevent additional charges.

### Resource Groups

Resource groups provide logical containers for resources that share a common purpose or lifecycle.

The first resource group establishes:

- A consistent naming pattern
- A defined deployment location
- A common governance scope
- A centralized cleanup boundary
- A foundation for subsequent lab resources

### Azure Tags

Tags provide key-value metadata for Azure resources and resource groups.

They were selected to support:

- Project identification
- Lab identification
- Environment classification
- Ownership
- Cost allocation
- Management-method tracking
- Cleanup scheduling

Tags do not provide access control and do not replace Azure RBAC or Azure Policy.

---

## Environment

| Component | Configuration |
|---|---|
| Organization | Monroe Redstone Technology Group |
| Project | MRTG Azure Fundamentals: The Bridge |
| Lab | Lab 01 |
| Microsoft account | Dedicated MRTG cloud-operations account |
| Account display name | MRTG Cloud Operations |
| Subscription | `MRTG-AZ900-Lab-Subscription` |
| Primary region | `Central US` |
| Environment | Lab |
| Management interface | Azure portal |
| Authentication protection | Microsoft Authenticator and two-step verification |
| Budget | `$10.00` monthly |
| Documentation platform | GitHub |

### Resource Naming Convention

```text
<resource-type>-<organization>-<project>-<lab>-<region>-<instance>
```

### Resource Group Name

```text
rg-mrtg-az900-lab01-centralus-001
```

### Required Tags

| Tag | Value |
|---|---|
| `Project` | `MRTG-AZ900-The-Bridge` |
| `Lab` | `Lab-01` |
| `Environment` | `Lab` |
| `Owner` | `MRTG-Cloud-Operations` |
| `CostCenter` | `Training` |
| `ManagedBy` | `Azure-Portal` |
| `DeleteAfter` | `2026-07-31` |

---

## Architecture / Concept Diagram

```text
+-----------------------------------------------------------+
| Dedicated MRTG Microsoft Account                          |
| Display Name: MRTG Cloud Operations                       |
| Two-Step Verification + Microsoft Authenticator           |
+-----------------------------+-----------------------------+
                              |
                              | Authenticated access
                              v
+-----------------------------------------------------------+
| Microsoft Azure Tenant                                    |
|                                                           |
|  +-----------------------------------------------------+  |
|  | MRTG-AZ900-Lab-Subscription                        |  |
|  |                                                     |  |
|  |  +----------------------+  +---------------------+  |  |
|  |  | Cost Management      |  | Activity Log        |  |  |
|  |  |                      |  |                     |  |  |
|  |  | Monthly Budget: $10  |  | Administrative     |  |  |
|  |  | Alert Thresholds     |  | Operations          |  |  |
|  |  +----------------------+  +---------------------+  |  |
|  |                                                     |  |
|  |  +------------------------------------------------+ |  |
|  |  | rg-mrtg-az900-lab01-centralus-001             | |  |
|  |  |                                                | |  |
|  |  | Region: Central US                             | |  |
|  |  | Standard MRTG Tags                             | |  |
|  |  | Initial Resources: None                        | |  |
|  |  +------------------------------------------------+ |  |
|  +-----------------------------------------------------+  |
+-----------------------------------------------------------+
```

---

## Steps Performed

### Step 1: Secure the Dedicated Microsoft Account

1. Signed in to the dedicated MRTG Microsoft account.
2. Opened the Microsoft account security settings.
3. Added appropriate account-recovery methods.
4. Enabled two-step verification.
5. Added the account to Microsoft Authenticator.
6. Completed the Authenticator verification test.
7. Confirmed that the additional sign-in method was active.
8. Stored recovery information securely outside the repository.

<!-- Add after sanitizing:
![Microsoft account security overview](screenshots/01-microsoft-account-security-overview.png)
-->

<!-- Add after sanitizing:
![Two-step verification enabled](screenshots/02-two-step-verification-enabled.png)
-->

<!-- Add after sanitizing:
![Microsoft Authenticator method confirmed](screenshots/03-authenticator-method-confirmed.png)
-->

**Screenshot requirements:**

- Show the account-security status
- Show that two-step verification is enabled
- Show Microsoft Authenticator as an active method
- Hide phone numbers and recovery email addresses
- Never capture QR codes, verification codes, or recovery codes

---

### Step 2: Register the Azure Account

1. Opened the official Azure account-registration page.
2. Selected the option to begin an Azure account.
3. Signed in with the dedicated MRTG Microsoft account.
4. Entered accurate identity and contact information.
5. Completed phone verification.
6. Completed payment-method verification.
7. Reviewed the applicable agreement and subscription terms.
8. Completed the Azure registration process.

<!-- Add after sanitizing:
![Azure account registration started](screenshots/04-azure-account-registration-started.png)
-->

<!-- Add after sanitizing:
![Azure account registration completed](screenshots/05-azure-account-registration-completed.png)
-->

**Screenshot requirements:**

- Capture only the beginning and successful completion of registration
- Hide the account email address where practical
- Never capture payment-card information
- Never capture phone numbers, addresses, or verification codes

---

### Step 3: Sign In to the Azure Portal

1. Opened the Azure portal.
2. Signed in with the dedicated MRTG Microsoft account.
3. Completed the required identity-verification challenge.
4. Confirmed that the Azure portal loaded successfully.
5. Verified that the correct account and directory were selected.

<!-- Add after sanitizing:
![Azure portal signed in](screenshots/06-azure-portal-signed-in.png)
-->

**Screenshot evidence:** The Azure portal home page confirms successful access to the MRTG Azure environment.

---

### Step 4: Validate the Azure Subscription

1. Searched for **Subscriptions** in the Azure portal.
2. Opened the subscription list.
3. Selected the subscription associated with the MRTG account.
4. Confirmed that the subscription status was active.
5. Reviewed the subscription offer and available usage information.
6. Confirmed that the subscription was associated with the correct directory.
7. Avoided exposing the subscription ID and tenant ID.

<!-- Add after sanitizing:
![Active Azure subscription](screenshots/07-active-azure-subscription.png)
-->

**Expected result:** The Azure subscription appears with an active status and is accessible from the MRTG account.

---

### Step 5: Rename the Subscription

1. Opened the active Azure subscription.
2. Selected the option to rename the subscription.
3. Entered the following name:

```text
MRTG-AZ900-Lab-Subscription
```

4. Saved the change.
5. Refreshed the subscription page.
6. Confirmed that the updated name appeared.

<!-- Add after sanitizing:
![Azure subscription renamed](screenshots/08-subscription-renamed.png)
-->

**Screenshot evidence:** The subscription overview shows the standardized MRTG subscription name and active status.

---

### Step 6: Review Free-Service and Credit Usage

1. Opened the subscription overview.
2. Located the available usage, credit, or free-service information.
3. Reviewed the current credit status.
4. Reviewed available free-service quantities.
5. Recorded applicable expiration information privately.
6. Confirmed that no unexpected service usage was present.

<!-- Add after sanitizing:
![Azure free service usage](screenshots/09-free-service-usage-overview.png)
-->

**Note:** Azure usage information may not appear immediately. Cost and usage data can be delayed after a resource is deployed.

---

### Step 7: Establish the Cost Baseline

1. Searched for **Cost Management + Billing**.
2. Opened **Cost Management**.
3. Selected the MRTG subscription as the management scope.
4. Opened **Cost analysis**.
5. Set the date range to the current month.
6. Reviewed the current estimated cost.
7. Confirmed that no unexpected billable resources were present.

<!-- Add after sanitizing:
![Azure cost analysis baseline](screenshots/10-cost-analysis-baseline.png)
-->

**Expected result:** Cost Management is accessible and displays the current subscription cost.

---

### Step 8: Create the Monthly Budget

1. Opened **Budgets** under the subscription-level Cost Management scope.
2. Selected **Create** or **Add**.
3. Entered the budget configuration:

```text
Budget name: mrtg-az900-monthly-budget
Reset period: Monthly
Budget amount: $10.00
Scope: MRTG-AZ900-Lab-Subscription
```

4. Configured actual-cost alert thresholds:

```text
50 percent: $5.00
80 percent: $8.00
100 percent: $10.00
```

5. Added a forecasted-cost threshold if the option was available.
6. Configured notifications for the MRTG cloud-operations account.
7. Reviewed the budget settings.
8. Created the budget.
9. Confirmed that the budget appeared in the budget list.

<!-- Add after sanitizing:
![Azure budget configuration](screenshots/11-budget-configuration.png)
-->

<!-- Add after sanitizing:
![Azure budget created](screenshots/12-budget-created.png)
-->

**Important:** The budget provides monitoring and notifications only. It does not suspend resources or prevent charges when a threshold is reached.

---

### Step 9: Create the First Resource Group

1. Searched for **Resource groups**.
2. Selected **Create**.
3. Entered the following configuration:

```text
Subscription: MRTG-AZ900-Lab-Subscription
Resource group: rg-mrtg-az900-lab01-centralus-001
Region: Central US
```

4. Opened the **Tags** tab.
5. Added the required MRTG tags:

```text
Project: MRTG-AZ900-The-Bridge
Lab: Lab-01
Environment: Lab
Owner: MRTG-Cloud-Operations
CostCenter: Training
ManagedBy: Azure-Portal
DeleteAfter: 2026-07-31
```

6. Selected **Review + create**.
7. Confirmed that Azure validation succeeded.
8. Selected **Create**.
9. Opened the completed resource group.

<!-- Add after sanitizing:
![Resource group configuration](screenshots/13-resource-group-configuration.png)
-->

<!-- Add after sanitizing:
![Resource group tags](screenshots/14-resource-group-tags.png)
-->

<!-- Add after sanitizing:
![Resource group validation passed](screenshots/15-resource-group-validation-passed.png)
-->

<!-- Add after sanitizing:
![Resource group created](screenshots/16-resource-group-created.png)
-->

**Expected result:** The resource group is created successfully in Central US with the complete MRTG tag set.

---

### Step 10: Validate Tags and Activity

1. Opened the deployed resource group.
2. Reviewed the resource-group overview.
3. Confirmed that the resource count was zero.
4. Opened the resource-group tags.
5. Confirmed that all required tags were present.
6. Opened the **Activity log**.
7. Located the resource-group creation operation.
8. Confirmed that the operation succeeded.

<!-- Add after sanitizing:
![Resource group tags validated](screenshots/17-resource-group-tags-validated.png)
-->

<!-- Add after sanitizing:
![Resource group Activity Log](screenshots/18-resource-group-activity-log.png)
-->

**Screenshot evidence:** The tags and Activity Log confirm that the resource group was created according to the MRTG governance standard.

---

### Step 11: Perform Final Cost Validation

1. Returned to subscription-level Cost Management.
2. Opened **Cost analysis**.
3. Reviewed the current-month estimated cost.
4. Confirmed that no unexpected billable resources existed.
5. Opened **Budgets**.
6. Confirmed that `mrtg-az900-monthly-budget` remained active.
7. Confirmed that the resource group contained no billable workloads.

<!-- Add after sanitizing:
![Final cost protection validation](screenshots/19-final-cost-protection-validation.png)
-->

**Final validation result:** The subscription has cost visibility, an active monthly budget, an organized resource group, and no unexpected billable workloads.

---

## Validation

| Validation Check | Expected Result | Observed Result | Status |
|---|---|---|---|
| Account access | MRTG account can access the Azure portal | Pending lab execution | Pending |
| Account security | Two-step verification and Authenticator are active | Pending lab execution | Pending |
| Subscription status | Azure subscription is active | Pending lab execution | Pending |
| Subscription name | Standard MRTG subscription name is displayed | Pending lab execution | Pending |
| Cost analysis | Subscription cost information is accessible | Pending lab execution | Pending |
| Budget | `$10.00` monthly budget is active | Pending lab execution | Pending |
| Resource group | Resource group exists in Central US | Pending lab execution | Pending |
| Tags | All seven MRTG tags are present | Pending lab execution | Pending |
| Activity Log | Successful creation operation is recorded | Pending lab execution | Pending |
| Resource cost | No unexpected billable resources are running | Pending lab execution | Pending |

Update the **Observed Result** and **Status** columns after each validation check is completed.

### Completion Checklist

- [ ] Dedicated MRTG account secured
- [ ] Two-step verification enabled
- [ ] Microsoft Authenticator configured
- [ ] Azure registration completed
- [ ] Azure portal access confirmed
- [ ] Subscription status confirmed
- [ ] Subscription renamed
- [ ] Free-service usage reviewed
- [ ] Cost baseline reviewed
- [ ] Monthly budget created
- [ ] Budget thresholds configured
- [ ] Resource group created
- [ ] Required tags applied
- [ ] Activity Log reviewed
- [ ] Final cost validation completed
- [ ] Screenshots sanitized and uploaded
- [ ] No sensitive information committed

---

## AZ-900 Exam Objective Coverage

### Primary Exam Domain

```text
Describe Azure management and governance
```

### Secondary Exam Domain

```text
Describe Azure architecture and services
```

### Skills Measured

This lab supports the ability to:

- Describe the factors that can affect costs in Azure
- Compare the Azure Pricing Calculator and Azure Cost Management
- Describe Azure Cost Management capabilities
- Describe the purpose of tags
- Describe Azure subscriptions
- Describe resource groups
- Describe the hierarchy of resource groups, subscriptions, and management groups
- Describe Azure management tools
- Describe the purpose of the Azure portal

### How This Lab Supports the Objectives

This lab demonstrates that an Azure subscription is more than a billing account. It is also an access-control, governance, and resource-management boundary.

The lab provides practical exposure to:

- Subscription management
- Cost analysis
- Budget configuration
- Resource-group organization
- Resource tagging
- Azure portal navigation
- Azure Resource Manager scopes
- Administrative activity logging

---

## Mini Objective Coverage

By completing this lab, I can now:

- Describe the purpose of an Azure subscription
- Explain why subscriptions act as billing and access boundaries
- Describe the purpose of resource groups
- Explain how Azure tags support organization and cost reporting
- Use Azure Cost Management to review estimated spending
- Explain the difference between a budget alert and a spending limit
- Identify the role of the Azure portal
- Recognize the relationship between identity, subscription access, and governance
- Explain why cost controls should be established before workloads are deployed

---

## IAM / Security Relevance

This lab begins the Azure IAM lifecycle by securing the identity that controls the subscription.

The dedicated MRTG account acts as the initial administrative identity for the lab environment. Protecting this account is critical because access to the account can provide access to subscription resources, billing information, role assignments, and governance settings.

### On-Premises Connection

| On-Premises Concept | Azure Concept |
|---|---|
| Administrative user account | Azure administrative identity |
| Domain authentication | Microsoft account or Microsoft Entra authentication |
| Group-based authorization | Azure RBAC role assignments |
| Organizational unit | Resource group as a logical organization boundary |
| Group Policy | Azure Policy |
| Windows Event Log | Azure Activity Log |
| Delegated administration | Scoped Azure RBAC assignment |
| Security baseline | Subscription governance baseline |

### Security Analysis

- Authentication confirms the identity signing in to Azure.
- Authorization determines what the identity can perform.
- Subscription ownership provides extensive administrative control.
- Two-step verification reduces the risk of password-only compromise.
- Resource groups provide scopes for future role assignments.
- The Activity Log creates accountability for management operations.
- Tags provide ownership metadata but do not grant or deny access.

### Sensitive Information Controls

The following information must not be published:

- Passwords
- Authenticator QR codes
- Verification codes
- Recovery codes
- Payment-card information
- Billing addresses
- Phone numbers
- Backup email addresses
- Subscription IDs
- Tenant IDs
- Object IDs
- Access tokens
- Security keys

---

## Governance Notes

### Governance Decisions

| Decision | Implementation | Reason |
|---|---|---|
| Account separation | Dedicated MRTG Microsoft account | Separates lab activity from personal cloud activity |
| Subscription naming | `MRTG-AZ900-Lab-Subscription` | Clearly identifies the subscription’s purpose |
| Resource naming | MRTG naming convention | Improves consistency and resource identification |
| Resource organization | Dedicated Lab 01 resource group | Establishes a logical deployment and cleanup boundary |
| Primary region | `Central US` | Provides regional consistency across the lab series |
| Tagging | Seven standard MRTG tags | Supports ownership, reporting, and lifecycle tracking |
| Cost monitoring | Subscription-level Cost Management | Provides centralized spending visibility |
| Budget | `$10.00` monthly budget | Provides early notification of unexpected spending |
| Cleanup date | `2026-07-31` | Establishes a defined resource-review deadline |
| Audit review | Azure Activity Log | Confirms administrative operations |

### Tagging Limitation

Tags do not automatically inherit from a resource group to its resources unless an Azure Policy or another automation mechanism applies them.

Resources created in later labs must therefore be checked individually for the required tags.

---

## Cost Considerations

### Potential Cost Factors

- Azure service selected
- Resource size and service tier
- Deployment region
- Runtime
- Storage capacity
- Data transfer
- Transactions
- Monitoring-data ingestion
- Backup and retention
- Premium security features
- Resources left deployed after a lab

### Cost Controls Applied

- Established Cost Management before deploying workloads
- Created a `$10.00` monthly budget
- Configured multiple alert thresholds
- Reviewed current-month cost analysis
- Reviewed free-service eligibility
- Created only an empty resource group
- Applied cost-ownership tags
- Added a cleanup date
- Avoided paid workloads during environment setup
- Avoided enabling optional premium services

### Budget Limitation

The Azure budget created in this lab:

- Monitors actual or forecasted costs
- Generates notifications when thresholds are reached
- Does not automatically stop resources
- Does not prevent spending
- Does not replace regular Cost Management reviews

### Estimated Lab Cost

```text
Estimated cost: $0.00
```

Creating an empty resource group and configuring a budget do not create a billable workload. Charges can begin when billable Azure resources or services are deployed.

---

## Troubleshooting Notes

### Issue 1: Azure Free Account Eligibility

**Symptom:**

The expected Azure free-account offer is unavailable.

**Possible Cause:**

The identity, phone number, payment method, or other eligibility information may have been associated with a previous Azure offer.

**Resolution:**

1. Review the message displayed during registration.
2. Confirm that accurate account information was entered.
3. Do not repeatedly create additional accounts to bypass eligibility controls.
4. Review available subscription options.
5. Use only a subscription type with understood billing terms.

### Issue 2: Cost Information Is Not Visible

**Symptom:**

Cost analysis or free-service usage does not display current information.

**Possible Cause:**

Azure cost and usage data may require time to process.

**Resolution:**

1. Confirm that the correct subscription scope is selected.
2. Confirm that the current-month date range is selected.
3. Wait for Azure usage processing to complete.
4. Return to Cost Management later.
5. Verify that the account has permission to view cost information.

### Issue 3: Budget Creation Is Unavailable

**Symptom:**

The option to create a budget is unavailable or disabled.

**Possible Cause:**

The wrong billing scope may be selected, or the account may not have sufficient permissions.

**Resolution:**

1. Return to Cost Management.
2. Select the MRTG subscription scope.
3. Confirm that the account has appropriate subscription access.
4. Reopen **Budgets**.
5. Attempt the configuration again.

### Issue 4: Resource-Group Validation Fails

**Symptom:**

Azure does not allow the resource group to be created.

**Possible Cause:**

The subscription, region, resource-group name, permissions, or policy configuration may be invalid.

**Resolution:**

1. Confirm that the subscription is active.
2. Confirm that `Central US` is available.
3. Review the resource-group name.
4. Confirm that the account has permission to create resource groups.
5. Review the validation message.
6. Correct the identified issue and repeat validation.

---

## What I Would Do Differently in Production

A production Azure environment would use additional controls, including:

- A verified organizational domain
- Microsoft Entra work accounts instead of a consumer Outlook account
- Separate administrator and standard-user identities
- Microsoft Entra groups for role assignments
- Least-privilege Azure RBAC
- Privileged Identity Management
- Conditional Access
- Emergency-access accounts
- Multiple subscriptions for workload separation
- Management groups
- Azure Policy enforcement
- Automated tag inheritance
- Resource locks
- Centralized logging and alerting
- Formal billing ownership
- Department-level cost allocation
- Infrastructure as code
- Peer-reviewed deployments
- Formal change management
- Automated resource-cleanup workflows

The lab uses a simplified design because its purpose is foundational learning and AZ-900 preparation.

---

## Lessons Learned

- Azure governance should begin before workloads are deployed.
- A subscription is a billing, access-control, and governance boundary.
- Resource groups organize resources with a shared purpose or lifecycle.
- Tags provide useful metadata but do not enforce security.
- Budget alerts do not automatically stop Azure spending.
- Administrative identities require strong authentication protection.
- Cost and usage data may not appear immediately.
- Consistent naming improves administration and documentation.
- Azure Activity Log provides evidence of management operations.
- Every deployed resource requires an ownership and cleanup plan.

### Technical Takeaway

Azure Resource Manager organizes resources through scopes that include management groups, subscriptions, resource groups, and individual resources.

### Business Takeaway

Establishing cost visibility, ownership, and organizational standards early reduces financial and operational risk.

### Security Takeaway

The identity controlling an Azure subscription must be protected because account compromise can expose resources, permissions, governance settings, and billing information.

### Exam Takeaway

For AZ-900, remember:

- Subscriptions are billing and access boundaries.
- Resource groups organize related resources.
- Tags provide metadata.
- Cost Management provides analysis, budgets, and alerts.
- Budgets do not stop resources or enforce a hard spending cap.

---

## Cleanup

### Resources Retained

| Resource or Configuration | Reason |
|---|---|
| MRTG Azure subscription | Required for the remaining labs |
| Monthly budget | Required for ongoing cost monitoring |
| MRTG naming standard | Required for project consistency |
| MRTG tagging standard | Required for governance and cost tracking |
| `rg-mrtg-az900-lab01-centralus-001` | Retained as the foundational Lab 01 resource group |

### Resources Removed

No billable Azure workloads are created during this lab.

### Cleanup Validation

- [ ] No unexpected Azure resources are running
- [ ] No unattached disks exist
- [ ] No unused public IP addresses exist
- [ ] No premium services were unintentionally enabled
- [ ] The subscription budget remains active
- [ ] Cost Management was reviewed
- [ ] Sensitive registration information was not committed
- [ ] All screenshots were sanitized

---

## Outcome

This lab establishes the security, cost-management, naming, tagging, and resource-organization foundation for the MRTG Azure Fundamentals series.

After completion, the environment will include:

- A protected MRTG cloud-operations account
- An active Azure subscription
- A standardized subscription name
- Subscription-level cost visibility
- A `$10.00` monthly budget
- Defined alert thresholds
- A documented naming convention
- A documented tagging standard
- A governed Azure resource group
- An initial administrative audit trail
- A verified zero-workload cost baseline

---

## Next Lab

The next lab is:

```text
Lab 02 - Cloud Computing and Shared Responsibility
```

The next lab will build on this foundation by examining:

- Cloud computing concepts
- The shared-responsibility model
- Consumption-based pricing
- Serverless computing
- Customer and provider responsibilities across cloud service models
