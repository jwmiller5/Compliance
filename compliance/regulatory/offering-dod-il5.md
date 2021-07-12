---
title: Department of Defense (DoD) Impact Level 5 (IL5)
description: Learn how Microsoft meets Department of Defense (DoD) Impact Level 5 (IL5) standards.
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

# Department of Defense (DoD) Impact Level 5 (IL5)

## DoD IL5 overview

The Defense Information Systems Agency (DISA) is an agency of the US Department of Defense (DoD) that is responsible for developing and maintaining the DoD Cloud Computing [Security Requirements Guide (SRG)](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html). The SRG defines the baseline security requirements used by DoD to assess the security posture of a cloud service provider (CSP), supporting the decision to grant a DoD Provisional Authorization (PA) that allows a CSP to host DoD missions. It incorporates, supersedes, and rescinds the previously published DoD Cloud Security Model (CSM) and maps to the DoD Risk Management Framework (RMF).

DISA guides DoD agencies and departments in planning and authorizing the use of a CSP. It also evaluates CSP offerings for compliance with the SRG, an authorization process whereby CSPs can furnish documentation outlining their compliance with DoD standards. It issues DoD Provisional Authorizations (PAs) when appropriate, so DoD agencies and supporting organizations can use cloud services without having to go through a full approval process on their own, saving time and effort.

According to [SRG Section 3.2](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#3.2InformationImpactLevels) *Information Impact Levels*, IL5 information covers:

- Controlled Unclassified Information (CUI) that requires higher level of protection than that afforded by IL4
    - The [CUI Registry](https://www.archives.gov/cui) provides specific categories of information that is under protection by the Executive branch, for example, more than 20 category groupings are included in the [CUI category list](https://www.archives.gov/cui/registry/category-list).
    - [NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final) *Protecting Controlled Unclassified Information in Nonfederal Systems and Organizations* is intended for use by federal agencies in contracts or other agreements established with non-federal organizations.

- National Security Systems (NSS)
    - [NIST SP 800-59](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-59.pdf) *Guideline for Identifying an Information System as a National Security System* provides definitions of NSS.
    - [CNSSI 1253](https://www.dcsa.mil/portals/91/documents/ctp/nao/CNSSI_No1253.pdf) *Security Categorization and Control Selection for National Security Systems* provides guidance on the security standards that federal agencies should apply to categorize national security information.

The [15 December 2014 DoD CIO memo](https://www.esi.mil/contentview.aspx?id=585) regarding *Updated Guidance on the Acquisition and Use of Commercial Cloud Computing Services* states that 'FedRAMP will serve as the minimum security baseline for all DoD cloud services'. The SRG uses the FedRAMP Moderate baseline at all information impact levels (IL) and considers the High Baseline at some.

[SRG Section 5.1.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD use of FedRAMP Security Controls* states that a FedRAMP High PA, supplemented with DoD FedRAMP+ controls and control enhancements (C/CEs) and requirements in the SRG, are used to assess CSPs toward awarding a DoD PA at IL5. No matter what C/CE baseline is used as the basis for a FedRAMP High PA, additional considerations and/or requirements will need to be assessed and approved before a DoD PA can be awarded at IL5. Specifically, [SRG Section 5.1.2](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD FedRAMP+ Security Controls/Enhancements* states in Table 2 that 10 additional C/CEs beyond the FedRAMP High baseline are required for a DoD IL5 PA.

Moreover, according to [SRG Section 5.2.2.3](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5.2LegalConsiderations) *IL5 Location and Separation Requirements*, the following requirements (among others) must be in place for a Level 5 PA:

- Virtual/logical separation between DoD and Federal Government tenants / missions is sufficient. Virtual/logical separation between tenant/mission systems is required.
- Physical separation from non-DoD/non-Federal Government tenants (that is, public, local/state government tenants) is required.
- The CSP restricts potential access to DoD's and the community's information to CSP employees that are U.S. Citizens.

## Microsoft in-scope cloud platforms & services

- Azure
- Dynamics 365 Customer Service
- Microsoft Defender for Endpoint (formerly Microsoft Defender Advanced Threat Protection)
- Microsoft Graph
- Microsoft Stream
- Office 365 U.S. Government Defense
- Power Automate (formerly Microsoft Flow)
- Power BI

## Azure, Dynamics 365, and DoD IL5

For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure DoD IL5 offering](/azure/compliance/offerings/offering-dod-il5).

## Office 365 and DoD IL5

### Office 365 cloud environments

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### Office 365 applicability and in-scope services

Use the following table to determine applicability for your Office 365 services and subscription:

| **Applicability** | **In-scope services** |
|:------------------|:----------------------|
| **DoD** | Activity Feed Service, Bing Services, Exchange Online, Exchange Online Protection, Intelligent Services, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, SharePoint Online, Skype for Business, Windows Ink |

### Attestation documents

US government customers can request Office 365 U.S. Government Defense FedRAMP documentation directly from the [FedRAMP Marketplace](https://marketplace.fedramp.gov/#!/products?sort=productName&productNameSearch=azure) by submitting a package access request form. You must have a .gov or .mil email address to access a FedRAMP security package directly from FedRAMP.

Select FedRAMP and DoD documentation, including System Security Plan (SSP), continuous monitoring reports, Plan of Action and Milestones (POA\&M), etc., is available to customers under NDA and pending access authorization from the Service Trust Portal [Audit Reports - FedRAMP Reports](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3) section. Contact your Microsoft account representative for assistance.

### Resources

- [Microsoft government solutions](https://www.microsoft.com/enterprise/government)
- [DoD Cloud Computing Security Requirements Guide](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)
- [FedRAMP documents](https://www.fedramp.gov/documents/)
- [DoD Instruction 8510.01](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodi/851001p.pdf) *DoD Risk Management Framework (RMF) for DoD Information Technology (IT)*
- [NIST SP 800-37](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) *Risk Management Framework for Information Systems and Organizations: A System Life-Cycle Approach for Security and Privacy*
- [NIST SP 800-53](https://csrc.nist.gov/Projects/risk-management/sp800-53-controls/release-search#!/800-53) *Security and Privacy Controls for Information Systems and Organizations*
- [NIST SP 800-59](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-59.pdf) *Guideline for Identifying an Information System as a National Security System*
- [CNSSI 1253](https://www.dcsa.mil/portals/91/documents/ctp/nao/CNSSI_No1253.pdf) *Security Categorization and Control Selection for National Security Systems*
- [NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final) *Protecting Controlled Unclassified Information in Nonfederal Systems and Organizations*
- Controlled Unclassified Information (CUI) [Registry](https://www.archives.gov/cui) and CUI [category list](https://www.archives.gov/cui/registry/category-list).
