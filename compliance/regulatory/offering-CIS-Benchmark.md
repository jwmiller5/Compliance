---
title: Center for Internet Security (CIS) Benchmarks
description: The Center for Internet Security (CIS) has published a series of benchmarks for Microsoft products and services
keywords: Microsoft 365, compliance, offerings
ms.localizationpriority: high
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmazz
manager: laurawi
audience: itpro
ms.collection:
- MS-Compliance
- MS-Compliance-Offering
hideEdit: true
titleSuffix: Microsoft Compliance
---

# Center for Internet Security (CIS) Benchmarks

## About CIS Benchmarks

The [Center for Internet Security](https://www.cisecurity.org/) is a nonprofit entity whose mission is to 'identify, develop, validate, promote, and sustain best practice solutions for cyberdefense.' It draws on the expertise of cybersecurity and IT professionals from government, business, and academia from around the world. To develop standards and best practices, including CIS benchmarks, controls, and hardened images, they follow a consensus decision-making model.  
  
[CIS benchmarks](https://www.cisecurity.org/cis-benchmarks/) are configuration baselines and best practices for securely configuring a system. Each of the guidance recommendations references one or more [CIS controls](https://www.cisecurity.org/controls/) that were developed to help organizations improve their cyberdefense capabilities. CIS controls map to many established standards and regulatory frameworks, including the NIST Cybersecurity Framework (CSF) and NIST SP 800-53, the ISO 27000 series of standards, PCI DSS, HIPAA, and others.  
  
Each benchmark undergoes two phases of consensus review. The first occurs during initial development when experts convene to discuss, create, and test working drafts until they reach consensus on the benchmark. During the second phase, after the benchmark has been published, the consensus team reviews the feedback from the internet community for incorporation into the benchmark.  
  
CIS benchmarks provide two levels of security settings:

- **Level 1** recommends essential basic security requirements that can be configured on any system and should cause little or no interruption of service or reduced functionality.
- **Level 2** recommends security settings for environments requiring greater security that could result in some reduced functionality.

[CIS Hardened Images](https://www.cisecurity.org/blog/cis-hardened-images-now-in-microsoft-azure-marketplace/) are securely configured virtual machine images based on CIS Benchmarks hardened to either a Level 1 or Level 2 CIS benchmark profile. Hardening is a process that helps protect against unauthorized access, denial of service, and other cyberthreats by limiting potential weaknesses that make systems vulnerable to cyberattacks.

## Microsoft and the CIS Benchmarks

The Center for Internet Security (CIS) has published benchmarks for Microsoft products and services including the Microsoft Azure and Microsoft 365 Foundations Benchmarks, the Windows 10 Benchmark, and the Windows Server 2016 Benchmark. The [CIS Microsoft Azure Foundations Benchmark](https://www.cisecurity.org/benchmark/azure/) is intended for customers who plan to develop, deploy, assess, or secure solutions that incorporate Azure. The document provides prescriptive guidance for establishing a secure baseline configuration for Azure.
  
CIS benchmarks are internationally recognized as security standards for defending IT systems and data against cyberattacks. Used by thousands of businesses, they offer prescriptive guidance for establishing a secure baseline configuration. System and application administrators, security specialists, and others who develop solutions using Microsoft products and services can use these best practices to assess and improve the security of their applications.  
  
Like all CIS benchmarks, the Microsoft benchmarks were created using a consensus review process based on input from subject matter experts with diverse backgrounds spanning software development, audit and compliance, security research, operations, government, and law. Microsoft was an integral partner in these CIS efforts. For example, Office 365 was tested against the listed services, and the resulting Microsoft 365 Foundations Benchmark covers a broad range of recommendations for setting appropriate security policies that cover account and authentication, data management, application permissions, storage, and other security policy areas.  
  
In addition to the benchmarks for Microsoft products and services, CIS has published [CIS Hardened Images on Azure](https://www.cisecurity.org/cis-hardened-images/microsoft/) configured to meet CIS Benchmarks and available from Microsoft Azure Marketplace. These images include the CIS Hardened Images for Windows Server 2016 and Windows Server 2019, as well as many versions of Linux. All CIS Hardened Images that are available in Azure Marketplace are certified to run on Microsoft Azure. As [stated by CIS](https://www.cisecurity.org/blog/cis-hardened-images-now-in-microsoft-azure-marketplace/), 'they've been pre-tested for readiness and compatibility with the Microsoft Azure public cloud, Microsoft Cloud Platform hosted by service providers through the Cloud OS Network, and on-premises private cloud Windows Server Hyper-V deployments managed by customers'.

[CIS Hardened Images](https://www.cisecurity.org/cis-hardened-images/) are securely configured virtual machine images based on CIS Benchmarks hardened to either a Level 1 or Level 2 CIS Benchmark profile. Hardening is a process that helps protect against unauthorized access, denial of service, and other cyber threats by limiting potential weaknesses that make systems vulnerable to cyber attacks. CIS Hardened Images are available on both Azure and Azure Government.

For additional customer assistance, Microsoft provides [Azure Blueprints](https://azure.microsoft.com/services/blueprints/), which is a service that helps you deploy and update cloud environments in a repeatable manner using composable artifacts such as Azure Resource Manager templates to provision resources, role-based access controls, and policies. Resources provisioned through Azure Blueprints adhere to an organization's standards, patterns, and compliance requirements. The overarching goal of Azure Blueprints is to help automate compliance and cybersecurity risk management in cloud environments. To help you deploy a core set of policies for any Azure-based architecture that must implement CIS Azure Foundations Benchmark recommendations, Microsoft has published the [Azure Blueprint for CIS Microsoft Azure Foundations Benchmark](/azure/governance/blueprints/samples/cis-azure-1-3-0). When assigned to an architecture, resources are evaluated by Azure Policy for compliance with assigned policy definitions.

## Microsoft in-scope cloud platforms & services

- [Azure and Azure Government](https://aka.ms/AzureCompliance)
- [Office and Microsoft 365](https://aka.ms/o365-compliance-framework)
- SQL Server
- Windows 10
- Windows Server 2016

## Audits, reports, and certificates

Get a [complete list of CIS benchmarks](https://www.cisecurity.org/cis-benchmarks/) for Microsoft products and services.

- [CIS Azure Foundations Benchmark](https://www.cisecurity.org/benchmark/azure/)
- [CIS Microsoft 365 Foundations Benchmark](https://www.cisecurity.org/benchmark/microsoft_office/)
- [Windows 10 Benchmark](https://www.cisecurity.org/benchmark/microsoft_windows_desktop/)
- [Windows Server 2016 Benchmark](https://www.cisecurity.org/benchmark/microsoft_windows_server/)

## How to implement

- [CIS Benchmark for Azure](https://azure.microsoft.com/mediahandler/files/resourcefiles/cis-microsoft-azure-foundations-security-benchmark/CIS_Microsoft_Azure_Foundations_Benchmark_v1.0.0.pdf): Get prescriptive guidance for establishing a secure baseline configuration for Azure.  
- [Microsoft 365 security roadmap](/microsoft-365/security/office-365-security/security-roadmap): Minimize the potential of a data breach or compromised account by following this roadmap.
- [Windows security baselines](/windows/security/threat-protection/windows-security-baselines): Follow these guidelines for effective use of security baselines in your organization.
- [CIS Controls Cloud Companion Guide](https://www.cisecurity.org/white-papers/cis-controls-cloud-companion-guide/): Get guidance on applying security best practices in CIS Controls Version 7 to cloud environments.

## Frequently asked questions

**Will following CIS Benchmark settings ensure the security of my applications?**

CIS benchmarks establish the basic level of security for anyone adopting in-scope Microsoft products and services. However, they shouldn't be considered as an exhaustive list of all possible security configurations and architecture but as a starting point. Each organization must still evaluate its specific situation, workloads, and compliance requirements and tailor its environment accordingly.

**How often are CIS Benchmarks updated?**

The release of revised CIS Benchmarks changes depending on the community of IT professionals who developed it and on the release schedule of the technology the benchmark supports. CIS distributes monthly reports that announce new benchmarks and updates to existing benchmarks. To receive these, register for the [CIS Workbench](https://workbench.cisecurity.org/) (it's free) and check Receive newsletter in your profile.

**Who contributed to the development of Microsoft CIS Benchmarks?**

CIS notes that its 'Benchmarks are developed through the generous volunteer efforts of subject matter experts, technology vendors, public and private CIS Benchmark community members, and the CIS Benchmark Development team.' For example, you'll find a list of Azure contributors on [CIS Microsoft Azure Foundations Benchmark v1.0.0 Now Available](https://www.cisecurity.org/blog/cis-microsoft-azure-foundations-benchmark-v1-0-0-now-available/).

## Use Microsoft Compliance Manager to assess your risk

[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft Purview portal](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks. Compliance Manager offers a premium template for building an assessment for this regulation. Find the template in the **assessment templates** page in Compliance Manager. Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).

## Resources

- [Azure compliance documentation](/azure/compliance/)
- [Azure enables a world of compliance](https://azure.microsoft.com/resources/azure-enables-a-world-of-compliance/)
- [Microsoft compliance offerings](/compliance/regulatory/offering-home)
- [Compliance on the Microsoft Trust Center](https://www.microsoft.com/trust-center/compliance/compliance-overview)
- [CIS Microsoft Azure Foundations Benchmark](https://www.cisecurity.org/benchmark/azure/) provides a step-by-step checklist for securing Azure.
- [CIS Hardened Images on Microsoft Azure](https://www.cisecurity.org/cis-hardened-images/microsoft/) are Azure certified and preconfigured to the security recommendations of the CIS Benchmarks.  They're available on both Azure and Azure Government.
- [Azure Blueprint for CIS Microsoft Azure Foundations Benchmark](/azure/governance/blueprints/samples/cis-azure-1-3-0) helps customers deploy a core set of policies for any Azure-based architecture that must implement CIS Azure Foundations Benchmark recommendations.
- [Azure Policy recommendation mapping](/azure/governance/policy/samples/cis-azure-1-3-0) provides details on policy definitions included within the above Blueprint and how these policy definitions map to the compliance domains and controls in CIS Microsoft Azure Foundations Benchmark. When assigned to an architecture, resources are evaluated by Azure Policy for non-compliance with assigned policy definitions.
- [CIS Controls Cloud Companion Guide](https://www.cisecurity.org/white-papers/cis-controls-cloud-companion-guide/) provides guidance on applying security best practices in CIS Controls Version 7 to cloud environments.
- [CIS Microsoft 365 Foundations Benchmark](https://www.cisecurity.org/benchmark/microsoft_office/) provides prescriptive guidance for establishing a secure baseline configuration for Microsoft 365.
- [Windows 10 security policy settings](/windows/security/threat-protection/security-policy-settings/security-policy-settings)
- [Windows 10 enterprise security](/windows/security/index)
