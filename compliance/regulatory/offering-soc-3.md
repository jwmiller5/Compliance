---
title: System and Organization Controls (SOC) 3
description: Learn how Microsoft cloud services comply with System and Organization Controls (SOC) 3 standards for operational security.
keywords: Microsoft 365, compliance, offerings
ms.localizationpriority: high
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmazz
manager: laurawi
audience: itpro
ms.collection:
- MS-Compliance
- MS-Compliance-Offering
hideEdit: true
titleSuffix: Microsoft Compliance
---

# System and Organization Controls (SOC) 3

## SOC 3 overview

System and Organization Controls (SOC) for Service Organizations are internal control reports created by the American Institute of Certified Public Accountants (AICPA). They're intended to examine services provided by a service organization so that end users can assess and address the risk associated with an outsourced service.

*SOC 3 for Service Organizations: Trust Services Criteria for General Use Report* is a short, publicly facing summary of the SOC 2 Type 2 attestation report for users who need assurances about service organization's controls but don't need a full SOC 2 report or aren't eligible under SOC 2 to receive one. Because SOC 3 reports are general use reports, they can be freely distributed.

A SOC 3 report contains a written assertion by service organization management regarding control effectiveness to achieve commitments based on the applicable trust services criteria, and service auditor's opinion on whether management's assertion is stated fairly.

## Microsoft in-scope cloud platforms & services

Microsoft in-scope services are shown in the Azure [SOC 2 Type 2 attestation](offering-soc-2.md) report.

- Azure (for detailed insight, see [Microsoft Azure Compliance Offerings](https://azure.microsoft.com/resources/microsoft-azure-compliance-offerings/) or Azure SOC 2 Type 2 attestation report)
- Dynamics 365 (for detailed insight, see Azure SOC 2 Type 2 attestation report)
- Microsoft 365 Defender
- Microsoft Defender for Cloud Apps
- Microsoft Defender for Endpoint
- Microsoft Defender for Identity
- Microsoft Forms Pro
- Microsoft Intune
- Microsoft Managed Desktop
- Microsoft Stream
- Microsoft Threat Experts
- Nomination Portal
- Office 365, Office 365 U.S. Government, Office 365 U.S. Government - High, Office 365 U.S. Government Defense
- Power Apps
- Power Automate
- Power BI
- Power Virtual Agents
- Update Compliance

## Azure, Dynamics 365, and SOC 3

For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure SOC 3 offering](/azure/compliance/offerings/offering-soc-3).

## Office 365 and SOC 3

### Office 365 environments

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### Office 365 applicability and in-scope services

Use the following table to determine applicability for your Office 365 services and subscription:

| **Applicability** | **In-scope services** |
|:------------------|:----------------------|
| **Commercial** | Compliance Manager, Customer Lockbox, Delve, Exchange Online Protection, Exchange Online, Forms, Griffin, Identity Manager, Lockbox (Torus), Microsoft Teams, MyAnalytics, Office 365 Customer Portal, Office 365 Microservices (including but not limited to Kaizala, ObjectStore, Sway, PowerPoint Online Document Service, Query Annotation Service, School Data Sync, Siphon, Speech, StaffHub, eXtensible Application Program), Office Online, Office Services Infrastructure, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, Project Online, Service Encryption with Microsoft Purview Customer Key, SharePoint Online, Skype for Business |
| **GCC** | Azure Active Directory, Compliance Manager, Delve, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, MyAnalytics, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business, Stream |
| **GCC High** | Azure Active Directory, Exchange Online, Flow, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business |
| **DoD** | Azure Active Directory, Exchange Online, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, Power Automate, Power BI, SharePoint Online, Skype for Business |

### Office 365 audit reports

- [Office 365 Core - SSAE 18 SOC 3 Report](https://aka.ms/o365SOC-3)
- [See bridge letters and additional audit reports](https://aka.ms/auditreports)

You must have an existing subscription or free trial account in Office 365 or Office 365 U.S. Government to download SOC 1 and SOC 2 attestation reports and any bridge letters as needed.

### Frequently asked questions

**How often are Office 365 SOC reports issued?**

Microsoft commissions a full SOC 1 Type 2 and SOC 2 Type 2 examination of Office 365 annually. The auditor's reports on these examinations (also known as audits) are issued as soon as they're ready after that audit. The SOC 3 report, which is based on the SOC 2 examination, is issued at the same time.

Because Microsoft doesn't control the investigative scope of the examination nor the timeframe of the auditor's completion, there's no set timeframe when these reports are issued. The reports are usually issued a few months after the end of the period under examination. Microsoft doesn't allow any gaps in the consecutive periods of examination from one examination to the next.

Microsoft also commissions a mid-year SOC 1 Type 1 and SOC 2 Type 1 examination of Office 365 for new Microsoft services that have been issued since the last SOC Type 2 audit. Type 1 audits don't look back over a period of performance.

Due to the sophisticated nature of Office 365, the service scope is large if examined as a whole. This can lead to examination completion delays due to scale. Microsoft organizes all the examinations described above into 2 categories: Core Services and Microservices. Microsoft issues reports scoped to each examination.

SOC Type 2 audits examine a rolling 12-month *run window* (also known as audit period or more formally *period of performance*) with examinations conducted annually for the period 1-October through 30-September of the next calendar year. The examination starts promptly after the period of performance is complete.  

Microsoft also issues bridge letters (also known as *gap letters*). These are self-attestations by Microsoft, not reports based on examinations by the auditor. Bridge letters are issued during the current period of performance that isn't yet complete and ready for audit examination. Microsoft  issues bridge letters at the end of each quarter to attest our performance during the prior three-month period. Due to the period of performance for the SOC type 2 audits, the bridge letters are typically issued in December, March, June, and September of the current operating period.

**Where can I get the Office 365 SOC audit documentation including Microsoft's bridge letters?**

For links to audit documentation, see the audit report section of the Service Trust Portal. You must have an existing subscription or free trial account in Office 365 or [Office](https://azure.microsoft.com/global-infrastructure/government/request/) 365 U.S. Government to log in. You can then download audit certificates, assessment reports, and other applicable documents to help you with your own regulatory requirements.

### Use Microsoft Purview Compliance Manager to assess your risk

[Microsoft Purview Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft Purview compliance portal](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks. Compliance Manager offers a premium template for building an assessment for this regulation. Find the template in the **assessment templates** page in Compliance Manager. Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).

### Resources

- [Service Trust Portal audit reports](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3)
- [AICPA SOC for Service Organizations](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/socforserviceorganizations.html)
- [SSAE No. 18, Attestation Standards: Clarification and Recodification (AICPA Professional Standards)](https://us.aicpa.org/research/standards/auditattest/ssae)
- [SOC 2 Reporting on an Examination of Controls at a Service Organization Relevant to Security, Availability, Processing Integrity, Confidentiality, or Privacy (AICPA Guide)](https://future.aicpa.org/cpe-learning/publication/soc-2-reporting-on-an-examination-of-controls-at-a-service-organization-relevant-to-security-availability-processing-integrity-confidentiality-or-privacy-OPL) (available for purchase)
- [TSP section 100 (AICPA, 2017 Trust Services Criteria)](https://www.aicpa.org/content/dam/aicpa/interestareas/frc/assuranceadvisoryservices/downloadabledocuments/trust-services-criteria.pdf)
