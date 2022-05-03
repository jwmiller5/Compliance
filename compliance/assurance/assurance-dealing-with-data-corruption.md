---
title: "Microsoft 365 Dealing with Data Corruption"
description: "This article explains data corruption in Microsoft 365, and efforts taken by Microsoft to prevent and recover data."
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
- MS-Compliance
- MS-Compliance-Assurance
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
---

# Dealing with data corruption in Microsoft 365

One of the challenging aspects of running a large-scale cloud service is how to handle data corruption, given the large volume of data and independent systems. Data corruption can be caused by:

- Application or infrastructure bugs, corrupting some or all of the application state
- Hardware issues that result in lost data or an inability to read data
- Human operational errors
- Malicious hackers and disgruntled employees
- Incidents in external services that result in some loss of data

Because greater resiliency in data integrity means fewer data corruption incidents, Microsoft has built into Microsoft 365 protection mechanisms to prevent corruption from happening, as well as systems and processes that enable us to recover data if it does. Checks and processes exist within the various stages of the engineering release process to increase resiliency against data corruption, including:

- System Design
- Code organization and structure
- Code review
- Unit tests, integration tests, and system tests
- Trip wires tests/gates

Within Microsoft 365 production environments, peer replication between datacenters ensures that there are always multiple live copies of any data. Standard images and scripts are used to recover lost servers, and replicated data is used to restore customer data. In Exchange Online, every mailbox is hosted in [Database Availability Groups (DAGs)](/compliance/assurance-exchange-data-resiliency#database-availability-groups) and replicated to geographically separate datacenters within the same region. Each mailbox database has four copies distributed across datacenters within the DAG: one active copy, two up-to-date copy, and one 7-day lagged copy used in the rare event of catastrophic logical corruption. For SharePoint and OneDrive, [files are written simultaneously](/compliance/assurance/assurance-sharepoint-onedrive-data-resiliency#blob-storage-resilience) to a primary and secondary datacenter region. Multiple types of [checksums](/compliance/assurance/assurance-sharepoint-onedrive-data-resiliency#integrity-checks) are stored in metadata in a separate location than the corresponding files and are used to ensure data integrity through all stages of the data lifecycle.

Because of the built-in data resiliency checks and processes, Microsoft maintains backups only of Microsoft 365 information system documentation (including security-related documentation), using built-in replication in SharePoint Online and our internal code repository tool, Source Depot. System documentation is stored in SharePoint Online, and Source Depot contains system and application images. Both SharePoint Online and Source Depot use versioning and are replicated in near real time.

## Resources

- [Exchange Online Database Availability Groups](/compliance/assurance/assurance-exchange-data-resiliency#database-availability-groups)
- [How does Exchange Online protect mailbox data?](/exchange/back-up-email#how-does-exchange-online-protect-mailbox-data)
- [SharePoint & OneDrive storage resilience](/compliance/assurance/assurance-sharepoint-onedrive-data-resiliency#blob-storage-resilience)
- [SharePoint & OneDrive integrity checks](/compliance/assurance/assurance-sharepoint-onedrive-data-resiliency#integrity-checks)
