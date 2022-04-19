---
title: System and Organization Controls (SOC) 1 Type 2
description: Learn how Microsoft cloud services comply with System and Organization Controls (SOC) 1 Type 2 standards for operational security.
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

# System and Organization Controls (SOC) 1 Type 2

## SOC 1 Type 2 overview

System and Organization Controls (SOC) for Service Organizations are internal control reports created by the American Institute of Certified Public Accountants (AICPA). They are intended to examine services provided by a service organization so that end users can assess and address the risk associated with an outsourced service.

A SOC 1 Type 2 attestation is performed under:

- SSAE No. 18, Attestation Standards: Clarification and Recodification, which includes AT-C section 320, *Reporting on an Examination of Controls at a Service Organization Relevant to User Entities' Internal Control Over Financial Reporting* (AICPA, Professional Standards).
- SOC 1 Reporting on an Examination of Controls at a Service Organization Relevant to User Entities' Internal Control Over Financial Reporting (AICPA Guide).

Aside from the AICPA Statement on Standards for Attestation Engagements 18 (SSAE 18), the Office 365 SOC 1 Type 2 audit is conducted in accordance with the International Standard on Assurance Engagements No. 3402 (ISAE 3402). The SOC 1 attestation has replaced SAS 70, and it is appropriate for reporting on controls at a service organization relevant to user entities internal controls over financial reporting. A Type 2 report includes auditor's opinion on the control effectiveness to achieve the related control objectives during the specified monitoring period.

## Microsoft in-scope cloud platforms & services

Microsoft online services in scope are shown in the Azure SOC 1 Type 2 attestation report:

- Azure (for detailed insight, see [Microsoft Azure Compliance Offerings](https://azure.microsoft.com/resources/microsoft-azure-compliance-offerings/) or Azure SOC 1 Type 2 attestation report)
- Azure DevOps (see separate Azure DevOps SOC 1 Type 2 attestation report)
- Dynamics 365 (for detailed insight, see Azure SOC 1 Type 2 attestation report)
- Microsoft 365 Defender
- Microsoft Defender for Cloud Apps
- Microsoft Defender for Endpoint (formerly Microsoft Defender Advanced Threat Protection)
- Microsoft Defender for Identity (formerly Azure Advanced Threat Protection)
- Microsoft Forms Pro (not in scope for Azure Government)
- Microsoft Graph
- Microsoft Intune
- Microsoft Managed Desktop (not in scope for Azure Government)
- Microsoft Stream
- Microsoft Threat Experts (not in scope for Azure Government)
- Nomination Portal
- Office 365, Office 365 U.S. Government, Office 365 U.S. Government - High, Office 365 U.S. Government Defense
- Power Apps
- Power Automate
- Power BI
- Power Virtual Agents (not in scope for Azure Government)
- Update Compliance (not in scope for Azure Government)

## Azure, Dynamics 365, and SOC 1

For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure SOC 1 offering](/azure/compliance/offerings/offering-soc-1).

## Office 365 and SOC 1

### Office 365 environments

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### Office 365 applicability and in-scope services

Use the following table to determine applicability for your Office 365 services and subscription:

| **Applicability** | **In-scope services** |
|:------------------|:----------------------|
| **Commercial** | Compliance Manager, Customer Lockbox, Delve, Exchange Online Protection, Exchange Online, Forms, Griffin, Identity Manager, Lockbox (Torus), Microsoft Teams, MyAnalytics, Office 365 Customer Portal, Office 365 Microservices (including but not limited to Kaizala, ObjectStore, Sway, PowerPoint Online Document Service, Query Annotation Service, School Data Sync, Siphon, Speech, StaffHub, eXtensible Application Program), Office Online, Office Services Infrastructure, OneDrive for Business, Planner, PowerApps, Power BI, Project Online, Service Encryption with Microsoft Purview Customer Key, SharePoint Online, Skype for Business |
| **GCC** | Azure Active Directory, Compliance Manager, Delve, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, MyAnalytics, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business, Stream |
| **GCC High** | Azure Active Directory, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power  BI, SharePoint Online, Skype for Business |
| **DoD** | Azure Active Directory, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, Power BI, SharePoint Online, Skype for Business |

### Office 365 audit reports

- [Office 365 Core - SSAE 18 SOC 1 Report](https://aka.ms/o365SOC-1)
- See bridge letters and additional audit reports

You must have an existing subscription or free trial account in Office 365 or Office 365 U.S. Government to download SOC 1 and SOC 2 attestation reports and any bridge letters as needed.

### Frequently asked questions

**How often are Office 365 SOC reports issued?**

SOC reports for Office 365 and are issued semi-annually. SOC audits for core and micro-services are based on a rolling 12-month run window (audit period) with new reports issued annually for the period 1-October through 30-September of the next calendar year. SOC audit reports are also issued in the spring for new services coming into scope for Office 365. *Bridge letters* are issued at the end of each audit quarter to cover the prior three-month period. For example, bridge letters are typically issued in December, March, June, and September.

**How can customers benefit from Office 365 SOC 1 Type 2 attestation?**

Customers can use the Office 365 SOC 1 Type 2 attestation when pursuing their own financial industry-specific compliance requirements such as Sarbanes-Oxley (SOX), Federal Financial Institutions Examination Council (FFIEC), Gramm-Leach-Bliley Act (GLBA), and others.

**Where can I get the Office 365 SOC audit documentation including bridge letters?**

For links to audit documentation, see the audit report section. You must have an existing subscription or free trial account in Office 365 or Office 365 U.S. Government to log in. You can then download audit certificates, assessment reports, and other applicable documents to help you with your own regulatory requirements.

**Where can I see management responses to exceptions noted?**

Management responses are located towards the end of the SOC attestation report. Search the document for 'Management Response'.

**Where can I see user entity responsibilities?**

User entity responsibilities are located at the very end of the SOC attestation report. Search the document for 'User Entity Responsibilities'.

### Use Microsoft Purview Compliance Manager to assess your risk

[Microsoft Purview Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft Purview compliance portal](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks. Compliance Manager offers a premium template for building an assessment for this regulation. Find the template in the **assessment templates** page in Compliance Manager. Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).

### Resources

- [Service Trust Portal audit reports](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3)
- [SSAE No. 18, Attestation Standards: Clarification and Recodification](https://www.aicpa.org/Research/Standards/AuditAttest/DownloadableDocuments/SSAE_No_18.pdf)
- [SOC 1 Reporting on an Examination of Controls at a Service Organization Relevant to User Entities' Internal Control Over Financial Reporting (AICPA Guide)](https://future.aicpa.org/cpe-learning/publication/reporting-on-an-examination-of-controls-at-a-service-organization-relevant-to-user-entities-internal-control-over-financial-reporting-soc-1-guide-OPL) (available for purchase)
