# AZ-900 Lab 06 - Explore Azure Monitor and Monitoring Services

## Lab Overview

Azure Monitor is Microsoft's centralized monitoring platform for collecting, analyzing, and responding to telemetry from Azure resources and hybrid environments. In this lab, I explored Azure Monitor's core services through Microsoft Learn and the Azure portal, gaining an understanding of how Azure provides visibility into resource health, performance, availability, and operational insights.

This lab focused on the monitoring services that form the foundation of Azure operations, including Azure Monitor, Metrics, Logs, Log Analytics, Alerts, Application Insights, Service Health, Resource Health, and Azure Advisor.

---

## Lab Objectives

- Understand the purpose of Azure Monitor.
- Learn the differences between Metrics and Logs.
- Explore Log Analytics workspaces.
- Review Azure Monitor Alerts.
- Examine Application Insights.
- Understand Azure Service Health.
- Explore Azure Resource Health.
- Review Azure Advisor recommendations.
- Navigate the Azure Monitor experience inside the Azure portal.

---

## Technologies Used

- Microsoft Azure
- Azure Monitor
- Azure Monitor Metrics
- Azure Monitor Logs
- Log Analytics Workspace
- Azure Monitor Alerts
- Application Insights
- Azure Service Health
- Azure Resource Health
- Azure Advisor
- Microsoft Learn

---

# Exercise 1 - Learn Azure Monitor Fundamentals

## Azure Monitor Overview

Azure Monitor collects telemetry from Azure resources, operating systems, applications, and hybrid environments. It centralizes monitoring data into a single platform where administrators can visualize, analyze, and respond to operational events.

**Key concepts learned:**

- Unified monitoring platform
- Metrics and Logs
- Dashboards and Workbooks
- Alerts
- Log Analytics
- Integration with Microsoft Defender for Cloud and Microsoft Sentinel

![Azure Monitor Overview](screenshots/01-azure-monitor-overview.png)

---

## Azure Monitor Metrics

Azure Monitor Metrics stores numerical performance data as time-series information.

Examples include:

- CPU utilization
- Memory usage
- Network throughput
- Disk operations

Metrics provide near real-time monitoring and are commonly used for dashboards and alerting.

![Azure Monitor Metrics Overview](screenshots/02-azure-monitor-metrics-overview.png)

---

## Azure Monitor Logs

Azure Monitor Logs stores detailed operational and diagnostic information.

Unlike Metrics, Logs support advanced searching using Kusto Query Language (KQL) and allow administrators to investigate events in much greater detail.

Logs support:

- Troubleshooting
- Security investigations
- Operational reporting
- Historical analysis

![Azure Monitor Logs Overview](screenshots/03-azure-monitor-logs-overview.png)

---

## Log Analytics Workspace

A Log Analytics Workspace serves as the central repository for Azure Monitor Logs.

Capabilities include:

- Centralized log storage
- Data retention management
- Access control
- Saved queries
- Dashboards
- Alert integration

![Log Analytics Workspace](screenshots/04-log-analytics-overview.png)

---

## Azure Monitor Alerts

Azure Monitor Alerts automatically notify administrators when predefined conditions are met.

Alert rules consist of:

- Scope
- Signal
- Condition
- Action Group

Alerts can be triggered using both Metrics and Logs.

![Azure Monitor Alerts](screenshots/05-azure-monitor-alerts-overview.png)

---

## Application Insights

Application Insights provides monitoring for web applications and services.

It helps administrators understand:

- Application availability
- Performance
- Exceptions
- User behavior
- Dependency tracking

Application Insights stores its telemetry inside Azure Monitor Logs.

![Application Insights](screenshots/06-application-insights-overview.png)

---

## Azure Service Health

Azure Service Health provides visibility into Microsoft service outages and maintenance events affecting Azure services.

It includes:

- Service Issues
- Planned Maintenance
- Health Advisories
- Security Advisories

![Azure Service Health](screenshots/07-azure-service-health-overview.png)

---

## Azure Resource Health

Resource Health focuses on the health of individual Azure resources.

It helps determine whether a problem originates from:

- Microsoft infrastructure
- Customer configuration
- Planned maintenance

![Azure Resource Health](screenshots/08-azure-resource-health-overview.png)

---

## Azure Advisor

Azure Advisor continuously analyzes Azure environments and recommends improvements across multiple categories.

Recommendation areas include:

- Cost Optimization
- Security
- Reliability
- Operational Excellence
- Performance

![Azure Advisor Overview](screenshots/09-azure-advisor-overview.png)

---

# Exercise 2 - Explore Azure Monitor in the Azure Portal

## Azure Monitor Overview

I opened Azure Monitor within the Azure portal to review its centralized monitoring dashboard and available monitoring services.

![Azure Monitor Portal](screenshots/10-azure-monitor-portal.png)

---

## Metrics

The Metrics blade allows administrators to visualize performance metrics from Azure resources and build charts for ongoing monitoring.

![Azure Monitor Metrics Portal](screenshots/11-azure-monitor-metrics-portal.png)

---

## Logs

The Logs experience provides access to Log Analytics and Kusto Query Language (KQL) for querying collected monitoring data.

Since no monitored resources had been deployed yet, the workspace contained no telemetry.

![Azure Monitor Logs Portal](screenshots/12-azure-monitor-logs-portal.png)

---

## Alerts

The Alerts dashboard showed no active alerts because the environment currently contains no monitored workloads.

This demonstrates the monitoring interface before production resources are deployed.

![Azure Monitor Alerts Portal](screenshots/13-azure-monitor-alerts-portal.png)

---

## Service Health

Azure Service Health confirmed there were currently no active Azure service incidents affecting the subscription.

![Azure Service Health Portal](screenshots/14-azure-service-health-portal.png)

---

## Resource Health

Resource Health showed no available resource health information because no Azure resources had been created beyond foundational configuration.

![Azure Resource Health Portal](screenshots/15-azure-resource-health-portal.png)

---

## Azure Advisor

Azure Advisor analyzed the subscription and displayed recommendations across multiple best practice categories.

Even within a new subscription, Advisor begins identifying opportunities to improve security and governance.

![Azure Advisor Portal](screenshots/16-azure-advisor-portal.png)

---

## Advisor Recommendations

The Advisor Recommendations page displayed several security-related recommendations, illustrating how Azure continuously evaluates subscriptions against Microsoft best practices.

These recommendations become increasingly valuable as cloud environments grow.

![Advisor Recommendations](screenshots/17-advisor-recommendations-portal.png)

---

# Key Takeaways

During this lab I learned:

- Azure Monitor serves as Microsoft's centralized monitoring platform.
- Metrics provide near real-time numerical performance data.
- Logs provide detailed searchable operational data using KQL.
- Log Analytics workspaces centralize monitoring data.
- Azure Alerts automate operational response.
- Application Insights extends Azure Monitor for application telemetry.
- Service Health tracks Azure-wide service events.
- Resource Health focuses on individual Azure resources.
- Azure Advisor continuously recommends improvements for cost, security, reliability, performance, and operational excellence.

---

# Skills Gained

- Azure monitoring fundamentals
- Azure operational visibility
- Metrics vs Logs
- Log Analytics concepts
- Monitoring architecture
- Azure troubleshooting fundamentals
- Azure governance awareness
- Azure operational best practices

---

## Repository Structure

```text
AZ-900-Lab-06/
│
├── README.md
└── screenshots/
    ├── 01-azure-monitor-overview.png
    ├── 02-azure-monitor-metrics-overview.png
    ├── 03-azure-monitor-logs-overview.png
    ├── 04-log-analytics-overview.png
    ├── 05-azure-monitor-alerts-overview.png
    ├── 06-application-insights-overview.png
    ├── 07-azure-service-health-overview.png
    ├── 08-azure-resource-health-overview.png
    ├── 09-azure-advisor-overview.png
    ├── 10-azure-monitor-portal.png
    ├── 11-azure-monitor-metrics-portal.png
    ├── 12-azure-monitor-logs-portal.png
    ├── 13-azure-monitor-alerts-portal.png
    ├── 14-azure-service-health-portal.png
    ├── 15-azure-resource-health-portal.png
    ├── 16-azure-advisor-portal.png
    └── 17-advisor-recommendations-portal.png
```

---

## Conclusion

This lab introduced Azure's monitoring ecosystem and demonstrated how Microsoft provides centralized visibility into cloud resources through Azure Monitor. Understanding Metrics, Logs, Alerts, Service Health, Resource Health, Application Insights, and Azure Advisor establishes a strong operational foundation that will support future labs involving virtual machines, networking, storage, identity, and cloud security.
