---
title: "Incident management overview"
description: "Learn about incident management in Microsoft 365"
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

# Incident management overview

## What is a security incident?

Microsoft defines a security incident in its online services as a confirmed breach of security leading to the accidental or unlawful destruction, loss, alteration, unauthorized disclosure of, or access to customer data or personal data while being processed by Microsoft. For example, unauthorized access to Microsoft online services infrastructure and exfiltration of customer data would constitute a security incident, while compliance events that don't affect the confidentiality, integrity, or availability of services or customer data aren't considered security incidents.

## How does Microsoft respond to security incidents?

Whenever there's a security incident, Microsoft strives to respond quickly and effectively to protect Microsoft services and customer data. Microsoft employs an incident response strategy designed to investigate, contain, and remove security threats quickly and efficiently.

Microsoft cloud services are continuously monitored for signs of compromise. In addition to automated security monitoring and alerting, all employees receive annual training to recognize and report signs of potential security incidents. Any suspicious activity detected by employees, customers, or security monitoring tools are escalated to Service-specific Security Response teams for investigation. All service operations teams, including Service-specific Security Response teams, maintain a deep on-call rotation to ensure resources are available for incident response 24x7x365. Our on-call rotations enable Microsoft to mount an effective incident response at any time or scale, including widespread or concurrent events.

When suspicious activity is detected and escalated, Service-specific Security Response teams initiate a process of **analysis, containment, eradication, and recovery**. These teams coordinate analysis of the potential incident to determine its scope, including any impact to customers or customer data. Based on this analysis, Service-specific Security Response teams work with impacted service teams to develop a plan to contain the threat and minimize the impact of the incident, eradicate the threat from the environment, and fully recover to a known secure state. Relevant service teams implement the plan with support from Service-specific Security Response teams to ensure the threat is successfully eliminated and impacted services undergo a complete recovery.

After an incident is resolved, service teams implement any lessons learned from the incident to better prevent, detect, and respond to similar incidents in the future. Select security incidents, especially those incidents that are customer-impacting or result in a data breach, undergo a full incident post-mortem. The post-mortem is designed to identify technical lapses, procedural failures, manual errors, and other process flaws that might have contributed to the incident or that were identified during the incident response process. Improvements identified during the post-mortem are implemented with coordination from Service-specific Security Response teams to help prevent future incidents and improve detection and response capabilities.

## How and when are customers notified of security or privacy incidents?

Whenever Microsoft becomes aware of a breach of security involving unauthorized loss, disclosure, or modification of customer data, Microsoft notifies affected customers within 72 hours as outlined in the Data Protection Addendum (DPA) of the Online Services Terms (OST). The notification timeline commitment begins when the official security incident declaration occurs. Upon declaring a security incident, the notification process occurs as expeditiously as possible, without undue delay.

Notifications include a description of the nature of the breach, approximate user impact, and mitigation steps (if applicable). If Microsoft's investigation isn't complete at the time of initial notification, the notification will also indicate next steps and timelines for subsequent communication.

If a customer becomes aware of an incident that could have an impact on Microsoft, including but not limited to a data breach, the customer is responsible for promptly notifying Microsoft of the incident as defined in the DPA.

## Related external regulations & certifications

Microsoft's online services are regularly audited for compliance with external regulations and certifications. Refer to the following table for validation of controls related to incident management.

### Azure and Dynamics 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=57c75724-dab3-44c6-8aa5-46fe697998c7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=2f22dafd-6c62-469b-9bb2-39ff2cff55e2&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d1172883-7a12-45e9-aee1-d09501beba5e&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.16.1: Management of information security incidents and improvements | December 2, 2021 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=57c75724-dab3-44c6-8aa5-46fe697998c7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=f452fc7c-b698-4cf4-8474-85067f2df951&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.16.1: Management of information security incidents and improvements | December 2, 2021 |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=57c75724-dab3-44c6-8aa5-46fe697998c7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=2f22dafd-6c62-469b-9bb2-39ff2cff55e2&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=0ce91d7c-b101-48da-88a6-64c882c09e5c&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.9.1: Notification of a data breach involving PII  | December 2, 2021 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c771094e-0ed7-4a5f-9244-73ad6ed04bfb&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | IM-1: Incident management framework <br> IM-2: Detection mechanisms and alerting <br> IM-3: Incident response execution <br> IM-4: Incident postmortems <br> IM-6: Incident response testing <br> OA-7: On-call engineer access | September 30, 2021 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=af02eb56-4261-416b-98e3-2e713e37a77e&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=645b2f97-5bfd-4cea-b02c-c4bcda328a37&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CCM-9: Forensic procedures <br> CUEC: Reporting incidents <br> IM-1: Incident management framework <br> IM-2: Detection mechanisms and alerting <br> IM-3: Incident response execution <br> IM-4: Incident postmortems <br> IM-6: Incident response testing <br> OA-7: On-call engineer access <br> SOC2-6: Customer Support website <br> SOC2-9: Service dashboards | November 12, 2021 |

### Office 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | IR-4: Incident handling <br> IR-6: Incident reporting <br> IR-8: Incident response plan | September 24, 2020 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=08ce227f-d1d9-4c4c-b255-4f2e4ec8f941&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27001/27002)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=118969b1-19e5-47dc-9c42-05a0daa44aec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27017)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.16.1: Management of information security incidents and improvements | March  2021 |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=08ce227f-d1d9-4c4c-b255-4f2e4ec8f941&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=43e89534-f48d-42ea-a7a7-3523ff516036&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports)  | A.10.1: Notification of a data breach involving PII  | April 20, 2021 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a65bb45f-8a4a-4a44-9aaa-55235263505f&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-26: Security incident reporting <br> CA-47: Incident response | September 30, 2021 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8f3942c-845e-418f-8f6e-329dbf6efce0&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-12: Service level agreements (SLAs) <br> CA-13: Incident response guides <br> CA-15: Service health notifications  <br>  <br> CA-26: Security incident reporting <br> CA-29: On-call engineers <br> CA-47: Incident response | September 30, 2021 |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=328d765a-1397-4ccc-9978-95de114dd3f2&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-08: Reporting incidents  | September 30, 2021  |

## Resources

- [Online Services Terms (OST)](https://www.microsoft.com/licensing/product-licensing/products)
- [Data Protection Addendum (DPA)](https://www.microsoft.com/licensing/product-licensing/products)
- [Microsoft Cloud Incident Management Implementation Guidance for Azure and Office 365](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=a8a7cb87-9710-4d09-8748-0835b6754e95&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_FAQ_and_White_Papers)
- [Office 365 - Third-Party Vulnerability Assessment of Office 365 - 2019](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=e85e478f-2491-435d-9c1b-2f0ad7ca8e56&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_Pen_Test_and_Security_Assessments)
