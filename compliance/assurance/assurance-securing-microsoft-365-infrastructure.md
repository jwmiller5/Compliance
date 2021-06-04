---
title: "Securing the Microsoft 365 infrastructure"
description: "Learn how Microsoft secures the Microsoft 365 infrastructure."
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

# Securing the Microsoft 365 infrastructure

Microsoft 365 is one of the largest enterprise and consumer cloud services in the world and continues to grow rapidly, both in customer base, products, and features. Customers turn to Microsoft 365 not only for its world-class productivity solutions, but to help protect their most sensitive information from the constantly evolving cyber threat landscape. It is Microsoft's top priority to keep customer data secure and maintain customer trust.

Securing a system of this scale and complexity is not possible if security is an afterthought, it is only effective if security is integrated during the initial design process. It requires a robust threat detection system with prompt responses from both automated systems and highly skilled engineers. Continuous assessment and validation of these systems is essential to ensure secure configurations remain intact and previously unknown vulnerabilities are identified.

## Core security principles

Seven security principles lay the foundation for our framework of *protecting* the Microsoft 365 services from threats, *detecting and responding* to any threats, and continuously *assessing* the security posture and improving services based on the results of those assessments.

- **Data privacy**: Customers own their data and Microsoft is the custodian. Microsoft 365 services are designed to operate without engineers accessing customer data, unless explicitly requested and approved by the customer.
- **Assume breach**: Personnel and services are treated as though compromise is a real possibility.
- **Least privilege**: Access and permissions to resources are limited to only what is necessary to perform needed tasks.
- **Breach boundaries**: Identities and infrastructure in one boundary are isolated from resources in other boundaries. Compromise of one boundary should not lead to compromise of another.
- **Service fabric integrated security**: Security priorities and requirements are built into the design of new features and capabilities, ensuring that a strong security posture scales with each service.
- **Automated and automatic**: Microsoft focuses on developing durable products and architectures that can intelligently and automatically enforce service security, while giving Microsoft engineers the ability to safely manage responses to security threats at scale.
- **Adaptive security**: Microsoft security capabilities adapt to and are enhanced by machine learning models, routine penetration testing, and automated assessments.

## Protection

### Access control

By default, personnel responsible for developing and maintaining Microsoft 365 services have Zero Standing Access (ZSA) to the service infrastructure. While Microsoft strives to hire only the best engineers and rigorous background checks are required, Microsoft does not assume that they are trusted by default in operating services. Additionally, when engineers are approved for privileged access, they are only granted access for a limited duration to perform only the actions needed for a specific scope of the service infrastructure. Microsoft refers to these policies as Just-in-Time (JIT) and Just-Enough-Access (JEA) which are implemented through a system called Lockbox.

To acquire elevated privileges, Microsoft engineers submit a request for the specific task and specify the time frame to perform it. Once approved, Lockbox generates a specialized JIT account with the ability to perform only the requested task. Actions usually take the form of automated workflows that securely perform any troubleshooting or recovery required. In rare instances when direct access to the infrastructure is necessary, strictly monitored Privileged Access Workstations (PAWs) are required.

Rogue users and compromised accounts are a real possibility in any organization, and our access control system are designed to protect against these threats.

For more information about access control, see [Identity and access management overview](/assurance-identity-and-access-management.md).

### Encryption

While access controls provide a vital role in defending Microsoft 365 services, encryption is used throughout the data lifecycle to further protect confidentiality and privacy for Microsoft customers.

Data in transit between client machines, Microsoft 365 servers, and non-Microsoft 365 servers is encrypted using TLS 1.2. We regularly review the ciphers and protocols in use, adding improved protocols when available and removing weaker ones as needed.

Customer content at rest on Microsoft servers is encrypted at the volume-level using BitLocker. Application-level encryption can additionally be applied using keys managed by either Microsoft or the customer. Access to Microsoft-managed keys is only possible when authorized and approved through the JIT and JEA process.

For more information about encryption in Microsoft 365, see [Encryption and key management overview](assurance-encryption.md).

### Network isolation

In line with the principle of least privilege, Microsoft 365 restricts communication between different parts of the service infrastructure to only what is necessary to operate. All network traffic is denied by default, with only explicitly defined communication being allowed. This restriction establishes breach boundaries throughout the infrastructure. Teams that would like to add new network paths to accommodate a new feature to their service must have the request evaluated and approved before it can be opened.

For more information about network isolation in Microsoft 365, see [Microsoft 365 isolation controls](/microsoft-365/enterprise/microsoft-365-isolation-controls).

## Detection & Response

### Security monitoring

Security monitoring at Microsoft's massive scale is only possible by generating highly accurate alerts using automated cloud-based solutions. Audit logs from each service and telemetry data gathered from throughout the core infrastructure is sent to a proprietary centralized near-real-time processing and alerting solution.

Detected threats are remediated using automatically triggered actions when possible. When automated solutions are unsuccessful or incapable of resolving the issue, on-call Microsoft engineers immediately take action to mitigate the threat.

For more information about security monitoring in Microsoft 365, see [Security monitoring overview](assurance-security-monitoring.md).

## Assessment

### Automated assessments

Regardless of how a system is designed, the security posture can degrade due to intentional and unintentional configuration drift over time. Automated tools constantly assess Microsoft 365 systems that look for unpatched and misconfigured services. This assessment is often referred to as patching, anti-virus, vulnerability, and configuration scanning (PAVC).

Our architecture is also frequently validated, identifying instances such as unused open ports and accounts with standing administrative access. Any services that drift from a pre-defined desired state are automatically brought back into alignment.

For more information about security monitoring in Microsoft 365, see [Vulnerability management overview](assurance-vulnerability-management.md).

### Attack simulation and penetration testing

Microsoft 365's top priority is to prevent attacks from infiltrating defenses. Microsoft 365 has a dedicated team of security experts who are constantly conducting simulated attacks to identify previously unknown vulnerabilities and to provide a constant stream of rich data to improve security monitoring capabilities. These simulated attacks take the form of frequent automated small-scale attacks and expert-driven deep dives. From these activities, Microsoft evaluates the ability to detect, respond, and evict attackers.

For more information about security monitoring in Microsoft 365, see [Attack simulation in Microsoft 365](assurance-monitoring-and-testing.md).

## Resources

[Behind the Scenes: Securing the Infrastructure Powering the Microsoft 365 Service](https://download.microsoft.com/download/c/4/5/c45b197e-f0d9-4f40-bd5f-ed8fc7d0cd8c/M365DCSecurityIntro_Whitepaper.pdf)
