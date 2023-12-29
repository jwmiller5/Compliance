---
title: "Encryption and key management overview"
description: "Learn about encryption and key management in Microsoft 365"
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: overview
f1.keywords:
- NOCSH
ms.service: O365-seccomp
ms.localizationpriority: medium
ms.collection:
- MS-Compliance
- MS-Compliance-Assurance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
---

# Encryption and key management overview

## What role does encryption play in protecting customer content?

Most Microsoft business cloud services are multi-tenant, meaning that customer content may be stored on the same physical hardware as other customers. To protect the confidentiality of customer content, Microsoft online services encrypt all data at rest and in transit with some of the strongest and most secure encryption protocols available.

Encryption isn't a substitute for strong access controls. Microsoft's access control policy of Zero Standing Access (ZSA) protects customer content from unauthorized access by Microsoft employees. Encryption complements access control by protecting the confidentiality of customer content wherever it's stored and by preventing content from being read while in transit between Microsoft online services systems or between Microsoft online services and the customer.

## How do Microsoft online services encrypt data-at-rest?

All customer content in Microsoft online services is protected by one or more forms of encryption. Microsoft servers use BitLocker to encrypt the disk drives containing customer content at the volume-level. The encryption provided by BitLocker protects customer content if there are lapses in other processes or controls (for example, access control or recycling of hardware) that could lead to unauthorized physical access to disks containing customer content.

In addition to volume-level encryption, Microsoft online services use Service Encryption at the application layer to encrypt customer content. Service Encryption provides rights protection and management features on top of strong encryption protection. It also allows for separation between Windows operating systems and the customer data stored or processed by those operating systems.

## How do Microsoft online services encrypt data-in-transit?

Microsoft online services use strong transport protocols, such as TLS, to prevent unauthorized parties from eavesdropping on customer data while it moves over a network. Examples of data in transit include mail messages that are in the process of being delivered, conversations taking place in an online meeting, or files being replicated between datacenters.

For Microsoft online services, data is considered 'in transit' whenever a user's device is communicating with a Microsoft server, or a Microsoft server is communicating with another server.

## How do Microsoft online services manage the keys used for encryption?

Strong encryption is only as secure as the keys used to encrypt data. Microsoft uses its own security certificates to encrypt TLS connections for data-in-transit. For data-at-rest, BitLocker-protected volumes are encrypted with a full volume encryption key, which is encrypted with a volume master key, which in turn is bound to the Trusted Platform Module (TPM) in the server. BitLocker uses FIPS-compliant algorithms to ensure that encryption keys are never stored or sent over the wire in the clear.

Service Encryption provides another layer of encryption for customer data-at-rest giving customers two options for encryption key management: Microsoft-managed keys or Customer Key. When using Microsoft-managed keys, Microsoft online services automatically generate and securely store the root keys used for Service Encryption.

Customers with requirements to control their own root encryption keys can use Service Encryption with a Customer Managed Key. Using Customer Managed Key, customers can generate their own cryptographic keys using either an on-premises Hardware Service Module (HSM) or Azure Key Vault (AKV). Customer root keys are stored in AKV, where they can be used as the root of one of the keychains that encrypts customer mailbox data or files. Customer root keys can only be accessed indirectly by Microsoft online service code for data encryption and can't be accessed directly by Microsoft employees.

## Related external regulations & certifications

Microsoft's online services are regularly audited for compliance with external regulations and certifications. Refer to the following table for validation of controls related to encryption and key management.

### Azure and Dynamics 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=0625f681-1b95-48a8-bec1-e2ea3b927126&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=ae13e89f-8ff6-4ef3-972c-dffb914a3eba&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certificate](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=6f2310d4-117d-468e-a3c5-d6c8556bbc0f&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.10.1: Cryptographic controls <br> A.18.1.5: Cryptographic controls | December 3, 2021 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=0625f681-1b95-48a8-bec1-e2ea3b927126&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certificate](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=f452fc7c-b698-4cf4-8474-85067f2df951&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.10.1: Cryptographic controls <br> A.18.1.5: Cryptographic controls | December 3, 2021 |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=0625f681-1b95-48a8-bec1-e2ea3b927126&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=ae13e89f-8ff6-4ef3-972c-dffb914a3eba&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certificate](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b5ba11f4-9acb-4bb2-901b-5c644eacacb6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.11.6: Encryption of PII transmitted over public data transmission networks | December 3, 2021 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c771094e-0ed7-4a5f-9244-73ad6ed04bfb&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=af02eb56-4261-416b-98e3-2e713e37a77e&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=645b2f97-5bfd-4cea-b02c-c4bcda328a37&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | DS-1: Secure storage of cryptographic certificates and keys <br> DS-2: Customer data is encrypted in-transit <br> DS-3: Internal communication of Azure components encrypted in-transit <br> DS-4: Cryptographic controls and procedures | September 30, 2021 <br> November 12, 2021 <br> November 12, 2021 |

### Office 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1a0939f8-1005-49fd-82f5-bd228aeb323f&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_FedRAMP_Reports) | SC-8: Transmission confidentiality and integrity <br> SC-13: Use of cryptography <br> SC-28: Protection of information at rest <br>  | September 24, 2021 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8873fa17-9962-4be9-b0d0-086262eb84fb&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27001/27002)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=27704ac1-afbd-4c4a-a75c-53d34133b9c4&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27017)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.10.1: Cryptographic controls <br> A.18.1.5: Cryptographic controls | March  2022 |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8873fa17-9962-4be9-b0d0-086262eb84fb&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certificate](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=afce1496-4cf1-439a-97b6-e7ec53fde63f&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.11.6: Encryption of PII transmitted over public data transmission networks | March  2022 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8f3942c-845e-418f-8f6e-329dbf6efce0&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-44: Data-in-transit encryption <br> CA-54: Data-at-rest encryption <br> CA-62: Customer Key mailbox encryption <br> CA-63: Customer Key data deletion <br> CA-64: Customer Key | September 30, 2021 |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=645b2f97-5bfd-4cea-b02c-c4bcda328a37&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2f_SSAE_16_Reports) | CUEC-16: Customer encryption keys <br> CUEC-17: Customer Key vault <br>  CUEC-18: Customer Key rotation| November 12, 2021 |

## Resources

- [Video: Microsoft 365 data at rest encryption](https://www.youtube.com/watch?v=Dk380mk-xh0)
