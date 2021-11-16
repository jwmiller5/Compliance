---
title: "Identity and access management overview"
description: "Learn about identity and access management in Microsoft 365"
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: article
f1.keywords:
- NOCSH
ms.service: O365-seccomp
ms.localizationpriority: medium
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

# Identity and access management overview

## How do Microsoft online services protect production systems from unauthorized or malicious access?

Microsoft online services are designed to allow Microsoft's engineers to operate services without accessing customer content. By default, Microsoft engineers have Zero Standing Access (ZSA) to customer content and no privileged access to the production environment. Microsoft online services use a Just-In-Time (JIT), Just-Enough-Access (JEA) model to provide service team engineers with temporary privileged access to production environments when such access is required to support Microsoft online services. The JIT access model replaces traditional, persistent administrative access with a process for engineers to request temporary elevation into privileged roles when required.

Engineers assigned to a service team to support production services request eligibility for a service team account through an identity and access management solution. The request for eligibility triggers a series of personnel checks to ensure the engineer has passed all cloud screening requirements, completed necessary training, and received appropriate management approval prior to account creation. Only after meeting all eligibility requirements can a service team account be created for the requested environment. To maintain eligibility for a service team account, personnel must go through role-based training annually and rescreening every two years. Failure to complete or pass these checks result in eligibilities automatically being revoked.

Service team accounts do not grant any standing administrator privileges or access to customer content. When an engineer requires additional access to support Microsoft online services, they request temporary elevated access to the resources they require using an access management tool called Lockbox. Lockbox restricts elevated access to the minimum privileges, resources, and time needed to complete the assigned task. If an authorized reviewer approves the JIT access request, the engineer is granted a temporary account with only the privileges necessary to complete their assigned work. This temporary account requires multifactor authentication and is automatically deleted after the approved period expires.

JEA is enforced by eligibilities and Lockbox roles at the time of request for JIT access. Only requests for access to assets within the scope of the engineer's eligibilities are accepted and passed on to the approver. Lockbox automatically rejects JIT requests that are outside the scope of the engineer's eligibilities and Lockbox roles, including requests that exceed allowed thresholds.  

## How do Microsoft online services use role-based access control (RBAC) with Lockbox to enforce least privilege?

Service team accounts do not grant any standing administrator privileges or access to customer content. JIT requests for limited administrator privileges are managed through Lockbox. Lockbox uses RBAC to limit the types of JIT elevation requests engineers can make, providing an additional layer of protection to enforce least privilege. RBAC also helps enforce separation of duties by limiting service team accounts to appropriate roles.
Engineers supporting a service are granted membership to security groups based on their role. Membership in a security group does not grant any privileged access. Instead, security groups allow engineers to use Lockbox to request JIT elevation when required for supporting the system. The specific JIT requests an engineer can make are limited by their security group memberships.

## How do Microsoft online services handle remote access to production systems?

Microsoft online services system components are housed in datacenters geographically separated from the operations teams. Datacenter personnel do not have logical access to Microsoft online services systems. As a result, Microsoft service team personnel manage the environment through remote access. Service team personnel who require remote access to support Microsoft online services are only granted remote access after approval from an authorized manager. All remote access uses FIPS 140-2 compatible TLS for secure remote connections.

Microsoft online services use Secure Admin Workstations (SAW) for service team remote access to help protect Microsoft online service environments from compromise. These workstations are designed to prevent intentional or unintentional loss of production data, including locking down USB ports and limiting the software available on the Secure Admin Workstation to what is required for supporting the environment. Secure Admin Workstations are closely tracked and monitored to detect and prevent malicious or inadvertent compromise of customer data by Microsoft engineers.

## How does Customer Lockbox add additional protection for customer content?

Customers can add an additional level of access control to their content by enabling Customer Lockbox. When a Lockbox elevation request involves access to customer content, Customer Lockbox requires approval from the customer as a final step in the approval workflow. This process gives organizations the option to approve or deny these requests and provides direct access control to the customer. If the customer rejects a Customer Lockbox request, access to the requested content is denied. If the customer does not reject or approve the request within a certain period, then the request will expire automatically without Microsoft obtaining access to customer content. If the customer approves the request, then Microsoft's temporary access to customer content will be logged, auditable, and revoked automatically after the time assigned to complete the troubleshooting operation expires.

## Related external regulations & certifications

Microsoft's online services are regularly audited for compliance with external regulations and certifications. Refer to the following table for validation of controls related to identity and access control.

### Azure and Dynamics 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.9.1: Business requirements of access control <br> A.9.2: User access management <br> A.9.3: User responsibilities <br> A.9.4: System and application access control <br> A.15.1: Information security in supplier relationships | December 2, 2020 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.9.1: Business requirements of access control <br> A.9.2: User access management <br> A.9.3: User responsibilities <br> A.9.4: System and application access control <br> A.15.1: Information security in supplier relationships | December 2, 2020 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=af02eb56-4261-416b-98e3-2e713e37a77e&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=645b2f97-5bfd-4cea-b02c-c4bcda328a37&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | OA-2: Provisioning access <br> OA-7: JIT access <br> OA-21: Secure Admin Workstations and MFA | March 31, 2021 <br> November 12, 2021 <br> November 12, 2021|

### Office 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | AC-2: Account management <br> AC-3: Access enforcement <br> AC-5: Separation of duties <br> AC-6: Least privilege <br> AC-17: Remote access | September 24, 2020 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=08ce227f-d1d9-4c4c-b255-4f2e4ec8f941&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27001/27002)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27017)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.9.1: Business requirements of access control <br> A.9.2: User access management <br> A.9.3: User responsibilities <br> A.9.4: System and application access control <br> A.15.1: Information security in supplier relationships | March, 2021 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-33: Account modification <br> CA-34: User authentication <br> CA-35: Privileged access <br> CA-36: Remote access <br> CA-57: Customer Lockbox Microsoft management approval <br> CA-58: Customer Lockbox service requests <br> CA-59: Customer Lockbox notifications <br> CA-61: JIT review and approval | December 24, 2020 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-32: Shared account policy <br> CA-33: Account modification <br> CA-34: User authentication <br> CA-35: Privileged access <br> CA-36: Remote access <br> CA-53: Third-party monitoring <br> CA-56: Customer Lockbox customer approval <br> CA-57: Customer Lockbox Microsoft management approval <br> CA-58: Customer Lockbox service requests <br> CA-59: Customer Lockbox notifications <br> CA-61: JIT review and approval | December 24, 2020 |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-15: Customer Lockbox requests | December 24, 2020 |