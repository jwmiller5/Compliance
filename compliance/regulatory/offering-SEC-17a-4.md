---
title: Securities and Exchange Commission (SEC) Rule 17a-4(f) United States
description: An independent assessment firm validated that Azure and Office 365 can help financial firms meet SEC Rule 17a-4(f) records retention and immutable storage requirements.
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
- M365-security-compliance
- MS-Compliance
hideEdit: true
titleSuffix: Microsoft Compliance
---

# Securities and Exchange Commission (SEC) Rule 17a-4(f) United States

## About SEC Rule 17a-4(f)

The [US Securities and Exchange Commission (SEC)](https://www.sec.gov/) is an independent agency of the US federal government and the primary overseer and regulator of US securities markets. It wields enforcement authority over federal securities laws, proposes new securities rules, and oversees market regulation of the securities industry.

The SEC defines rigorous and explicit requirements for regulated entities that elect to retain books and records on electronic storage media. It established [17 CFR 240.17a-3](https://www.govinfo.gov/app/details/CFR-2012-title17-vol3/CFR-2012-title17-vol3-sec240-17a-3) and [17 CFR 240.17a-4](https://www.ecfr.gov/cgi-bin/text-idx?mc=true&node=pt17.4.240&rgn=div5#se17.4.240_117a_64) to regulate recordkeeping, including retention periods, for securities broker-dealers. Later, the SEC [amended](https://www.sec.gov/rules/interp/34-47806.htm) 17 CFR 240.17a-4 paragraph (f), issuing two interpretive releases expressly to allow books and records to be retained on electronic storage media as long as certain conditions were met.

An electronic storage system meets those conditions if it prevents the alteration or erasure of records for the required retention period. Retention periods vary from three to six years based on record types, with immediate accessibility mandated for the first two years. Moreover, one of the interpretive releases requires that the storage system be capable of retaining records beyond the SEC-established retention period to comply with subpoenas, legal hold, or other such requirements.

## Microsoft and SEC Rule 17a-4(f)

Financial services customers, representing one of the most heavily regulated industries in the world, are subject to complex provisions like the retention of financial transactions and related communication in a non-erasable and non-modifiable state. Among the most prescriptive is Rule 17a-4(f) of the US Security and Exchange Commission (SEC) that stipulates stringent requirements for regulated entities that elect to retain books and records on electronic storage media. Records stored must be tamper-proof with no ability to alter or delete them until after the designated retention period.

Microsoft Azure Immutable Blob Storage with Policy Lock and Microsoft Office 365 with Preservation Lock can help financial institutions meet the immutable storage requirements of SEC Rule 17a-4(f).

## Microsoft in-scope cloud platforms & services

- [Azure](https://gallery.technet.microsoft.com/Overview-of-Azure-c1be3942)
- [Office 365](https://aka.ms/Office365ComplianceOfferings)

## Independent assessments

To evaluate Azure and Office 365 compliance with SEC Rule 17a-4(f), Microsoft retained an independent assessment firm that specializes in records management and information governance, Cohasset Associates.

### Azure

[Immutable storage for Azure Blob storage](/azure/storage/blobs/storage-blob-immutable-storage) enables users to store business-critical records in a write once read many (WORM) state. This state makes the data non-erasable and non-modifiable for a user-specified interval. For the duration of the retention interval, blobs can be created and read, but cannot be modified or deleted. These features of Azure immutable storage can help customers address their records retention requirements.

Microsoft retained an independent third-party assessment firm that specializes in records management and information governance to evaluate immutable storage for Azure Blob storage compliance with SEC Rule 17a-4(f) requirements. The resulting report *[Cohasset Assessment: Microsoft Azure WORM Storage](https://azure.microsoft.com/resources/azure-immutable-storage-assessment-for-sec-17a-4f-by-cohasset/)* is available to customers.

It is the assessor's opinion that Azure Storage with the *immutable storage for Azure Blobs* feature and *locked time-based policy* option retains time-based Blobs (records) in a non-erasable and non-rewritable format and meets relevant storage requirements of SEC Rule 17a-4(f), [FINRA Rule 4511(c)](./offering-finra-4511-us.md), and the principles-based requirements of [CFTC Rule 1.31(c)-(d)](./offering-cftc-1-31-us.md).

Upon request, Microsoft will also provide a *90-day letter* required to meet the SEC 17a-4(f)(2) requirements for customers to notify their designated examining authority at least 90 days prior to employing electronic storage media. As stated in the regulations, "the member, broker, or dealer must provide its own representation or one from the storage medium vendor or other third party with appropriate expertise that the selected storage media meets the conditions set forth in this paragraph (f)(2)." To obtain the Microsoft *Attestation of Electronic Storage Media Services* for SEC Rule 17a-4, customers with an [Azure support plan](https://azure.microsoft.com/support/plans/) can [create a support ticket](https://azure.microsoft.com/support/create-ticket/) in the Azure portal and request the attestation letter for SEC Rule 17a-4. In this document, Microsoft provides assurances relevant to the SEC 17a-4(f)(2) requirements.

### Office 365

For [SEC 17a-4(f)](/microsoft-365/compliance/retention-regulatory-requirements#sec-17a-4f-finra-4511c-and-cftc-131c-d) requirements, Cohasset validated that Microsoft 365 includes archiving features that enable regulated customers, including broker-dealers, to store data in a manner that helps them comply with SEC requirements for records retention. Retention features in Microsoft 365 help preserve a wide range of data, including email, voicemail, shared documents, instant messages, and third-party data. In particular, archiving in Microsoft 365 enables customers to set global or granular messaging retention policies to store data for a defined period and beyond in a non-rewriteable, non-erasable format.

## Audits, reports, and certificates

### Azure & SEC Rule 17

- [SEC 17a-4(f) & CFTC 1.31 (c-d) Compliance Assessment of Azure Storage](https://azure.microsoft.com/resources/azure-immutable-storage-assessment-for-sec-17a-4f-by-cohasset/)

Microsoft *Attestation of Electronic Storage Media Services* for SEC Rule 17a-4 can be requested by [creating a support ticket](https://azure.microsoft.com/support/create-ticket/) with [Azure support](https://azure.microsoft.com/support/plans/). In this attestation letter, Microsoft provides assurances to help customers comply with the SEC 17a-4(f)(2) requirements.

### Office 365 & SEC Rule 17

- [SEC 17a-4(f) Compliance Assessment: Microsoft Security & Compliance Center with SharePoint, OneDrive, Teams, Exchange, and Skype for Business](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=2dc92867-5f83-49d8-ad04-9e7295c9e40e&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_FAQ_and_White_Papers)

## How to implement

### Financial services regulation

Compliance map of key US regulatory principles for cloud computing and Microsoft online services. [Learn more](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides)

### Risk Assessment & Compliance Guide

Create a governance model for risk assessment of Microsoft cloud services, and regulator notification. [Learn more](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=edee9b14-3661-4a16-ba83-c35caf672bd7&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_FAQ_and_White_Papers)

### Financial use cases

Use case overviews, tutorials, and other resources to build Azure solutions for financial services. [Learn more](/azure/industry/financial/)

## Use Microsoft Compliance Manager to assess your risk

[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft 365 compliance center](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks. Compliance Manager offers a premium template for building an assessment for this regulation. Find the template in the **assessment templates** page in Compliance Manager. Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).

## Resources

- [Azure compliance documentation](/azure/compliance/)
- [Azure enables a world of compliance](https://azure.microsoft.com/resources/azure-enables-a-world-of-compliance/)
- [Securities and Exchange Commission](https://www.sec.gov/) (SEC) [Rule 17a-4](https://www.sec.gov/rules/final/34-38245.txt)
- [Microsoft Cloud financial services resources](https://servicetrust.microsoft.com/viewpage/financialservicesoverview)
- [Microsoft Cloud financial services compliance program](https://aka.ms/FSCP-Print)
- [Compliance map of cloud computing regulatory principles and Microsoft online services](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides)
- [Risk assessment and compliance guide for financial institutions in the Microsoft Cloud](https://azure.microsoft.com/resources/risk-assessment-and-compliance-guide-for-financial-institutions-in-the-microsoft-cloud-/)
- [Financial Services industry use cases](/azure/industry/financial/)
- [Archiving in Microsoft Office 365, Data Retention, and Rule 17a-4](https://www.microsoft.com/microsoft-365/blog/2015/11/10/office-365-exchange-online-archiving-now-meets-sec-rule-17a-4-requirements/)
