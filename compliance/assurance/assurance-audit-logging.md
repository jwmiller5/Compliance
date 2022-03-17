---
title: "Audit logging overview"
description: "Learn about audit logging in Microsoft 365"
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

# Audit logging overview

## How do Microsoft online services employ audit logging?

Microsoft online services employ audit logging to detect unauthorized activities and provide accountability for Microsoft personnel. Audit logs capture details about system configuration changes and access events, with details to identify who was responsible for the activity, when and where the activity took place, and what the outcome of the activity was. Automated log analysis supports near real-time detection of suspicious behavior. Potential incidents are escalated to the appropriate Microsoft security response team for further investigation.

Microsoft online services internal audit logging captures log data from various sources, such as:

- Event logs
- AppLocker logs
- Performance data
- System Center data
- Call detail records
- Quality of experience data
- IIS Web Server logs
- SQL Server logs
- Syslog data
- Security audit logs

## How do Microsoft online services centralize and report on audit logs?

Many different types of log data are uploaded from Microsoft servers to a proprietary security monitoring solution for near real-time (NRT) analysis and an internal big data computing service (Cosmos) or Azure Data Explorer (Kusto) for long-term storage. This data transfer occurs over a FIPS 140-2-validated TLS connection on approved ports and protocols using automated log management tools.

Logs are processed in NRT using rule-based, statistical, and machine learning methods to detect system performance indicators and potential security events. Machine learning models use incoming log data and historical log data stored in Cosmos or Kusto to continuously improve detection capabilities. Security-related detections generate alerts, notifying on-call engineers of a potential incident and triggering automated remediation actions when applicable. In addition to automated security monitoring, service teams use analysis tools and dashboards for data correlation, interactive queries, and data analytics. These reports are used to monitor and improve the overall performance of the service.

For more information on security monitoring and alerting, see the [Security monitoring overview](assurance-security-monitoring.md).

![Audit data flow.](../media/assurance-audit-data-flow.png)

## How do Microsoft online services protect audit logs?

The tools used in Microsoft online services to collect and process audit records don’t allow permanent or irreversible changes to the original audit record content or time ordering. Access to Microsoft online service data stored in Cosmos or Kusto is restricted to authorized personnel. In addition, Microsoft restricts the management of audit logs to a limited subset of security team members responsible for audit functionality. Security team personnel don’t have standing administrative access to Cosmos or Kusto. Administrative access requires Just-In-Time (JIT) access approval, and all changes to logging mechanisms for Cosmos are recorded and audited. Audit logs are retained long enough to support incident investigations and meet regulatory requirements. The exact period of audit log data retention determined by the service teams; most audit log data is retained for 90 days in Cosmos and 180 days in Kusto.

## How do Microsoft online services protect user personal data that may be captured in audit logs?

Prior to uploading log data, an automated log management application uses a scrubbing service to remove any fields that contain customer data, such as tenant information and user personal data, and replace those fields with a hash value. The anonymized and hashed logs are rewritten and then uploaded into Cosmos. All log transfers occur over a TLS encrypted connection (FIPS 140-2).

## Related external regulations & certifications

Microsoft's online services are regularly audited for compliance with external regulations and certifications. Refer to the following table for validation of controls related to audit logging.

### Azure and Dynamics 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=57c75724-dab3-44c6-8aa5-46fe697998c7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=2f22dafd-6c62-469b-9bb2-39ff2cff55e2&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d1172883-7a12-45e9-aee1-d09501beba5e&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.4: Logging and monitoring | December 2, 2020 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=57c75724-dab3-44c6-8aa5-46fe697998c7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=f452fc7c-b698-4cf4-8474-85067f2df951&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.4: Logging and monitoring | December 2, 2020 |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=57c75724-dab3-44c6-8aa5-46fe697998c7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=2f22dafd-6c62-469b-9bb2-39ff2cff55e2&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=0ce91d7c-b101-48da-88a6-64c882c09e5c&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.4: Logging and monitoring | December 2, 2020 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c771094e-0ed7-4a5f-9244-73ad6ed04bfb&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | VM-1: Security event logging and collection | September 30, 2021 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=af02eb56-4261-416b-98e3-2e713e37a77e&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | C5-6: Restricted access to logs <br> VM-1: Security event logging and collection | November 12, 2021 |

### Office 365

| **External audits** | **Section** | **Latest report date** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | AU-2: Audit events <br> AU-3: Content of audit records <br> AU-4: Audit storage capacity <br> AU-5: Response to audit processing failures <br> AU-6: Audit review, analysis, and reporting <br> AU-7: Audit reduction and report generation <br> AU-8: Time stamps <br> AU-9: Protection of audit information  <br> AU-10: Non-repudiation <br> AU-11: Audit record retention <br> AU-12: Audit generation  | September 24, 2020 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=08ce227f-d1d9-4c4c-b255-4f2e4ec8f941&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Statement of Applicability](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27001/27002)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=118969b1-19e5-47dc-9c42-05a0daa44aec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Certification (27017)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.4: Logging and monitoring | March  2021 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a65bb45f-8a4a-4a44-9aaa-55235263505f&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8f3942c-845e-418f-8f6e-329dbf6efce0&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-48: Datacenter logging <br> CA-60: Audit logging | September 30, 2021 |