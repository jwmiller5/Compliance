---
title: System and Organization Controls (SOC) 3
description: Learn how Microsoft cloud services comply with System and Organization Controls (SOC) 3 standards for operational security.
keywords: Microsoft 365, compliance, offerings
localization_priority: Priority
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmazz
manager: laurawi
audience: itpro
ms.collection:
- M365-security-compliance
- MS-Compliance
hideEdit: true
titleSuffix: Microsoft Compliance
---

# System and Organization Controls (SOC) 3

## SOC 3 overview

System and Organization Controls (SOC) for Service Organizations are internal control reports created by the American Institute of Certified Public Accountants (AICPA). They are intended to examine services provided by a service organization so that end users can assess and address the risk associated with an outsourced service.

*SOC 3 SOC for Service Organizations: Trust Services Criteria for General Use Report* is a short, publicly facing version of the SOC 2 Type 2 attestation report for users who need assurances about service organization's controls relevant to Security, Availability, Processing Integrity, Confidentiality, or Privacy but do not need a full SOC 2 report. Because SOC 3 reports are general use reports, they can be freely distributed.

A SOC 3 report contains a written assertion by service organization management regarding control effectiveness to achieve commitments based on the applicable trust services criteria, as well as service auditor's opinion on whether management's assertion is stated fairly.

## Microsoft in-scope cloud platforms & services

Microsoft in-scope services are shown in the Azure [SOC 2 Type 2 attestation](offering-soc-2.md) report.

- Azure (for detailed insight, see [Microsoft Azure Compliance Offerings](https://azure.microsoft.com/resources/microsoft-azure-compliance-offerings/) or Azure SOC 2 Type 2 attestation report)
- Dynamics 365 (for detailed insight, see Azure SOC 2 Type 2 attestation report)
- Microsoft 365 Defender
- Microsoft Cloud App Security (MCAS)
- Microsoft Defender for Endpoint
- Microsoft Defender for Identity
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

## Azure, Dynamics 365, and SOC 3

For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure SOC 3 offering](/azure/compliance/offerings/offering-soc-3).

## Office 365 and SOC 3

### Office 365 cloud environments

Microsoft Office 365 is a multi-tenant hyperscale cloud platform and an integrated experience of apps and services available to customers in several regions worldwide. Most Office 365 services enable customers to specify the region where their customer data is located. Microsoft may replicate customer data to other regions within the same geographic area (for example, the United States) for data resiliency, but Microsoft will not replicate customer data outside the chosen geographic area.

This section covers the following Office 365 cloud environments:

- **Office 365**: the commercial public Office 365 cloud service available globally.
- **Office 365 Government Community Cloud (GCC)**: the [Office 365 GCC cloud service](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/gcc) is available for United States Federal, State, Local, and Tribal governments, as well as contractors holding or processing data on behalf of the US Government.
- **Office 365 Government Community Cloud - High (GCC High)**: the [Office 365 GCC High cloud service](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/gcc-high-and-dod) is designed according to Department of Defense (DoD) Security Requirements Guidelines Level 4 controls and supports strictly regulated federal and defense information. This environment is used by federal agencies, the Defense Industrial Base (DIBs), and government contractors.
- **Office 365 DoD (DoD)**: the [Office 365 DoD cloud service](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/gcc-high-and-dod) is designed according to DoD Security Requirements Guidelines Level 5 controls and supports strict federal and defense regulations. This environment is for the exclusive use by the US Department of Defense.

Use this section to help meet your compliance obligations across regulated industries and global markets. To find out which services are available in which regions, see the [International availability information](https://products.office.com/business/international-availability) and the [Where your Microsoft 365 customer data is stored](/microsoft-365/enterprise/o365-data-locations) article. For more information about Office 365 Government cloud environment, see the [Office 365 Government Cloud](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government) article.

Your organization is wholly responsible for ensuring compliance with all applicable laws and regulations. Information provided in this section does not constitute legal advice and you should consult legal advisors for any questions regarding regulatory compliance for your organization.

### Office 365 applicability and in-scope services

Use the following table to determine applicability for your Office 365 services and subscription:

| **Applicability** | **In-scope services** |
|:------------------|:----------------------|
| **Office 365** | Compliance Manager, Customer Lockbox, Delve, Exchange Online Protection, Exchange Online, Forms, Griffin, Identity Manager, Lockbox (Torus), Microsoft Teams, MyAnalytics, Office 365 Customer Portal, Office 365 Microservices (including but not limited to Kaizala, ObjectStore, Sway, PowerPoint Online Document Service, Query Annotation Service, School Data Sync, Siphon, Speech, StaffHub, eXtensible Application Program), Office Online, Office Services Infrastructure, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, Project Online, Service Encryption with Customer Key, SharePoint Online, Skype for Business |
| **GCC** | Azure Active Directory, Compliance Manager, Delve, Exchange Online, 
, Microsoft Defender for Office 365, Microsoft Teams, MyAnalytics, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business, Stream |
| **GCC High** | Azure Active Directory, Exchange Online, Flow, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business |
| **DoD** | Azure Active Directory, Exchange Online, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, Power Automate, Power BI, SharePoint Online, Skype for Business |

### Office 365 audit reports

- [Office 365 Core - SSAE 18 SOC 3 Report](https://aka.ms/o365SOC-3)
- [See bridge letters and additional audit reports](https://aka.ms/auditreports)

You must have an existing subscription or free trial account in Office 365 or Office 365 U.S. Government to download SOC 1 and SOC 2 attestation reports and any bridge letters as needed.

### Frequently asked questions

**How often are Office 365 SOC reports issued?**

SOC reports for Office 365 and other online services are based on a rolling 12-month run window (audit period) with new reports issued semi-annually (period ends are March 31 and September 30). *Bridge letters* are issued each quarter to cover the prior three-month period. For example, the January letter covers 1-Oct through 31-Dec, the April letter covers 1-Jan through 31-Mar, the July letter covers 1-Apr through 30-Jun, and the October letter covers 1-Jul through 30-Sep.

**Where can I get the Office 365 SOC audit documentation including bridge letters?** For links to audit documentation, see the audit report section. You must have an existing subscription or free trial account in Office 365or [Office](https://azure.microsoft.com/global-infrastructure/government/request/) 365 U.S. Government to login. You can then download audit certificates, assessment reports, and other applicable documents to help you with your own regulatory requirements.

### Use Microsoft Compliance Manager to assess your risk

[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft 365 compliance center](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks. Compliance Manager offers a premium template for building an assessment for this regulation. Find the template in the **assessment templates** page in Compliance Manager. Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).

### Office 365 resources

- [Service Trust Portal audit reports](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3)
- [AICPA SOC for Service Organizations](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/socforserviceorganizations.html)
- [SSAE No. 18, Attestation Standards: Clarification and Recodification (AICPA Professional Standards)](https://www.aicpa.org/Research/Standards/AuditAttest/DownloadableDocuments/SSAE_No_18.pdf)
- [SOC 2 Reporting on an Examination of Controls at a Service Organization Relevant to Security, Availability, Processing Integrity, Confidentiality, or Privacy (AICPA Guide)](https://future.aicpa.org/cpe-learning/publication/soc-2-reporting-on-an-examination-of-controls-at-a-service-organization-relevant-to-security-availability-processing-integrity-confidentiality-or-privacy-OPL) (available for purchase)
- [TSP section 100 (AICPA, 2017 Trust Services Criteria)](https://www.aicpa.org/content/dam/aicpa/interestareas/frc/assuranceadvisoryservices/downloadabledocuments/trust-services-criteria.pdf)
