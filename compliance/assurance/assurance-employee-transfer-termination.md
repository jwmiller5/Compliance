---
title: "Microsoft employee transfer and termination"
description: "Learn about the Microsoft employee transfer and termination process in Microsoft 365"
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

# Microsoft employee transfer and termination

Microsoft, like every other organization, handles employee transfers and terminations as a part of their normal business operation. When an employee changes positions or leaves the company, it is essential to revoke inappropriate access in a timely manner. To facilitate efficient access changes and access revocations, Microsoft uses standardized procedures and automated processes to coordinate the Human Resources Information System (HRIS) with the Identity Management (IDM) system. Automated orchestration between these two systems is essential to maintaining operational consistency, safeguarding Microsoft's online services and data, preventing privilege creep, and reducing risks related to insider threats.

Microsoft online services are designed to operate without standing administrative access to production environments for our engineers. Microsoft uses a Just-In-Time (JIT), Just-Enough-Access (JEA) model to provide engineers with the temporary access needed to support their service when required. To request and use a service team account for JIT access, engineers must request and maintain eligibilities through the IDM tool. When employees are transferred or terminated, their service team account and related eligibilities are automatically modified to prevent inappropriate access.

## Transfer and reassignment

Employee transfers are initiated through a transfer transaction request by the employee's manager. The manager creates a requisition and engages with Global Talent Acquisition for the offer letter process. Once the employee accepts the offer for the new role, HR services completes the transfer in the HR core tools, triggering IDM to set an expiration date for all the employee's eligibilities. The employee must submit a request and receive approval from their new manager to retain their eligibilities. Failure to submit a request or receive manager approval results in the revocation of the transferred employee's eligibilities. For transfers that include specific security implications, system accesses and security group memberships are reevaluated immediately to reflect their new role.

## Termination

Microsoft uses clearly defined policies and procedures to promptly revoke physical and logical access to Microsoft systems and resources when an employee is terminated. When an employee gives their notice, the employee's manager enters the termination date into the HRIS. Following the employee's last working day, the HRIS marks the employee as terminated and shares the information to IDM, which removes all service team accounts and eligibilities automatically.

For involuntary terminations, HR works with the employee's manager to follow the appropriate steps to terminate and offboard the employee. Similar to a voluntary termination, the termination information is entered into the HRIS along with any necessary steps such as effective date coordination, access removal, and any other steps relative to transitioning out of role.
