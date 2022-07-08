---
title: "Security development and operations overview"
description: "Learn about security development and operations in Microsoft 365"
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

Microsoft engineering teams maintain responsibility for the security of all open-source software included in a product or service. To achieve this security at scale, Microsoft has built essential capabilities into engineering systems through Component Governance (CG), which automates open-source detection, legal requirement workflows, and alerting for vulnerable components. Automated CG tools scan builds at Microsoft for open-source components and associated security vulnerabilities or legal obligations. Discovered components are registered and submitted to the appropriate teams for business and security reviews. These reviews are designed to evaluate any legal obligations or security vulnerabilities associated with open-source components and resolve them before approving components for deployment.

## Related external regulations & certifications

Microsoft's online services are regularly audited for compliance with external regulations and certifications. Refer to the following table for validation of controls related to security development and operation.

### Azure and Dynamics 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=0625f681-1b95-48a8-bec1-e2ea3b927126&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=ae13e89f-8ff6-4ef3-972c-dffb914a3eba&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certificate](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=6f2310d4-117d-468e-a3c5-d6c8556bbc0f&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.2: Change management controls <br> A.14.2: Security in development and support processes | December 3, 2021 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=0625f681-1b95-48a8-bec1-e2ea3b927126&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certificate](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=f452fc7c-b698-4cf4-8474-85067f2df951&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.2: Change management controls <br> A.14.2: Security in development and support processes | December 3, 2021 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c771094e-0ed7-4a5f-9244-73ad6ed04bfb&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=af02eb56-4261-416b-98e3-2e713e37a77e&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=645b2f97-5bfd-4cea-b02c-c4bcda328a37&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | SDL-1: Security Development Lifecycle (SDL) methodology <br> SDL-2: Security control requirements documented in releases <br> SDL-4: Segregation of test and production environments <br> SDL-6: Malware scans on source code builds <br> SDL7: Semi-annual SDL review | September 30, 2021 <br> November 12, 2021 <br> November 12, 2021 |

### Office 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1a0939f8-1005-49fd-82f5-bd228aeb323f&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_FedRAMP_Reports) | SA-3: System Development Life Cycle | September 24, 2021 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8873fa17-9962-4be9-b0d0-086262eb84fb&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27001/27002)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=27704ac1-afbd-4c4a-a75c-53d34133b9c4&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27017)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.2: Change management controls <br> A.14.2: Security in development and support processes | March 2022 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a65bb45f-8a4a-4a44-9aaa-55235263505f&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8f3942c-845e-418f-8f6e-329dbf6efce0&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-03: Risk management <br> CA-18: Change management <br> CA-19: Change monitoring <br> CA-21: Change testing <br> CA-38: Baseline configurations <br> CA-46: Security review | September 30, 2021 |

## Resources

- [Video: Microsoft 365 security development and operation](https://www.youtube.com/watch?v=zLyY08o0k-g)
- [Microsoft's Security Development Lifecycle](https://www.microsoft.com/securityengineering/sdl)
