---
title: "Microsoft security incident management"
description: "This article, provides an overview of the security incident management process in Microsoft online services."
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: Normal
search.appverid:
- MET150
f1.keywords:
- NOCSH
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
titleSuffix: Microsoft Service Assurance
hideEdit: true
---

# Microsoft security incident management

Microsoft works continuously to provide highly secure, enterprise-grade services for Microsoft customers, but security incidents are an inevitable reality that must be thoroughly and swiftly managed. This document provides an overview on how Microsoft handles security incidents using tried and true methods and technologies to minimize their potential impact. A security incident refers to any unlawful access to customer data stored on Microsoft's equipment or in Microsoft's facilities, or unauthorized access to such equipment or facilities that have the potential to result in the loss, disclosure, or alteration of customer data. Microsoft's goals when responding to security incidents are to protect customer data and Microsoft's online services.

Microsoft online services security teams and the various service teams work jointly and take the same approach to security incidents:

- Preparation
- Detection and Analysis
- Containment, Eradication, and Recovery
- Post-Incident Activity

## Microsoft approach to security incident management

Microsoft's approach to managing a security incident conforms to [National Institute of Standards and Technology (NIST)](https://www.nist.gov/) Special Publication (SP) 800-61. Microsoft has several dedicated teams that work together to prevent, monitor, detect, and respond to security incidents.

|**Team/Area**|**Description**|
|:------------|:--------------|
| Microsoft Security Response Center | Identifies, monitors, resolves, and responds to security incidents and Microsoft software security vulnerabilities. |
| Cyber Defense Operations Center | The Cyber Defense Operations Center is the physical location that brings together security response teams and experts from across the company to help protect, detect, and respond to threats in real time. |
| Corporate, External, and Legal Affairs | Provides legal and regulatory advice for a suspected security incident. |
| Microsoft Datacenter Security Team | Team that focuses across the various services on common security engineering investments to protect, detect, and respond to service architecture risks and threats. |
| Microsoft security response teams | Independent Azure, Dynamics 365, and Microsoft 365 security teams that partner with service teams to build the appropriate security incident management process and to drive any security incident response. |
| Microsoft Governance, Risk, and Compliance (GRC) teams | Provide guidance on regulatory requirements, compliance, and privacy. |
| Service teams | Engineering teams for Azure, Dynamics 365, Microsoft 365 that are responsible for security-related policies and decisions for each service. |
| Azure operations managers | Oversees the investigation and resolution of Azure-related security and privacy incidents. |
| Microsoft Threat Intelligence Center (MSTIC) | Provides the current state of art in digital security threats against Microsoft infrastructure and assets, helps partner teams inside Microsoft prioritize mitigation and prevention effort action plans, and increases protection by adopting near real-time incident monitoring/detection. |
| Customer experience communication teams | Engineering teams responsible for all customer communications about security and service incidents. Separate teams are dedicated to Azure, Dynamics 365, and Microsoft 365. |

## Response management process

Microsoft online services security teams and service teams work together on and take the same approach to security incidents, which is based on the NIST 800-61 response management phases:

- **Preparation**: Refers to the organizational preparation that is needed to be able to respond, including tools, processes, competencies, and readiness.
- **Detection & analysis**: Refers to the activity to detect a security incident in a production environment and to analyze all events to confirm the authenticity of the security incident.
- **Containment, eradication, recovery**: Refers to the required and appropriate actions taken to contain the security incident based on the analysis done in the previous phase. More analysis may also be necessary in this phase to fully recovery from the security incident.
- **Post-incident activity**: Refers to the post-mortem analysis performed after the recovery of a security incident. The operational actions performed during the process are reviewed to determine if any changes need to be made in the preparation or detection and analysis phases.

![Security incident management phases](../media/assurance-sim-phases.png)

## Federated security response model

Microsoft online services consist of core Microsoft products, including Azure, Dynamics 365, and Microsoft 365. Each of these services are operated by separate teams with their own security operational processes. Other teams at Microsoft, such as MSTIC, are also engaged in various security aspects of Microsoft online services. Because of the multitude of teams working on security operations management across all the various services that make up Microsoft online services, Microsoft has implemented a federated security response model.

This table presents the operational boundaries between the various Microsoft online service security operations teams and the Microsoft service teams:

|**Activity**|**Microsoft Security Team Operations**|**Microsoft Service Team Operations**|
|:-----------|:-----------------------------------------|:----------------------------------------|
| Detection and analysis | - Detection requirements <br> - Security monitoring and analysis <br> - Indicator of compromise (IOC) sweeps <br> - Breach hunt <br> - 24x7 security on-call and incident response lead | - Detection requirements <br> - Monitoring infrastructure deployment <br> - Service analysis and insight <br> - Event and alert triage <br> - 24x7 service engineering on-call  |
| Containment, eradication, recovery | - Incident response lead <br> - Forensics investigation <br> - Security expertise and consulting <br> - Recovery guidance | - Security incident owner <br> - Service insight and expertise <br> - Execute containment, eradication, and recovery |
| Post-incident activity | - Post-incident analysis lead <br> - Data collection and archival <br> - Lessons learned and bug requests <br> - Incident reporting | - Service-side incident analysis <br> - Prioritize follow-up activities <br> - Implementation security investments <br> - Service security readiness |

## Related articles

- [Microsoft security incident management: Preparation](assurance-sim-preparation.md)
- [Microsoft security incident management: Detection and analysis](assurance-sim-detection-analysis.md)
- [Microsoft security incident management: Containment, eradication, and recovery](assurance-sim-containment-eradication-recovery.md)
- [Microsoft security incident management: Post-incident activity](assurance-sim-post-incident-activity.md)
