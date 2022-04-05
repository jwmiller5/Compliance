---
title: Federal Financial Institutions Examination Council (FFIEC)
description: Microsoft helps financial services clients comply with the audit requirements of the Federal Financial Institutions Examination Council (FFIEC).
keywords: Microsoft 365, compliance, offerings
ms.localizationpriority: medium
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

# Federal Financial Institutions Examination Council (FFIEC)

## FFIEC overview

The Federal Financial Institutions Examination Council (FFIEC) is a formal interagency body comprising five banking regulators that are responsible for US federal government examinations of financial institutions in the United States. The FFIEC Examiner Education Office publishes IT Examination Handbooks intended for field examiners from FFIEC member agencies.

The [FFIEC Audit IT Examination Handbook](https://ithandbook.ffiec.gov/it-booklets/audit.aspx) contains guidance for these examiners to assess the quality and effectiveness of IT audit programs of both financial institutions and TSPs. Specifically, it includes mention of SOC 1, SOC 2, and SOC 3 attestation reports of the American Institute of Certified Public Accountants (AICPA) as examples of independent audit reports. However, the FFIEC recommends that financial institutions not rely solely on the information contained in these reports, but also use verification and monitoring procedures discussed in detail in the [FFIEC Outsourcing Technology Services IT Examination Handbook](https://ithandbook.ffiec.gov/it-booklets/outsourcing-technology-services.aspx).

## Microsoft and FFIEC

Microsoft Azure, Microsoft Power BI, and Microsoft Office 365 are built to meet the stringent requirements of providing cloud services for financial services institutions. Azure provides financial institutions with SOC 1 Type 2, SOC 2 Type 2, and SOC 3 attestation reports produced by an independent auditing firm to help customers meet their own FFIEC compliance obligations. For example, the [SOC 1 Type 2 attestation](./offering-soc-1.md) is performed under:

- SSAE No. 18, Attestation Standards: Clarification and Recodification, which includes AT-C section 320, *Reporting on an Examination of Controls at a Service Organization Relevant to User Entities' Internal Control Over Financial Reporting* (AICPA, Professional Standards).
- SOC 1 Reporting on an Examination of Controls at a Service Organization Relevant to User Entities' Internal Control Over Financial Reporting (AICPA Guide).

The AICPA SSAE 18 standard replaced SAS 70, and it is appropriate for reporting on controls at a service organization relevant to user entities internal controls over financial reporting. This is the formal audit that financial institutions can leverage for third-party reviews of technology service providers when pursuing their own FFIEC specific compliance obligations for assets deployed on Azure. It includes auditor’s opinion on control effectiveness to achieve the related control objectives during the specified monitoring period.

Moreover, Azure has developed an Excel-based cloud security diagnostic tool intended to expedite a risk assessment that a financial institution may want to conduct relative to Azure services. The tool is based on a spreadsheet featuring 19 separate domains that identify requirements set forth in relevant standards and financial services-related regulations, including the FFIEC IT Examination Handbooks.  The risk assessment tool is pre-populated with explanations for how Azure complies with requirements applicable to cloud service providers, and can assist customers in meeting their own FFIEC compliance requirements.

Also available to customers is the Azure FFIEC cloud security diagnostic workbook companion, which offers guidance on the use of Azure services and considerations for customer compliance with FFIEC requirements

## Microsoft in-scope cloud platforms & services

- Azure
- Intune
- Office 365, Office 365 U.S. Government
- Power BI cloud service (either as a standalone service or as included in an Office 365 branded plan or suite)

## Azure guidance documents

To assist financial institutions subject to FFIEC oversight with cloud adoption, Microsoft has published the following guidance documents that can be downloaded from the Service Trust Portal [Data Protection Resources - Compliance Guides](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3) section:

- Azure - Cloud security diagnostic tool
- Azure - FFIEC cloud security diagnostic workbook companion

## Office 365 and FFIEC

### Office 365 environments

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### Office 365 applicability and in-scope services

Use the following table to determine applicability for your Office 365 services and subscription:

| **Applicability** | **In-scope services** |
|:------------------|:----------------------|
| **Commercial** | Azure Active Directory, Azure Information Protection, Bookings, Compliance Manager, Delve, Exchange Online, Exchange Online Protection, Forms, Kaizala, Microsoft Analytics, Microsoft Booking, Microsoft Defender for Office 365, Microsoft Graph, Microsoft Teams, Microsoft To-Do for Web, MyAnalytics, Office 365 Advanced Compliance add-on, Office 365 Cloud App Security, Office 365 Groups, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business, StaffHub, Stream, Sway, Yammer Enterprise |
| **GCC** | Azure Active Directory, Compliance Manager, Delve, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, MyAnalytics, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business, Stream |

### Office 365 audits, reports, and certificates

See the Office 365 SOC attestation reports.

### Frequently asked questions

**Can I use Microsoft compliance with SOC standards to meet the FFIEC compliance obligations for my institution?**

To help you meet these obligations, Microsoft supplies the specifics about our compliance with SOC standards as described above. However, ultimately, it is up to you to determine whether our services comply with the specific laws and regulations applicable to your institution. The FFIEC also advises that 'users of audit reports or reviews should not rely solely on the information contained in the report to verify the internal control environment of the TSP. They should use other verification and monitoring procedures as discussed more fully in the [Outsourcing Technology Booklet](https://ithandbook.ffiec.gov/it-booklets/outsourcing-technology-services.aspx) of the FFIEC IT Examination Handbook.'

### Use Microsoft Compliance Manager to assess your risk

[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft Purview compliance portal](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks. Compliance Manager offers a premium template for building an assessment for this regulation. Find the template in the **assessment templates** page in Compliance Manager. Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).

## Resources

- [Federal Financial Institutions Examination Council (FFIEC)](https://www.ffiec.gov/)
- [Compliance Map of Cloud Computing and Regulatory Principles in the US](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides)
- [FFIEC Audit IT Examination Handbook](https://ithandbook.ffiec.gov/it-booklets/audit.aspx)
- [FFIEC Outsourcing Technology Services IT Examination Handbook](https://ithandbook.ffiec.gov/it-booklets/outsourcing-technology-services.aspx)

## Other Microsoft resources for financial services

- [Azure compliance documentation](/azure/compliance/)
- [Azure enables a world of compliance](https://azure.microsoft.com/resources/azure-enables-a-world-of-compliance/)
- [Microsoft Cloud financial services resources](https://servicetrust.microsoft.com/viewpage/financialservicesoverview)
- [Microsoft Cloud financial services compliance program](https://aka.ms/FSCP-Print)
- [Risk assessment and compliance guide for financial institutions in the Microsoft Cloud](https://azure.microsoft.com/resources/risk-assessment-and-compliance-guide-for-financial-institutions-in-the-microsoft-cloud-/)
- [Financial Services industry use cases](/azure/industry/financial/)
