---
title: "Network security"
description: "Learn about network security in Microsoft 365"
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

# Network security overview

## How do Microsoft online services secure the network boundary?

Microsoft online services employ multiple strategies for securing its network boundary, including automated detection and prevention of network-based attacks, specialized firewall devices, and Exchange Online Protection (EOP) for anti-spam and anti-malware protection. In addition, Microsoft online services separate their production environments into logically isolated network segments, with only necessary communication permitted between segments. Network traffic is secured using additional network firewalls at boundary points to help detect, prevent, and mitigate network attacks.

## How do Microsoft online services defend against DDoS attacks?

Microsoft's large internet presence insulates it from the negative effects of many distributed denial-of-service (DDoS) attacks. Distributed instances of each Microsoft online service and multiple routes to each service limit the impact of DDoS attacks against the system. This redundancy improves Microsoft online services' ability to absorb DDoS attacks and increases the amount of time available to detect and mitigate DDoS attacks before they impact service availability.

In addition to Microsoft's redundant system architecture, Microsoft uses sophisticated detection and mitigation tools to respond to DDoS attacks. Special-purpose firewalls monitor and drop unwanted traffic before it crosses the boundary into the network, reducing stress on systems located inside the network boundary. To further protect our cloud services, Microsoft utilizes a DDoS defense system deployed as part of Microsoft Azure. The Azure DDoS defense system is designed to withstand attacks from the outside and from other Azure tenants.

## How does Microsoft protect users against spam and malware being uploaded or sent through online services?

Microsoft online services build antimalware protection into services that might be vectors for malicious code, such as Exchange Online and SharePoint Online. Exchange Online Protection (EOP) scans all emails and email attachments for malware as they enter and exit the system, preventing infected messages and attachments from being delivered. Advanced spam filtering is automatically applied to inbound and outbound messages to help prevent customer organizations from receiving and sending spam. This layer of protection guards against attacks that take advantage of unsolicited or unauthorized email, such as phishing attacks. SharePoint Online uses the same virus detection engine to selectively scan uploaded files for malware. If a file is marked as infected, users are prevented from downloading or syncing the file to protect client endpoints. Similarly, Azure compares hashes related to files uploaded to Azure Storage to those hashes of known malware. When matches are found, an alert is raised in Azure Security Center where a decision is made about the legitimacy of the alert and how it should be addressed.

## Related external regulations & certifications

Microsoft's online services are regularly audited for compliance with external regulations and certifications. Refer to the following table for validation of controls related to network security.

### Azure and Dynamics 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=af02eb56-4261-416b-98e3-2e713e37a77e&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=645b2f97-5bfd-4cea-b02c-c4bcda328a37&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | VM-1: Security event logging <br> VM-3: Intrusion detection and monitoring <br> VM-4: Malicious events investigation <br> VM-6: Vulnerability scanning <br> VM-7: Network device configuration <br> VM-8: Penetration testing <br> VM-9: Network device security event logging <br> VM-13: Network device vulnerability mitigation | March 31, 2021 <br> November 12, 2021 <br> November 12, 2021 |

### Office 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | SC-5: Denial of service protection <br> SC-7: Boundary protection <br> SI-2: Flaw remediation <br> SI-3: Malicious code protection <br> SI-8: Spam protection | September 24, 2020 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-27: Vulnerability Scanning | December 24, 2020 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-27: Vulnerability Scanning <br> CA-45: Anti-malware | December 24, 2020 |