---
title: "Security development and operations overview"
description: "Learn about security development and operations in Microsoft 365"
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

# Security development and operations overview

## How does Microsoft implement secure development practices?

Microsoft's Security Development Lifecycle (SDL) is a security assurance process focused on developing and operating secure software. The SDL provides detailed, measurable security requirements for developers and engineers at Microsoft to reduce the number and severity of vulnerabilities in our products and services. All Microsoft software development teams must follow SDL requirements, and we continuously update the SDL to reflect the changing threat landscape, industry best practices, and regulatory standards for compliance.

## How does Microsoft's SDL improve application security?

The SDL process at Microsoft can be thought of in terms of five phases of development: requirements, design, implementation, verification, and release. It begins by defining software requirements with security in mind. To do meet this goal, we ask security-relevant questions about what the application must accomplish. Does the application need to collect sensitive data? Will the application perform sensitive or important tasks? Does the application need to accept input from untrusted sources?

Once relevant security requirements have been identified, we design our software to incorporate security features that meet these requirements. Our developers implement SDL and design requirements in the code, which we verify through manual code review, automated security tooling, and penetration testing. Finally, before code can be released, new features and material changes undergo final security and privacy review to ensure all requirements are met.

## How does Microsoft test source code for common vulnerabilities?

To support our developers in implementing security requirements during code development and after release, Microsoft provides a suite of secure development tools to automatically check source code for security flaws and vulnerabilities. Microsoft defines and publishes a list of approved tools for our developers to use, such as compilers and development environments, along with the built-in security checks executed automatically within Microsoft build pipelines. Our developers use the latest versions of approved tools to take advantage of new security features.

Before code can be checked into a release branch, the SDL requires manual code review by a separate reviewer. Code reviewers check for coding errors and verify that code changes meet SDL and design requirements, pass functional and security tests, and perform reliably. They also review associated documentation, configs, and dependencies to ensure code changes are documented appropriately and will not cause unintended side-effects. If a reviewer finds problems during code review, they can ask the submitter to resubmit the code with suggested changes and additional testing. Code reviewers may also decide to block check-in entirely for code that does not meet requirements. Once the code has been deemed satisfactory by the reviewer, the reviewer provides approval, which is required before code can proceed to the next deployment phase.

In addition to secure development tools and manual code review, Microsoft enforces SDL requirements using automated security tooling. Many of these tools are built into the commit pipeline and automatically analyze code for security flaws as it is checked in and as new builds are compiled. Examples include static code analysis for common security flaws and credential scanners that analyze code for embedded secrets. Issues uncovered by automated security tools must be fixed before new builds can pass security review and be approved for release.

## How does Microsoft manage open-source software?

Microsoft has adopted a high-level strategy for managing open-source security, which uses tools and workflows designed to:

- Understand which open-source components are being used in our products and services.
- Track where and how those components are used.
- Determine whether those components have any vulnerabilities.
- Respond properly when vulnerabilities are discovered that affect those components.

Microsoft engineering teams maintain responsibility for the security of all open-source software included in a product or service. To achieve this security at scale, Microsoft has built essential capabilities into engineering systems through CG, which automates open-source detection, legal requirement workflows, and alerting for vulnerable components. Automated CG tools scan builds at Microsoft for open-source components and associated security vulnerabilities or legal obligations. Discovered components are registered and submitted to the appropriate teams for business and security reviews. These reviews are designed to evaluate any legal obligations or security vulnerabilities associated with open-source components and resolve them before approving components for deployment.

## Related external regulations & certifications

Microsoft's online services are regularly audited for compliance with external regulations and certifications. Refer to the following table for validation of controls related to security development and operation.

### Azure and Dynamics 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.2: Change management controls <br> A.14.2: Security in development and support processes | December 2, 2020 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.2: Change management controls <br> A.14.2: Security in development and support processes | December 2, 2020 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> | [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | SDL-1: Security Development Lifecycle (SDL) methodology <br> SDL-2: Security control requirements documented in releases <br> SDL-4: Segregation of test and production environments <br> SDL-6: Malware scans on source code builds <br> SDL7: Semi-annual SDL review | March 31, 2021 |

### Office 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | SA-3: System Development Life Cycle | September 24, 2020 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.2: Change management controls <br> A.14.2: Security in development and support processes | April 20, 2021 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-03: Risk management <br> CA-18: Change management <br> CA-19: Change monitoring <br> CA-21: Change testing <br> CA-38: Baseline configurations <br> CA-46: Security review | December 24, 2020 |

## Resources

- [Microsoft's Security Development Lifecycle](https://www.microsoft.com/securityengineering/sdl)
