---
title: Department of Defense (DoD) Impact Level 2 (IL2)
description: Learn how Microsoft meets Department of Defense (DoD) Impact Level 2 (IL2) standards.
keywords: Microsoft 365, compliance, offerings
localization_priority: None
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

# Department of Defense (DoD) Impact Level 2 (IL2)

## DoD IL2 overview

The Defense Information Systems Agency (DISA) is an agency of the US Department of Defense (DoD) that is responsible for developing and maintaining the DoD Cloud Computing [Security Requirements Guide (SRG)](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html). The SRG defines the baseline security requirements used by DoD to assess the security posture of a cloud service provider (CSP), supporting the decision to grant a DoD Provisional Authorization (PA) that allows a CSP to host DoD missions. It incorporates, supersedes, and rescinds the previously published DoD Cloud Security Model (CSM) and maps to the DoD Risk Management Framework (RMF).

DISA guides DoD agencies and departments in planning and authorizing the use of a CSP. It also evaluates CSP offerings for compliance with the SRG — an authorization process whereby CSPs can furnish documentation outlining their compliance with DoD standards. It issues DoD Provisional Authorizations (PAs) when appropriate, so DoD agencies and supporting organizations can use cloud services without having to go through a full approval process on their own, saving time and effort.

The [15 December 2014 DoD CIO memo](https://www.esi.mil/contentview.aspx?id=585) regarding *Updated Guidance on the Acquisition and Use of Commercial Cloud Computing Services* states that 'FedRAMP will serve as the minimum security baseline for all DoD cloud services'. The SRG uses the FedRAMP Moderate baseline at all information impact levels (IL) and considers the High Baseline at some.

[SRG Section 5.1.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD use of FedRAMP Security Controls* states that IL2 information may be hosted in a CSP that minimally holds a FedRAMP Moderate PA and a DoD Level 2 PA, subject to compliance with the personnel security requirements outlined in Section 5.6.2. However, this approach does not alleviate the CSP from meeting other security and integration requirements as required by the Mission Owner. According to [SRG Section 5.2.2.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5.2LegalConsiderations) *IL2 Location and Separation Requirements*, DoD IL2 PA is adequately covered by a FedRAMP Moderate PA such that the requirements will not be additionally assessed for an IL2 PA.

## Microsoft in-scope cloud platforms & services

- Azure
- Dynamics 365
- Microsoft Cloud App Security
- Microsoft Defender for Endpoint
- Microsoft Graph
- Microsoft Intune
- Microsoft Stream
- Office 365 U.S. Government, Office 365 U.S. Government - High
- Power Apps
- Power Automate
- Power BI

## Azure, Dynamics 365, and DoD IL2

For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure DoD IL2 offering](/azure/compliance/offerings/offering-dod-il2).

## Office 365 and DoD IL2

### Office 365 cloud environments

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### Office 365 applicability and in-scope services

Use the following table to determine applicability for your Office 365 services and subscription:

| **Applicability** | **In-scope services** |
|:------------------|:----------------------|
| **GCC** | Activity Feed Service, Bing Services, Delve, Exchange Online Protection, Exchange Online, Intelligent Services, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, SharePoint Online, Skype for Business, Windows Ink |
| **GCC High** | Activity Feed Service, Bing Services, Delve, Exchange Online Protection, Exchange Online, Intelligent Services, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, SharePoint Online, Skype for Business, Windows Ink |

### Resources

- [Microsoft government solutions](https://www.microsoft.com/enterprise/government)
- [DoD Cloud Computing Security Requirements Guide](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)
- [FedRAMP documents](https://www.fedramp.gov/documents/)
- [NIST SP 800-37](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) *Risk Management Framework for Information Systems and Organizations: A System Life Cycle Approach for Security and Privacy*
- [NIST SP 800-53](https://csrc.nist.gov/Projects/risk-management/sp800-53-controls/release-search#!/800-53) *Security and Privacy Controls for Information Systems and Organizations*
- [DoD Instruction 8510.01](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodi/851001p.pdf) *DoD Risk Management Framework (RMF) for DoD Information Technology (IT)*
