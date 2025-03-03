---
title: "Microsoft 365 reporting features"
description: Learn about various reporting features within Microsoft 365, including Azure Active Directory and Exchange Online.
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
- MS-Compliance
- MS-Compliance-Assurance
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
---

# Microsoft 365 reporting features

Reporting features in Microsoft 365 provides various audit reports for Azure Active Directory (Azure AD), Exchange Online, device management, supervisory review, and data loss prevention (DLP). These reports are different and separate from the Microsoft 365 activity reports.

## Microsoft 365 Reports dashboard

The Reports dashboard in the Microsoft 365 admin center preview displays usage activity across Microsoft 365. Microsoft 365 global administrators, or an Exchange Online, SharePoint Online, or Skype for Business administrator, can get granular insight into the usage of that service. For example, the number of users in a particular Microsoft 365 service, the number of users that have activated Microsoft 365 Apps for enterprise (previously named Office 365 ProPlus), and how much mail is flowing through the organization. Reports are available for the last 7, 30, 90, and 180 days.

The following reports are available:

- [Email activity report](https://support.office.com/article/Office-365-Reports-in-the-admin-center-preview--Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)
- [Microsoft Office activations report](https://support.office.com/article/Office-365-Reports-in-the-admin-center-preview--Microsoft-Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)
- [SharePoint Online Site usage report](https://support.office.com/article/Office-365-Reports-in-the-admin-center-preview--SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)
- [OneDrive for Business usage report](https://support.office.com/article/Office-365-Reports-in-the-Admin-Center-Preview--OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)
- [Yammer activity report](https://support.office.com/article/View-the-Yammer-Activity-report-in-the-Office-365-admin-center-preview-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)
- [Skype for Business activity report](/SkypeForBusiness/skype-for-business-online-reporting/activity-report)
- [Skype for Business Peer-to-Peer activity report](/SkypeForBusiness/skype-for-business-online-reporting/peer-to-peer-activity-report)
- [Skype for Business Conference Organizer report](/SkypeForBusiness/skype-for-business-online-reporting/conference-organizer-activity-report)
- [Skype for Business Conference Participant activity report](/SkypeForBusiness/skype-for-business-online-reporting/conference-participant-activity-report)

For more information, see [Activity Reports in the Microsoft 365 admin center](https://support.office.com/article/activity-reports-in-the-office-365-admin-center-0d6dfb17-8582-4172-a9a9-aed798150263).

## Azure AD Reports

Microsoft 365 uses Azure AD for authentication and identity management. Microsoft 365 administrators use reports generated by Azure to identify unusual activity and unauthorized access to their data. You can use access and usage reports in Azure AD to gain visibility into the directory integrity and security for your organization. With this information, you can identify and mitigate possible security risks.

Azure AD reports can be exported to Microsoft Excel and correlated with other data from Microsoft 365. For example, the results of an audit log search can provide insight into access, authentication, and application-level activities. Advanced anomaly and resource usage reports are available with Azure AD Premium. These advanced reports help improve your security posture and help you respond to potential threats by applying analytics about device access and application usage. For more information, see [Azure Active Directory reporting](/azure/active-directory/reports-monitoring/overview-reports/).

## Exchange Online Audit Reports

Exchange Online audit reports include details on mailbox access and changes made by administrators to your Exchange Online tenant. With mailbox auditing, you can use the tasks in the following table to run reports and export Exchange Online audit logs.

> [!NOTE]
> You must enable mailbox audit logging for each mailbox so that audited events are saved in the audit log for that mailbox. If mailbox audit logging isn't enabled for a mailbox, events for that mailbox won't be saved in the audit log and won't appear in mailbox audit reports. For more information, see [enable mailbox auditing](https://support.office.com/article/Enable-mailbox-auditing-in-Office-365-aaca8987-5b62-458b-9882-c28476a66918).

| Task | Description |
|----------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Run a non-owner mailbox access report](/exchange/security-and-compliance/exchange-auditing-reports/non-owner-mailbox-access-report) | Displays the list of mailboxes accessed by someone other than the owner of the mailbox. The report contains information about who accessed the mailbox, the actions they took in the mailbox, and whether the actions were successful. |
| [Export mailbox audit logs](/exchange/security-and-compliance/exchange-auditing-reports/export-mailbox-audit-logs) | Mailbox audit logs contain information on access and actions in a mailbox taken by a user other than the mailbox owner. Administrators can specify mailboxes along with a date range to generate reports. The logs are exported in XML, attached to a message, and sent to specific users as determined by the administrator. |
| [Run an administrator role group report](/Office365/SecurityCompliance/eop/run-an-administrator-role-group-report-in-eop-eop) | The administrator role group assigns administrative privileges to users. These privileges allow users to perform administrative tasks such as reset passwords, create or modify mailboxes, and assign admin privileges to other users. The admin role group report shows changes to role groups, including the addition or removal of members. |
| [View the admin audit log](/exchange/security-and-compliance/exchange-auditing-reports/view-administrator-audit-log) | The admin audit log report lists all create, update, and delete functions performed by administrators in Exchange Online. Log entries provide information on which cmdlet was run, what parameters were used, who ran the cmdlet, and what objects were affected. |
| [Mailbox content search and hold](/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) | Provides details of any changes to In-Place eDiscovery or In-Place Hold settings on mailboxes. |
| [Export the admin audit log](/exchange/security-and-compliance/exchange-auditing-reports/search-role-group-changes) | The admin audit log records specific administrative actions such as create, update, and delete in Exchange Online. The results from the log are exported to XML and administrators can choose to send this log to a set of users. |
| [Run a per-mailbox litigation hold report](/exchange/security-and-compliance/exchange-auditing-reports/per-mailbox-litigation-hold-report) | Provides details of any changes to litigation hold settings on mailboxes. |
| [View and export the external admin audit log](/exchange/security-and-compliance/exchange-auditing-reports/view-external-admin-audit-log) | Contains details of actions performed by external administrators. The entries provide information on which cmdlet was run, what parameters were used, and any actions that create, modify, or delete objects in Exchange Online. |

## Device compliance Reports

You manage and secure mobile devices connected to your subscription using Basic Mobility and Security for Microsoft 365. Mobile devices used to access work email, calendar, contacts, and documents play a significant part in making sure that employees are able to work anytime and from anywhere. It's critical that you protect your organization's information. You use Basic Mobility and Security for Microsoft 365 to set device security policies and access rules. If lost or stolen, you also use Basic Mobility and Security for Microsoft 365 to wipe mobile devices.

Basic Mobility and Security compliance reports provide an overview of policies set up by an organization to secure mobile devices that access Microsoft 365 data. The report allows filtering of devices by compliance status, reported violations, blocked devices, and how many devices wiped as a result of security policies. For more information, see [Overview of Basic Mobility and Security for Microsoft 365](https://support.microsoft.com/office/overview-of-basic-mobility-and-security-for-microsoft-365-faa7d8e5-645d-4d59-839c-c8d4c1869e4a).

## Data loss prevention

DLP policies help manage the security and flow of information in an organization. You can set up policies to block access to content, encrypt data, or notify users of policy and policy violations using in-application DLP Policy Tips. DLP reports provide insight into the number of policy and rule matches, overrides, and false positives.

You use the Microsoft 365 admin center to view information about the number of messages detected by your DLP policies. DLP reports provide insights into policy and rule matches for sent and received mail. You can also view the number of matches, overrides, and false positives for each policy within the past 24 hours using the Exchange admin center. If you download an Excel report, you can view even more detail, such as who sent which message, on what day, and what policy matches were triggered. For more information, see [View reports about DLP policy detections](/previous-versions/exchange-server/exchange-150/jj889415(v=exchg.150)).

## Auditing in Yammer Enterprise

Yammer Enterprise provides administrators with the ability to export user activity data from their Yammer network via the [Yammer data export API](https://support.office.com/article/export-data-from-yammer-enterprise-b303d8f3-007d-4ad4-81f8-54fb1ecfb3f2), or manually via the Yammer network admin page. The ability to export logs is restricted to Network Administrators in Yammer. (All Microsoft 365 global administrators are Yammer Network Administrators.)

The following data is exportable:

| Filename | Description |
|----------------------------|-------------------------------------------------------------------------|
| Users.csv | All new, pending, and suspended users in the network |
| Messages.csv | All messages in the network |
| Files.csv (metadata) | Metadata such as filename, file API URL, uploader ID, uploaded at, etc. |
| Files.csv (Original files) | Zip file of the original files uploaded by users into Yammer |
| Topics.csv | Topics created on the network |
| Pages.csv | Pages (notes) created by users in the network |
| Admins.csv | All verified administrators on the network |
| Networks.csv | All Yammer external networks |

Yammer Enterprise data is also available through the Microsoft 365 activity reports. In addition, Yammer is actively working on exposing additional logging via the Microsoft 365 Management Activity API, and on the ability to reason over data using Power BI. See the [Office Roadmap](https://fasttrack.microsoft.com/roadmap?filters=yammer) for more information on these features.
