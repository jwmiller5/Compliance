---
title: "Data-bearing device destruction"
description: In this article, you'll find an overview of the data-bearing device destruction process for Microsoft datacenters.
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
search.appverid:
- MET150
ms.collection:
- M365-security-compliance
- MS-Compliance
- MS-Compliance-Assurance
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
---

# Data-bearing device destruction

## Data destruction overview

Microsoft has data-bearing device (DBD) guidelines, policies, security requirements, and procedures for handling and management of DBDs within Microsoft datacenters.

A DBD is any storage device capable of storing customer or proprietary Microsoft data:

- Hard disk drives (HDD)
- Solid-state drives (SSD)
- USB drives
- IO Accelerator cards
- SD/Compact Flash cards
- HSM cards
- PCIe SSD cards
- NVDIMM (Non-Volatile Dual In-line Memory Module)

Failed DBDs used within Microsoft datacenters are audited and destroyed within the datacenter campus. Any asset retired from service is evaluated for disposal in a manner commensurate with its security/privacy requirements and asset classification, and in accordance with any applicable rules, laws, and regulations.

Microsoft uses three categories of data sanitization for DBDs and assets containing data:

- **Clear**: relates to the logical techniques that help to sanitize data in all user-addressable storage locations for protection against simple non-invasive data recovery techniques. These are techniques typically applied through the standard read and write commands to the storage device, such as by rewriting with a new value or using a menu option to reset the device to the factory state (where rewriting is not supported).
- **Purge**: relates to physical or logical techniques that render target data recovery infeasible using state-of-the-art laboratory techniques.
- **Destroy**: renders target data recovery infeasible using state-of-the-art laboratory techniques and results in the subsequent inability to use the media for storage of data.

Purge and destroy sanitization is performed using tools and processes approved by the Security Group. Records are kept of the erasure and destruction of assets. Devices that fail to complete the clear are successfully degaussed (for magnetic media only), multi-pin punched (for chipped based boards such as SSDs), or destroyed.

## Clear

If a retired asset is evaluated and deemed to be non-accessible, it is cleared by an approved data eradication solution. Microsoft datacenters use the NIST SP-800-88 clear guidelines.

## Purge

Depending on the on-site configuration and device availability, some devices are purged before destruction. Purge devices include NSA-approved degaussers for magnetic media and multi-pin punch devices for solid-state media. Microsoft datacenters use the NIST SP-800-88 purge guidelines.

## Destroy

If a retired asset is evaluated and deemed to be accessible, it is destroyed onsite using an approved standard operating procedure that meets NIST SP-800-88 guidelines. These DBDs are physically and logically tracked to maintain chain of custody through final disposition.

Each Microsoft datacenter uses an on-site process to sanitize and dispose of failed and retired DBDs. During this process, Microsoft personnel ensure chain of custody is maintained throughout the disposal process.

## Resources

- [NIST Special Publication 800-88](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-88r1.pdf)
