---
title: "Resiliency and continuity"
description: "Learn about resiliency and continuity in Microsoft 365"
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

# Resiliency and continuity overview

## How does Microsoft ensure business continuity if a disaster or other threat to service availability occurs?

Microsoft's Enterprise Business Continuity Management (EBCM) team oversees business continuity management and disaster recovery activities across Microsoft services and cloud offerings. Representatives from Microsoft business units coordinate with the EBCM team to develop business continuity plans and validate compliance with business continuity requirements.

The Business Continuity Management (BCM) lifecycle is at the core of our BCM methodology. This three-phase process is designed to be adaptable so it can be implemented by a wide variety of business models across Microsoft. It begins with an **Assessment** phase to identify critical processes and objectives that should be included in the business continuity program. The Assessment phase also requires a Business Impact Analysis (BIA). The **Planning** phase focuses on developing and implementing resilience and recovery strategies and documenting them in official business continuity plans. Finally, **Capability Validation** tests business continuity plans and their implementations to verify effectiveness and identify potential improvements.

Microsoft online services business continuity strategies use hardware, network, and datacenter redundancy. Data replication between datacenters provides high availability and reliability during a catastrophic incident. It also increases resilience to mundane incidents such as isolated hardware failure or data corruption.

## How does Microsoft test business continuity and disaster recovery plans?

Microsoft's Enterprise Business Continuity Management (EBCM) policy stipulates that all Microsoft business continuity and disaster recovery plans must be tested, updated, and reviewed on an annual basis. Microsoft online services test their business continuity plans at least annually per EBCM policies. After Action reports are created and reviewed to validate,  test results and inform plan updates in response to any problems discovered during testing.

To validate resilience and recovery strategies against a wide range of potential incidents, the EBCM Program defines multiple categories of test scenarios affecting people, locations, and technology. The level of validation required for each service is based on the service's criticality, with more critical services receiving more rigorous validation. Each Microsoft online service team tests their business continuity plan according to EBCM guidelines to measure the plan's effectiveness and the service team's readiness to execute the plan.

Per EBCM guidelines, annual reviews of business continuity plans and capability validation must take place within 12 months of the last review. Capability validation must include review of supporting documentation, such as the BIA, to ensure it remains accurate. Microsoft makes capability validation results for select Microsoft online services available to our customers through quarterly reports.

## How do Microsoft online services ensure system capacity meets demand?

Capacity planning helps service teams allocate the resources necessary to support Microsoft online service availability. Regular capacity planning is required as part of Microsoft's EBCM program. Service teams review capacity data during quarterly reviews, and during emergency situations that warrant more capacity review.

The raw data for capacity planning is maintained by each service team and includes metrics like system processing, memory, and hardware capacity. Scheduled reviews use a model of the system's current capacity and test it against projected needs in emergency situations. If the model indicates gaps in capacity, proposed changes to system capacity are submitted to service team leadership for review. Approved changes are incorporated into a new model before implementation by service team engineers.

## How do Microsoft online services maintain service availability during routine system failures?

Microsoft online services achieve service resilience through redundant architecture, data replication, and automated integrity checking. Redundant architecture involves deploying multiple instances of a service on geographically and physically separate hardware, providing increased fault-tolerance for Microsoft online services. Data replication ensures there are always multiple copies of customer data in different fault-zones, allowing critical customer data to be recovered if corrupted, lost, or even accidentally deleted by the customer. Automated integrity checking increases data availability by automatically restoring data impacted by many kinds of physical or logical corruption.

## Related external regulations & certifications

Microsoft's online services are regularly audited for compliance with external regulations and certifications. Refer to the following table for validation of controls related to resiliency and continuity.

### Azure and Dynamics 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=57c75724-dab3-44c6-8aa5-46fe697998c7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=2f22dafd-6c62-469b-9bb2-39ff2cff55e2&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d1172883-7a12-45e9-aee1-d09501beba5e&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.17.1: Information security continuity <br> A.17.2: Redundancies | December 2, 2020 |
| [ISO 22301](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=71a4321f-32e7-4da5-9b11-967731c82ff0&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=2f355027-2549-4dcc-b6f0-7394ff69ec35&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | All controls | June 21, 2021 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c771094e-0ed7-4a5f-9244-73ad6ed04bfb&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=af02eb56-4261-416b-98e3-2e713e37a77e&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=645b2f97-5bfd-4cea-b02c-c4bcda328a37&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | BC-1: Business continuity plans <br> BC-3: Business continuity and disaster recovery procedures <br> BC-4: BCDR testing <br> BC-7: Datacenter business continuity plans <br> BC-8: Datacenter business continuity testing <br> BC-9: Datacenter resiliency assessment <br> DS-5: Backup key service components <br> DS-6: Redundancy of critical components <br> DS-7: Automatic replication of customer data <br> DS-8: Backup schedule <br> DS-9: Backup restoration procedures <br> DS-11: Offsite backups <br> DS-14: Automatic restoration of customer services | September 30, 2021 <br> November 12, 2021 <br> November 12, 2021 |

### Office 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | CP-2: Contingency plan <br> CP-3: Contingency training <br> CP-4: Contingency plan testing <br> CP-6: Alternate storage site <br> CP-7: Alternate processing site <br> CP-9: Information system backup <br> CP-10: Information system recovery and reconstitution | September 24, 2020 |
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=08ce227f-d1d9-4c4c-b255-4f2e4ec8f941&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=118969b1-19e5-47dc-9c42-05a0daa44aec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.17.1: Information security continuity <br> A.17.2: Redundancies | April 20, 2021 |
| [ISO 22301](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=08ce227f-d1d9-4c4c-b255-4f2e4ec8f941&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=2bb29cc0-53e7-4a53-a9de-871316e1b80c&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | All controls | March 18, 2019 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a65bb45f-8a4a-4a44-9aaa-55235263505f&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8f3942c-845e-418f-8f6e-329dbf6efce0&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-49: Backup policies <br> CA-50: Business continuity <br> CA-51: Data replication | September 30, 2021 |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=328d765a-1397-4ccc-9978-95de114dd3f2&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-09: EXO email restoration | September 30, 2021 |

## Resources

- [Video: Microsoft online services continuity management](https://www.youtube.com/watch?v=J0QUgUW8sAs)
- [Microsoft Enterprise Business Continuity Management Program Whitepaper](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=64f922a6-d624-40dd-a8ae-6f996b5186f3&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f)
- [Microsoft Cloud EBCM and Disaster Recovery Plan Validation Report: FY22 Q2](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=93c35abe-4f6f-4624-a939-8791d4c49821&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_FAQ_and_White_Papers)

## Legal disclaimer

- [Enterprise business continuity legal disclaimer](assurance-ebcm-legal-disclaimer.md)