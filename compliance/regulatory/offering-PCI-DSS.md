---
title: Payment Card Industry (PCI) Data Security Standard (DSS)
description: Azure, SharePoint Online, and OneDrive for Business comply with Payment Card Industry Data Security Standards Level 1 version 3.2.
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

# Payment Card Industry (PCI) Data Security Standard (DSS)

## PCI DSS overview

The Payment Card Industry (PCI) Data Security Standards (DSS) is a global information security standard designed to prevent fraud through increased control of credit card data. Organizations of all sizes must follow PCI DSS standards if they accept payment cards from the five major credit card brands, Visa, MasterCard, American Express, Discover, and the Japan Credit Bureau (JCB). Compliance with PCI DSS is required for any organization that stores, processes, or transmits payment and cardholder data.

## Microsoft and PCI DSS

Microsoft completed an annual PCI DSS assessment using an approved Qualified Security Assessor (QSA). The auditors reviewed Microsoft Azure, Microsoft OneDrive for Business, and Microsoft SharePoint Online  environments, which include validating the infrastructure, development, operations, management, support, and in-scope services. The PCI DSS designates four levels of compliance based on transaction volume. Azure, OneDrive for Business, and SharePoint Online are certified as compliant under PCI DSS version 3.2 at Service Provider Level 1 (the highest volume of transactions, more than 6 million a year).

The assessment results in an Attestation of Compliance (AoC), which is available to customers and Report on Compliance (RoC) issued by the QSA. The effective period for compliance begins upon passing the audit and receiving the AoC from the assessor and ends one year from the date the AoC is signed. 

Customers who want to develop a cardholder environment or card processing service can use these validations in many of the underlying portions, thereby reducing the associated effort and costs of getting their own PCI DSS certification.

It is important to understand that PCI DSS compliance status for Azure, OneDrive for Business, and SharePoint Online does not automatically translate to PCI DSS certification for the services that customers build or host on these platforms. Customers are responsible for ensuring that they achieve compliance with PCI DSS requirements.

## Microsoft in-scope cloud platforms & services

- Azure and Azure Government
- Intune
- Microsoft Defender for Cloud Apps
- [Microsoft Defender for Endpoint](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection)
- Microsoft Graph
- Office 365
- OneDrive for Business and SharePoint Online (United States only)
- PowerApps cloud service either as a standalone service or as included in an Office 365 or Dynamics 365 branded plan or suite
- Power Automate (either as a standalone service or as included in an Office 365 or Dynamics 365 branded plan or suite)
- Power BI cloud service either as a standalone service or as included in an Office 365 branded plan or suite

## Azure, Dynamics 365, and PCI DSS

For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure PCI DSS offering](/azure/compliance/offerings/offering-pci-dss).

## Office 365 and PCI DSS

### Office 365 environments

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### Office 365 applicability and in-scope services

Use the following table to determine applicability for your Office 365 services and subscription:

| **Applicability** | **In-scope services** |
|:------------------|:----------------------|
| **Commercial** | OneDrive for Business (United States), SharePoint Online (United States) |

### Office 365 audit, reports, and certificates

- [OneDrive for Business and SharePoint Online PCI DSS Attestation of Compliance (AoC)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=f1962237-32ea-4123-939e-1c8f04d13c16&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_PCI_DSS)

### Frequently asked questions

**Why does the Attestation of Compliance (AoC) cover page say 'June 2018'?**

The June 2018 date on the cover page is when the AoC template was published. Refer to Section 2 for the date of the assessment. 

**What is the relationship between the PA DSS and PCI DSS?**

The Payment Application Data Security Standard (PA DSS) is a set of requirements that comply with the PCI DSS, and replaces Visa's Payment Application Best Practices, and consolidates the compliance requirements of the other primary card issuers. The PA DSS helps software vendors develop third-party applications that store, process, or transmit cardholder payment data as part of a card authorization or settlement process. Retailers must use PA DSS certified applications to efficiently achieve their PCI DSS compliance. The PA DSS does not apply to Azure.

**What is an acquirer and does Azure use one?**

An acquirer is a bank or other entity that processes payment card transactions. Azure does not offer payment card processing as a service and thus does not use an acquirer.

**To what organizations and merchants does the PCI DSS apply?**

PCI DSS applies to any company, no matter the size, or number of transactions, that accepts, transmits, or stores cardholder data. That is, if any customer ever pays a company using a credit or debit card, then the PCI DSS requirements apply. Companies are validated at one of four levels based on the total transaction volume over a 12-month period. Level 1 is for companies that process over 6 million transactions a year; Level 2 for 1 million to 6 million transactions; Level 3 is for 20,000 to 1 million transactions; and Level 4 is for fewer than 20,000 transactions.

**Are there plans for OneDrive for Business and SharePoint Online to be PCI DSS-compliant outside of the United States?**

Currently OneDrive for Business and SharePoint Online is PCI-DSS compliant only in the United States (US). Microsoft will evaluate the requirements and timelines for regions outside of US and provide updates when and if other regions are added to the roadmap.

**What is in-scope for OneDrive for Business and SharePoint Online?**

Currently, only files and documents uploaded to OneDrive for Business and SharePoint Online will be compliant with PCI DSS.

### Use Microsoft Purview Compliance Manager to assess your risk

[Microsoft Purview Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft Purview compliance portal](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks. Compliance Manager offers a premium template for building an assessment for this regulation. Find the template in the **assessment templates** page in Compliance Manager. Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).

### Resources

- [PCI Security Standards Council](https://www.pcisecuritystandards.org/)
- [PCI Data Security Standard](https://www.pcisecuritystandards.org/documents/PCI_DSS_v3-1.pdf)
- [PCI DSS Quick Reference Guide](https://www.pcisecuritystandards.org/documents/PCISSC%20QRG%20August%202014%20-print.pdf)
- [Compliance on the Microsoft Trust Center](https://www.microsoft.com/trust-center/compliance/compliance-overview)
