---
title: "Microsoft 365 service engineer access control"
description: "An overview of the Microsoft 365 service engineer access control architecture."
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
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
f1.keywords:
- NOCSH
titleSuffix: Microsoft Service Assurance
hideEdit: true
---

# Microsoft 365 service engineer access control

Zero Standing Access (ZSA) means that Microsoft service team personnel do not have any standing privileged access to the Microsoft 365 production environment or to customer data. When a Microsoft service team member wants to update the service or access customer data for any reason, they must submit a request justifying the need and receive approval from an authorized manager. At scale, it isn't feasible to manually provide and remove access as required to maintain Microsoft 365 services, so Microsoft has developed an automated solution to manage privileged access as needed.

## Lockbox

All access to Microsoft 365 systems and customer data is brokered by Lockbox, an access control system that uses a Just-In-Time (JIT) and Just-Enough-Access (JEA) model to provide service engineers with temporary privileged access to specified Microsoft 365 services and data. Additionally, all requests and actions are logged for auditing purposes and are accessible by using the [Office 365 Management Activity API](/office/office-365-management-api/get-started-with-office-365-management-apis) and the [Security and Compliance Center](https://protection.office.com/).

Before a Microsoft service engineer can connect to any Microsoft 365 systems or access customer data, they must submit an access request through Lockbox. This request can only be approved if certain criteria are met:

- The service engineer meets the [eligibility requirements for a service team account](assurance-microsoft-365-account-management.md),
- They belong to the Lockbox role associated with the work in the request,
- The requested access time does not exceed the maximum permitted time,
- They have a legitimate business justification,
- The requested resource they wish to access is within their work scope, and
- They receive manager approval

Once all criteria have been met and verified by Lockbox, temporary access is granted to perform the specific action requested. After the time for the request has elapsed, the access is revoked.

![Lockbox access process.](../media/assurance-lockbox-process.png)

Additionally, if a customer licenses and enables the [Customer Lockbox](/microsoft-365/compliance/customer-lockbox-requests) feature, any attempt from a Microsoft service engineer to access customer data must be additionally approved by an administrator in the customer tenant. The need to access customer data can arise from both customer and Microsoft. For example, an incident raised by a customer may require access to their data to fix the issue or when Microsoft needs data access to apply a specific update.

![Customer Lockbox access process.](../media/assurance-customer-lockbox-process.png)

Customers do not have any tools to initiate a Customer Lockbox request; they must submit a ticket to Microsoft that requires a Customer Lockbox request to be raised. A Customer Lockbox request raised by a Microsoft service engineer must be approved by a Microsoft Manager and an authorized administrator in the customer tenant.

### Lockbox roles

To enforce separation of duties and the principle of least privilege, service engineers must belong to a Lockbox role that corresponds to their role on the team. Lockbox roles are managed within the Identity Management tool and define the privileges and actions a service team member can be approved for through the Lockbox request process. Service team personnel must request to be a member of a Lockbox role and receive managerial approval. If approved, the employee's service team account is placed in a security group enforced by Active Directory (AD) and Azure Active Directory (AAD).

## Constrained management interfaces

Service engineers use two management interfaces to perform administrative tasks: Remote Desktop from a Secure Access Workstation (SAW) through a secured Terminal Service Gateway (TSG) and Remote PowerShell. Within these management interfaces, access controls based on the approved Lockbox request and software policies place significant restrictions on which applications are executed and which commands and cmdlets are available.

## Remote Desktop

Service team members administrating their service using Remote Desktop must connect from a SAW, specially designed and manufactured laptops managed by Microsoft specifically for this use case. Microsoft partners with suppliers to build SAWs, creating a short and secure supply chain. SAWs use hardened operating systems that are configured to limit all functionality except what is needed for defined management tasks. These limitations include disabling of all USB ports, strict application access lists, removal of email access, limiting internet browsing, and enforcing inactivity screensaver lockouts. Microsoft access control systems examine SAW machines periodically to ensure they are compliant with the latest security controls and automatically disables machines if they are determined to be non-compliant.

Service engineers are only permitted to connect to one TSG at a time and multiple sessions are not allowed. However, TSGs allow Microsoft 365 service team administrators to connect to multiple servers, each with only one concurrent session, so that administrators can effectively perform their duties. Service team administrators do not have any permissions on the TSGs themselves. The TSG is used only to enforce multifactor authentication (MFA) and encryption requirements. Once the service team administrator connects to a specific server through a TSG, the specific server enforces a session limit of one per administrator.

Usage restrictions, connection, and configuration requirements for Microsoft 365 personnel are established by Active Directory group policies. These policies include the following TSG characteristics:

- Use only [FIPS 140-2](/compliance/regulatory/offering-FIPS-140-2) validated encryption
- Sessions disconnect after 15 minutes of inactivity
- Sessions automatically log off after 24 hours

Connections to TSGs also require MFA using a separate physical smart card. Service engineers are issued different smart cards for various platforms and secrets management platforms ensure secure storage of credentials. TSGs use Active Directory group policies to control who can log into remote servers, the number of allowed sessions, and idle timeout settings.

## Remote PowerShell

In addition to remote access using specially configured TSGs, service team personnel with the Service Engineer Operations Lockbox role can access certain administrative functionality on production servers using Remote PowerShell. To use this access, the user must be authorized for read-only (debug) access to the Microsoft 365 production environment. Privilege escalation is enabled the same way it is enabled for TSGs using the Lockbox process.

For remote access, each datacenter has a load-balanced virtual IP that serves as a single point of access. The available Remote PowerShell cmdlets are based on the privilege level identified in the access claim obtained during authentication. These cmdlets provide the only administrative functionality accessible by users connecting using this method. Remote PowerShell limits the scope of commands available to the engineer and is based on the level of access granted via the Lockbox process. For example, in Exchange Online, the Get-Mailbox cmdlet might be available, but the Set-Mailbox cmdlet would not.

## Resources

- [Isolation in Microsoft 365](assurance-isolation-in-microsoft-365.md)
- [Microsoft pre-employment screening](assurance-pre-employment-screening.md)[Microsoft cloud background check](assurance-cloud-background-check.md)
