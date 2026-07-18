# AZ-900 Lab 12 - Azure Monitoring, Health, and Optimization

## Lab Overview

Azure provides a comprehensive set of monitoring, health, and optimization services that help administrators maintain visibility into cloud resources, troubleshoot issues, and improve operational efficiency. In this lab, I explored Azure Monitor through Microsoft Learn and the Azure portal to understand how Azure collects telemetry, analyzes operational data, monitors service health, and recommends improvements for cloud environments.

This lab focused on Azure Monitor, Metrics, Logs, Log Analytics, Alerts, Application Insights, Service Health, Resource Health, and Azure Advisor, providing a solid operational foundation for managing Azure workloads.

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
- Navigate Azure Monitor inside the Azure portal.

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

# Exercise 1 - Learn Azure Monitoring Fundamentals

## Azure Monitor Overview

Azure Monitor is Microsoft's centralized observability platform for collecting, analyzing, and responding to telemetry from Azure resources, applications, operating systems, and hybrid environments.

**Key concepts reviewed:**

- Unified monitoring platform
- Metrics
- Logs
- Dashboards
- Workbooks
- Alerts
- Integration with Microsoft Defender for Cloud
- Integration with Microsoft Sentinel

![Azure Monitor Overview](screenshots/01-azure-monitor-overview.png)

---

## Azure Monitor Metrics

Azure Monitor Metrics stores numerical performance information as time-series data, allowing administrators to monitor resource performance in near real time.

Examples include:

- CPU utilization
- Memory usage
- Network throughput
- Disk operations

Metrics are commonly used for dashboards, visualizations, and alerting.

![Azure Monitor Metrics Overview](screenshots/02-azure-monitor-metrics-overview.png)

---

## Azure Monitor Logs

Azure Monitor Logs stores detailed operational and diagnostic information for Azure resources.

Unlike Metrics, Logs support advanced searches using Kusto Query Language (KQL), making them valuable for troubleshooting, reporting, and security investigations.

Logs support:

- Troubleshooting
- Historical analysis
- Operational reporting
- Security investigations

![Azure Monitor Logs Overview](screenshots/03-azure-monitor-logs-overview.png)

---

## Log Analytics Workspace

A Log Analytics Workspace serves as the centralized repository for Azure Monitor Logs.

Capabilities include:

- Centralized log storage
- Data retention
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

Alerts can be created using both Metrics and Logs.

![Azure Monitor Alerts](screenshots/05-azure-monitor-alerts-overview.png)

---

## Application Insights

Application Insights extends Azure Monitor by providing application-level monitoring for web applications and services.

It provides visibility into:

- Application availability
- Performance
- Exceptions
- Dependencies
- User behavior

Telemetry collected by Application Insights is stored within Azure Monitor Logs.

![Application Insights](screenshots/06-application-insights-overview.png)

---

## Azure Service Health

Azure Service Health provides personalized visibility into Azure service outages, planned maintenance, health advisories, and security advisories that may affect Azure subscriptions.

Categories include:

- Service Issues
- Planned Maintenance
- Health Advisories
- Security Advisories

![Azure Service Health](screenshots/07-azure-service-health-overview.png)

---

## Azure Resource Health

Azure Resource Health reports the health status of individual Azure resources and helps determine whether issues originate from Microsoft infrastructure or customer configuration.

This information helps administrators quickly identify the source of outages and determine whether Service Level Agreements (SLAs) have been impacted.

![Azure Resource Health](screenshots/08-azure-resource-health-overview.png)

---

## Azure Advisor

Azure Advisor continuously evaluates Azure environments and provides recommendations to improve deployments across several best practice categories.

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

I opened Azure Monitor within the Azure portal to review Microsoft's centralized monitoring dashboard and available monitoring services.

![Azure Monitor Portal](screenshots/10-azure-monitor-portal.png)

---

## Metrics

The Metrics blade provides graphical visualization of Azure resource performance metrics.

Since no workloads had been deployed, no performance data was available to display.

![Azure Monitor Metrics Portal](screenshots/11-azure-monitor-metrics-portal.png)

---

## Logs

The Logs experience provides access to Log Analytics and Kusto Query Language (KQL) for querying monitoring data.

Because the environment contained no monitored resources, no telemetry data was available for querying.

![Azure Monitor Logs Portal](screenshots/12-azure-monitor-logs-portal.png)

---

## Alerts

The Alerts dashboard displayed no active alerts because the subscription currently contains no monitored production workloads.

This demonstrates the monitoring interface before alert rules are configured.

![Azure Monitor Alerts Portal](screenshots/13-azure-monitor-alerts-portal.png)

---

## Service Health

Azure Service Health confirmed there were no active Azure service incidents affecting the subscription during this lab.

![Azure Service Health Portal](screenshots/14-azure-service-health-portal.png)

---

## Resource Health

Resource Health displayed no available health information because no Azure resources had been deployed beyond the foundational subscription configuration.

![Azure Resource Health Portal](screenshots/15-azure-resource-health-portal.png)

---

## Azure Advisor

Azure Advisor evaluated the subscription and displayed recommendations across Microsoft's best practice categories.

Even a new subscription begins receiving recommendations designed to improve governance and security.

![Azure Advisor Portal](screenshots/16-azure-advisor-portal.png)

---

## Advisor Recommendations

The Advisor Recommendations page displayed several security-focused recommendations for improving the subscription's security posture.

As Azure environments grow, these recommendations become increasingly valuable for maintaining secure and well-governed deployments.

![Advisor Recommendations](screenshots/17-advisor-recommendations-portal.png)

---

# Key Takeaways

During this lab I learned:

- Azure Monitor is Microsoft's centralized monitoring platform.
- Metrics provide near real-time numerical performance data.
- Logs provide detailed searchable operational data using KQL.
- Log Analytics workspaces centralize monitoring data.
- Alerts automate operational response to issues.
- Application Insights extends Azure Monitor for application telemetry.
- Service Health monitors Azure-wide platform events.
- Resource Health focuses on the health of individual Azure resources.
- Azure Advisor continuously recommends improvements for cost, security, reliability, operational excellence, and performance.

---

# Skills Gained

- Azure Monitor fundamentals
- Azure operational monitoring
- Metrics vs. Logs
- Log Analytics concepts
- Azure troubleshooting fundamentals
- Azure operational visibility
- Azure health monitoring
- Azure Advisor recommendations
- Cloud monitoring best practices

---

## Repository Structure

```text
AZ-900-Lab-12/
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

This lab introduced Azure's monitoring, health, and optimization services and demonstrated how Azure Monitor serves as the foundation for operational visibility across cloud environments. Understanding Metrics, Logs, Log Analytics, Alerts, Application Insights, Service Health, Resource Health, and Azure Advisor provides the monitoring knowledge required to support future Azure deployments involving virtual machines, networking, storage, identity, governance, and cloud security.
