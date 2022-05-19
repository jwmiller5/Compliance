---
title: "Security monitoring overview"
description: "Learn about security monitoring in Microsoft 365"
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

# Security monitoring overview

## What is Microsoft's strategy for monitoring security?

Microsoft engages in continuous security monitoring of its systems to detect and respond to threats to Microsoft online services. Our key principles for security monitoring and alerting are:

- Robustness: signals and logic to detect various attack behaviors
- Accuracy: meaningful alerts to avoid distractions from noise
- Speed: ability to catch attackers quickly enough to stop them

Automation, scale, and cloud-based solutions are key pillars of our monitoring and response strategy. For us to effectively prevent attacks at the scale of some of the Microsoft online services, our monitoring systems need to automatically raise highly accurate alerts in near real time. Likewise, when an issue is detected, we need the ability to mitigate the risk at scale, we cannot rely on our team to manually fix issues machine-by-machine. To mitigate risks at scale, we use cloud-based tools to automatically apply countermeasures and provide engineers with tools to apply approved mitigation actions quickly across the environment.

## How do Microsoft online services perform security monitoring?

Microsoft online services use centralized logging to collect and analyze log events for activities that might indicate a security incident. Centralized logging tools aggregate logs from all system components, including event logs, application logs, access control logs, and network-based intrusion detection systems. In addition to server logging and application-level data, core infrastructure is equipped with customized security agents that generate detailed telemetry and provide host-based intrusion detection. We use this telemetry for monitoring and forensics.

The logging and telemetry data we collect enables 24/7 security alerting. Our alerting system analyzes log data as it gets uploaded, producing alerts in near real time. This includes rules-based alerts and more sophisticated alerting based on machine learning models. Our monitoring logic goes beyond generic attack scenarios and incorporates deep awareness of service architecture and operations. We analyze security monitoring data to continuously improve our models to detect new kinds of attacks and improve the accuracy of our security monitoring.

## How do Microsoft online services respond to security monitoring alerts?

When security events that trigger alerts require responsive action or further investigation of forensic evidence throughout the service, our cloud-based tools allow for rapid response throughout the environment. These tools include fully automated, intelligent agents that respond to detected threats with security countermeasures. In many cases, these agents deploy automatic countermeasures to mitigate security detections at scale without human intervention. When this response is not possible, the security monitoring system automatically alerts the appropriate on-call engineers, who are equipped with a set of tools that enable them to act in real time to mitigate detected threats at scale. Potential incidents are escalated to the appropriate Microsoft security response team and are resolved using the security incident response process.

## How do Microsoft online services monitor system availability?

Microsoft actively monitors its systems for indicators of resource over-utilization and abnormal use. Resource monitoring is complemented by service redundancies to help avoid unexpected downtime and provide customers with reliable access to products and services. Microsoft online service health issues are communicated promptly to customers through the Service Health Dashboard (SHD).

Azure and Dynamics 365 online services utilize multiple infrastructure services to monitor their security and health availability. The implementation of Synthetic Transaction (STX) testing allows Azure and Dynamics services to check the availability of their services. The STX framework is designed to support the automated testing of components in running services and is tested on live site failure alerts. Additionally, the Azure Security Monitoring (ASM) service has implemented centralized synthetic testing procedures to verify security alerts function as expected in both new and running services.

## Related external regulations & certifications

Microsoft's online services are regularly audited for compliance with external regulations and certifications. Refer to the following table for validation of controls related to security monitoring.

### Azure and Dynamics 365

| **External audits** | **Section** | **Latest report date** |
|:--------|:--------|:------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=0625f681-1b95-48a8-bec1-e2ea3b927126&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> <br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=ae13e89f-8ff6-4ef3-972c-dffb914a3eba&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=6f2310d4-117d-468e-a3c5-d6c8556bbc0f&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.3: Availability monitoring and capacity planning | December 3, 2021 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=0625f681-1b95-48a8-bec1-e2ea3b927126&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=f452fc7c-b698-4cf4-8474-85067f2df951&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.3: Availability monitoring and capacity planning <br> A.16.1: Management of information security incidents and improvements | December 3, 2021 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c771094e-0ed7-4a5f-9244-73ad6ed04bfb&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | IM-1: Incident management framework <br> IM-2: Incident detection configuration <br> IM-3: Incident management procedures <br> IM-4: Incident post-mortem <br> VM-1: Security event logging and collection <br> VM-12: Azure services availability monitoring <br> VM-4: Malicious events investigation <br> VM-6: Security vulnerability monitoring | September 30, 2021 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=af02eb56-4261-416b-98e3-2e713e37a77e&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=645b2f97-5bfd-4cea-b02c-c4bcda328a37&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | IM-1: Incident management framework <br> IM-2: Incident detection configuration <br> IM-3: Incident management procedures <br> IM-4: Incident post-mortem <br> PI-2: Azure portal SLA performance review <br> VM-1: Security event logging and collection <br> VM-12: Azure services availability monitoring <br> VM-4: Malicious events investigation <br> VM-6: Security vulnerability monitoring | November 12, 2021 |

### Office 365

| **External audits** | **Section** | **Latest report date** |
|:--------|:--------|:------|
| [FedRAMP](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1a0939f8-1005-49fd-82f5-bd228aeb323f&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_FedRAMP_Reports) | AC-2: Account management <br> AC-17: Remote access <br> AU-7: Audit reduction and report generation <br> SI-4: Information system monitoring <br> SI-7: Software, firmware, and information integrity <br> | September 24, 2021 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8873fa17-9962-4be9-b0d0-086262eb84fb&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> <br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27001/27002)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=118969b1-19e5-47dc-9c42-05a0daa44aec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27017)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.3: Availability monitoring and capacity planning | March, 2022 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a65bb45f-8a4a-4a44-9aaa-55235263505f&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-19: Change monitoring <br> CA-26: Security incident reporting <br> CA-29: On-call engineers <br> CA-48: Datacenter logging | September 30, 2021 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8f3942c-845e-418f-8f6e-329dbf6efce0&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-19: Change monitoring <br> CA-26: Security incident reporting <br> CA-29: On-call engineers <br> CA-30: Availability monitoring <br> CA-48: Datacenter logging | September 30, 2021 |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=328d765a-1397-4ccc-9978-95de114dd3f2&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-08: Reporting incidents <br> CUEC-10: Service contracts | September 30, 2021 |

## Resources

- [Behind the Scenes: Securing the Infrastructure Powering the Microsoft 365 Service](https://download.microsoft.com/download/c/4/5/c45b197e-f0d9-4f40-bd5f-ed8fc7d0cd8c/M365DCSecurityIntro_Whitepaper.pdf)
