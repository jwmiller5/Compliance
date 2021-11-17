---
title: "Architecture overview"
description: "Learn about architecture in Microsoft 365"
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

# Architecture overview

## What are Microsoft online services?

Microsoft online services refer to the cloud-based services offered by Microsoft, which includes Azure, Dynamics 365, and Microsoft 365.  Each service offers unique solutions to common business operation and productivity needs, serving customers around the world ranging from small businesses to large enterprises and governments. Globally distributed  datacenters connected by Microsoft's independently managed network infrastructure act as the backbone to support online services, providing the ability to sustain availability in almost every situation and scale to massive worldwide demand.

All Microsoft online services have the same goal of safeguarding the service infrastructure they manage and their customers' data, but each online service is operated by a separate business unit. In many instances, security controls are implemented in the same way across all services, but in some cases, they take a different approach to fulfilling their customer promises and compliance obligations.

## What is Azure?

Microsoft Azure is a cloud computing platform for building, deploying, and managing applications through a global network of Microsoft and third-party managed datacenters. It supports both Platform as a Service (PaaS) and Infrastructure as a Service (IaaS) cloud service models, and enables hybrid solutions that integrate cloud services with customers' on-premises resources. Microsoft Azure supports many customers, partners, and government organizations that span across a broad range of products and services, geographies, and industries. Microsoft Azure is designed to meet their security, confidentiality, and compliance requirements.

## What is Dynamics 365?

Dynamics 365 is an online business application suite that integrates the Customer Relationship Management (CRM) capabilities and its extensions with the Enterprise Resource Planning (ERP) capabilities. These end-to-end business applications help customers turn relationships into revenue, earn customers, and accelerate business growth. Dynamics 365 is a Software as a Service (SaaS) suite built on Azure's infrastructure and is made available to customers around the world through their globally distributed datacenters.

## What is Microsoft 365?

Microsoft 365 is the cloud-powered, subscription-based version of Office, Windows 10, Enterprise Mobility + Security, and Compliance. Microsoft 365 customers get clients such as Outlook and Windows, and they also benefit from services that Microsoft hosts on their behalf, such as Exchange Online, Microsoft Teams, and SharePoint Online. All components of the service are regularly updated as part of the subscription model, so that our customers have an 'evergreen' product. Microsoft manages the service infrastructure on behalf of customers, meaning that Microsoft is responsible for securing the infrastructure that stores customer data.

In terms of scale, Microsoft currently uses close to a million machines to power Microsoft 365 services. The infrastructure powering these services varies widely across service-specific hardware and virtualized environments in Azure, Windows and Linux, and multi-tenant and dedicated platforms. Microsoft 365 is a global business, and our infrastructure is distributed in datacenters around the world, enabling our customers to meet data residency and sovereignty requirements.

## How do Microsoft online services ensure isolation between customer tenants?

Microsoft's cloud services are built on the assumption that all tenants are potentially hostile to all other tenants. To properly isolate tenants from one another, Microsoft implements various isolation technologies and controls. These controls are designed to safeguard against information leakage or unauthorized access to customer data across tenants and to prevent the actions of one tenant from adversely affecting the service for another tenant.

Customer content is logically isolated within tenants using Azure Active Directory (Azure AD). User authentication in Microsoft online services verifies not only the user identity, but also the tenant identity the user account is part of, preventing users from accessing data outside their tenant environment. To supplement the logical isolation of Azure AD, customer content is always encrypted at rest and in transit. Individual services may also provide additional layers of tenant isolation, such as SharePoint Online isolation of tenant data in separate, encrypted databases.

## How do Microsoft online services engineer resilient services that avoid single points of failure?

Microsoft designs and builds cloud services to maximize reliability and minimize the negative effects on customers in the face of faults and challenges to normal operations. This strategy begins with the design of the network connecting our geographically distributed datacenters. Microsoft's network architecture includes direct interconnections and multiple network paths. Microsoft online services use this redundancy to automatically route traffic around failures to improve service quality.

Wherever possible, Microsoft online services are deployed in active/active configurations with automated service health monitoring, allowing the service to detect and recover from many common faults and failures without human intervention. In addition to active/active configurations, Microsoft online services increase fault-tolerance by ensuring the service is deployed in separate fault zones, preventing a fault in one zone from affecting the availability of other zones.

Data resiliency complements service resiliency by protecting the integrity and availability of data in Microsoft online services. Our services use local storage redundancy and geo-redundancy to replicate copies of customer data into different fault zones. If data is corrupted or lost in one fault zone, it can be accessed in another fault zone without loss of availability. Automated integrity checking automatically restores data impacted by many kinds of physical or logical corruption. Microsoft also provides customers with tools to restore data accidentally deleted or modified by the customer in services such as Exchange Online and SharePoint Online.

## How do Microsoft online services track dependencies and prevent unauthorized external system connections?

Microsoft online services teams identify critical system components and their dependencies as part of Business Continuity Management. In addition, Microsoft documents and tracks all external system connections to ensure only authorized connections are allowed in network firewall configurations. Microsoft online services systems, dependencies, and external connections are documented in Microsoft online services' information security architecture. Both the information security architecture and corresponding data flow diagrams are reviewed and updated annually at a minimum, as well as whenever significant changes are made to the system.

Microsoft online services architecture is validated regularly and automatically using cloud-based tools to verify alignment with our security principles and to continuously test isolation and resiliency features. Architectural validation works to automatically identify instances where the current state of the service has drifted from the desired state, flagging any deviations for review and mitigation. The goal of architecture validation is to ensure the security capabilities of our service infrastructure continue to function as expected.

## Related external regulations & certifications

Microsoft's online services are regularly audited for compliance with external regulations and certifications. Refer to the following table for validation of controls related to architecture.

### Azure and Dynamics 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.6: Organization of information security <br> A.13.1: Network security management <br> A.17.2: Redundancies | December 2, 2020 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.6: Organization of information security <br> A.13.1: Network security management <br> A.17.2: Redundancies | December 2, 2020 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=af02eb56-4261-416b-98e3-2e713e37a77e&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=645b2f97-5bfd-4cea-b02c-c4bcda328a37&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | BC-1: Business continuity plans <br> BC-3: BCDR procedures <br> BC-4: BCDR testing <br> BC-5: Business continuity risk assessments <br> BC-6: Third-party business continuity <br> BC-7: Datacenter business continuity procedures <br> BC-8: Datacenter business continuity testing <br> BC-9: Datacenter resiliency assessment <br>  DS-6: Redundancy of critical components <br> DS-7: Replication of customer data <br> DS-14: Restoration of customer services <br> DS-16: Customer data segregation | March 31, 2021 <br> November 12, 2021 <br> November 12, 2021 |

### Office 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | AC-4: Information flow enforcement <br> CP-9: Information system backup <br> PL-8: Information security architecture <br> SC-7: Boundary protection <br> SC-22: Architecture and provisioning | September 24, 2020 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=08ce227f-d1d9-4c4c-b255-4f2e4ec8f941&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27001/27002)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27017)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.6: Organization of information security <br> A.13.1: Network security management <br> A.17.2: Redundancies | March, 2021 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-37: Tenant isolation <br> CA-49: Backup policies <br> CA-51: Data replication | December 24, 2020 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-05: Data flow diagrams <br> CA-37: Tenant isolation <br> CA-49: Backup policies <br> CA-51: Data replication | December 24, 2020 |