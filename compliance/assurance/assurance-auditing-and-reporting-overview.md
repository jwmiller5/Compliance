---
title: "Auditing and reporting in Microsoft cloud services"
description: "An overview of auditing and reporting features within Office 365, Microsoft 365, and Service Assurance."
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: overview
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

# Auditing and reporting in Microsoft cloud services

Microsoft cloud services include several auditing and reporting features you can use to track user and administrative activity within their tenant, Examples include changes made to Exchange Online and SharePoint Online tenant configuration settings, and changes made by users to documents and other items. You can use audit information and reports available in Microsoft cloud services to more effectively manage user experience, mitigate risks, and fulfill compliance obligations.

## Security & Compliance Centers

The [Microsoft 365 Security & Compliance Center](https://protection.office.com), [Microsoft 365 Defender portal](https://security.microsoft.com), and [Microsoft Purview compliance portal](https://compliance.microsoft.com) are one-stop portals for protecting data in your organization, and they include many auditing and reporting features. These centers help you with your data protection or compliance needs and audit user and administrator activity. You can access these centers using your subscription admin account.

These centers include navigation panes for access to several features:

- **Alerts:** Enables you to manage alerts, view security-related alerts, and manage advanced alerts using [Defender for Cloud Apps](/cloud-app-security/what-is-cloud-app-security).
- **Permissions:** Enables you to [assign permissions](/microsoft-365/security/office-365-security/grant-access-to-the-security-and-compliance-center) such as Compliance Administrator, eDiscovery Manager, and others to people in your organization so they can perform tasks in these centers. You assign permissions for most features in each center, but other permissions must be configured using the Exchange admin center and SharePoint admin center.
- **Threat management:** Enables you to create and apply device management policies using [Basic Mobility and Security for Microsoft 365](https://support.microsoft.com/office/overview-of-basic-mobility-and-security-for-microsoft-365-faa7d8e5-645d-4d59-839c-c8d4c1869e4a), to set up [data loss prevention](/microsoft-365/compliance/data-loss-prevention-policies) (DLP) policies for your organization, to configure email filtering, anti-malware, DomainKeys Identified Mail (DKIM), safe attachments, safe links, and OAuth apps.
- **Data governance:** Enables you to [import email or SharePoint data from other systems into Microsoft 365](https://support.office.com/article/Import-PST-files-or-SharePoint-data-to-Office-365-ba688e0a-0fcb-4bd7-8e57-2b669564ea84), [configure archive mailboxes](https://support.office.com/article/Enable-archive-mailboxes-in-the-Office-365-Security-Compliance-Center-268a109e-7843-405b-bb3d-b9393b2342ce), and set [retention policies](/microsoft-365/compliance/retention-policies) for email and other content within your organization.
- **Search & investigation:** Provides [content search](https://support.office.com/article/Run-a-Content-Search-in-the-Office-365-Security-Compliance-Center-61852fd9-fe8a-4880-a339-cb19ed3bff4a), [audit log](https://support.office.com/article/Search-the-audit-log-in-the-Office-365-Security-Compliance-Center-0d4d0f35-390b-4518-800e-0c7ec95e946c), quarantine, and [eDiscovery case management](https://support.office.com/article/Manage-eDiscovery-cases-in-the-Office-365-Security-Compliance-Center-edea80d6-20a7-40fb-b8c4-5e8c8395f6da) tools to quickly drill into activity across Exchange Online mailboxes, groups and public folders, SharePoint Online, and OneDrive for Business.
- **Reports:** Enables you to quickly access [reports](https://support.office.com/article/Reports-in-the-Office-365-Security-Compliance-Center-7acd33ce-1ec8-49fb-b625-43bac7b58c5a) for SharePoint Online, OneDrive for Business, Exchange Online, and Azure AD.
- **Service assurance:** Provides information about how Microsoft maintains security, privacy, and compliance with global standards for Microsoft 365, Azure, Microsoft Dynamics CRM Online, Microsoft Intune, and other cloud services. Also includes access to third-party ISO, SOC, and other audit reports, as well as Audited Controls, which provides details about the various controls that have been tested and verified by third-party auditors of Microsoft 365.

## Service assurance

Many organizations in regulated industries are subject to extensive compliance requirements. To perform their own risk assessments, customers often need in-depth information about how Microsoft 365 maintains the security and privacy of their data. Microsoft is committed to the security and privacy of customer data in its cloud services and to earning customer trust by providing a transparent view of its operations, and easy access to independent compliance reports and assessments.

Service Assurance provides transparency of operations and information about how Microsoft maintains the security, privacy, and compliance of customer data in Microsoft 365. It includes third-party audit reports along with a library of white papers, FAQs, and other materials on Microsoft 365 topics such as data encryption, data resiliency, security incident management and more. Customers can use this information to perform their own regulatory risk assessments. Compliance officers can assign the "Service Assurance User" role to give users access to Service Assurance. The tenant administrator can also provide external users, such as independent auditors, with access to information in the Service Assurance dashboard through the [Microsoft Cloud Service Trust Portal](https://aka.ms/STP) (STP).

## Resources

- [Microsoft 365 Reporting Features](assurance-reporting-features.md)
- [Internal Logging for Microsoft 365 Engineering](assurance-internal-logging.md)
