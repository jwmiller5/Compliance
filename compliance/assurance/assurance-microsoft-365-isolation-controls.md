---
title: "Microsoft 365 isolation controls"
description: "Learn about isolation controls in Microsoft 365"
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: article
f1.keywords:
- NOCSH
ms.service: O365-seccomp
localization_priority: Normal
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
---

# Microsoft 365 isolation controls

Microsoft continuously works to ensure that the multi-tenant architecture of Microsoft 365 supports enterprise-level security, confidentiality, privacy, integrity, local, international, and availability [standards](https://www.microsoft.com/trust-center/compliance/compliance-overview). The scale and the scope of services provided by Microsoft make it difficult and non-economical to manage Microsoft 365 with significant human interaction. Microsoft 365 services are provided through globally distributed data centers, each highly automated with few operations requiring a human touch or any access to customer content. Our staff supports these services and data centers using automated tools and highly secure remote access.

Microsoft 365 is composed of multiple services that provide important business functionality and contribute to the entire Microsoft 365 experience. Each of these services is self-contained and designed to integrate with one another. Microsoft 365 is designed with the following principles:

- Service-oriented architecture: designing and developing software in the form of interoperable services providing well-defined business functionality.
- [Operational security assurance](https://www.microsoft.com/securityengineering/osa): a framework that incorporates the knowledge gained through various capabilities that are unique to Microsoft, including the Microsoft [Security Development Lifecycle](https://www.microsoft.com/sdl/default.aspx), the [Microsoft Security Response Center](https://www.microsoft.com/msrc), and deep awareness of the cybersecurity threat landscape.

Microsoft 365 services inter-operate with each other but are designed and implemented so they can be deployed and operated as autonomous services, independent of each other. Microsoft segregates duties and areas of responsibility for Microsoft 365 to reduce opportunities for unauthorized or unintentional modification or misuse of the organization's assets. Microsoft 365 teams have defined roles as part of a comprehensive role-based access control mechanism.

## Tenant isolation

One of the primary benefits of cloud computing is concept of a shared, common infrastructure across numerous customers simultaneously, leading to economies of scale. Microsoft works continuously to ensure that the multi-tenant architectures of our cloud services support enterprise-level security, confidentiality, privacy, integrity, and availability standards.

Microsoft cloud services were designed with the assumption that all tenants are potentially hostile to all other tenants, and we have implemented security measures to prevent the actions of one tenant from affecting the security or service of another tenant or accessing the content of another tenant.

The two primary goals of maintaining tenant isolation in a multi-tenant environment are:

- Preventing leakage of, or unauthorized access to, customer content across tenants; and
- Preventing the actions of one tenant from adversely affecting the service for another tenant

Multiple forms of protection have been implemented throughout Microsoft 365 to prevent customers from compromising Microsoft 365 services or applications or gaining unauthorized access to the information of other tenants or the Microsoft 365 system itself, including:

- Logical isolation of customer content within each tenant for Microsoft 365 services is achieved through Azure Active Directory authorization and role-based access control.
- SharePoint Online provides data isolation mechanisms at the storage level.
- Microsoft uses rigorous physical security, background screening, and a multi-layered encryption strategy to protect the confidentiality and integrity of customer content. All Microsoft 365 datacenters have biometric access controls, with most requiring palm prints to gain physical access. In addition, all U.S.-based Microsoft employees are required to successfully complete a standard background check as part of the hiring process. For more information on the controls used for administrative access in Microsoft 365, see [Microsoft 365 Administrative Access Controls](assurance-administrative-access-controls-overview.md).
- Microsoft 365 uses service-side technologies that encrypt customer content at rest and in transit, including BitLocker, per-file encryption, Transport Layer Security (TLS) and Internet Protocol Security (IPsec). For specific details about encryption in Microsoft 365, see [Data Encryption Technologies in Microsoft 365](/microsoft-365/compliance/office-365-encryption-in-the-microsoft-cloud-overview).

Together, the above-listed protections provide robust logical isolation controls that provide threat protection and mitigation equivalent to that provided by physical isolation alone.

## Resources

- [Azure AD isolation controls](/microsoft-365/enterprise/microsoft-365-isolation-in-azure-active-directory)
- [Isolation and Access Control in Azure Active Directory](/microsoft-365/enterprise/microsoft-365-isolation-in-azure-active-directory)
- [Monitoring and Testing Tenant Boundaries](assurance-monitoring-and-testing.md)
- [Isolation and Access Control in Microsoft 365](/microsoft-365/enterprise/microsoft-365-isolation-in-microsoft-365)
