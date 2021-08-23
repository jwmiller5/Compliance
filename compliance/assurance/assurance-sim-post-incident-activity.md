---
title: "Microsoft security incident management: Post-incident activity"
description: "This article, provides an overview of the security incident management post-incident activity process in Microsoft online services."
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
f1.keywords:
- NOCSH
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
titleSuffix: Microsoft Service Assurance
hideEdit: true
---

# Microsoft security incident management: Post-incident activity

## Postmortem

Some security incidents, especially those incidents that are customer impacting or result in a data breach, are subject to a full incident postmortem. The security response team conducts a detailed postmortem with all the parties involved in security incident response to:

- Document the sequence of events that caused the incident.
- Create a technical summary of the incident as supported by the evidence that includes the actors involved in the breach (if known). This summary will include how the response was executed and other key takeaways.
- Identify technical lapses, procedural failures, manual errors, process flaws, and communication glitches, and/or any previously unknown attack vectors that were identified during the security incident response.

The postmortem will directly influence Microsoft online service improvement, operational processes, and documentation by setting new priorities in the Microsoft online services engineering development cycle.

## Documentation

All key technical findings in the postmortem process are captured in a report and service investments or fixes in the form of bugs or development change requests. These findings are followed-up with the appropriate engineering teams. For process failures and cross-organizational issues, issues are documented in the security response team's database and followed-up with the appropriate groups to address them.

## Process improvement

Responding to a security incident in Microsoft online services involves coordination with multiple groups spread across different organizations within Microsoft, and potentially even appropriate external organizations such as law enforcement. We know that it is critical to evaluate our responses after every security incident for both sufficiency and completeness. For any identified improvements or changes, the security response team evaluates the suggestions in consultation with the appropriate teams and stakeholders, and where appropriate incorporates them into standard operating procedures. All required changes, bugs, or service improvements identified during the security incident response or postmortem activity are logged and tracked in an internal Microsoft engineering database. All potential bugs or features are assigned to the appropriate owner. The Microsoft security response team reviews all entries until the issue is resolved.

## Related articles

- [Microsoft security incident management](assurance-security-incident-management.md)
- [Microsoft security incident management: Preparation](assurance-sim-preparation.md)
- [Microsoft security incident management: Detection and analysis](assurance-sim-detection-analysis.md)
- [Microsoft security incident management: Containment, eradication, and recovery](assurance-sim-containment-eradication-recovery.md)
- [How to Log a Security Event Support Ticket](/azure/security/fundamentals/event-support-ticket)
- [Azure and Dynamics 365 breach notification under the GDPR](/compliance/regulatory/gdpr-breach-azure-dynamics)
