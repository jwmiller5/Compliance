---
title: "Risk management program"
description: "Learn about the risk management program in Microsoft 365"
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
- MS-Compliance
- MS-Compliance-Assurance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
---

# Microsoft 365 Risk Management program

The purpose of the Microsoft 365 Risk Management program is to identify, assess, and manage risks to Microsoft 365. Microsoft's top priority is to proactively identify and address risks that could impact our service infrastructure, as well as our customers, their data, and their trust. In addition, a robust risk management program is necessary to meet contractual obligations and maintain public accreditations that our customers rely on to satisfy their own compliance requirements. While the Microsoft 365 Risk Management program functions independently, it aligns with the overarching Enterprise Risk Management (ERM) program's policies, priorities, and methodologies. Working with the ERM program allows for consistent comparison across business units and engineering groups, contributing to a more cohesive approach to risk management across the enterprise.

The Microsoft 365 Trust team is responsible for managing the Microsoft 365 Risk Management program and conducting the activities defined by the ERM program. The Trust team focuses on integrating the risk management framework with existing Microsoft 365 engineering, service operations, and compliance process to make the Risk Management program more effective and efficient.

The Trust team also maintains the Microsoft 365 Controls Framework, a set of rationalized controls that, when properly implemented with supporting compliance activities, allows engineering teams to comply with key regulations and certifications. This framework is continuously updated based on feedback and findings as part of the risk management process.

Risk management activities fall into four phases: identification, assessment, response, and monitoring and reporting.

![Risk management process activities.](../media/assurance-risk-management-review-process.png)

## Identification

The risk management process starts with identifying all possible risks to all key control areas, internal and external threats, and vulnerabilities in the Microsoft 365 environment. The information guiding this process comes from multiple sources including interviews, vulnerability scans, attack simulation exercises, audit findings, and incident management activities.

The Trust team interviews subject matter experts (SMEs) from multiple service teams on previously identified risks and potential future risks that may be introduced as the services grow. Additionally, SMEs help to validate the accuracy and completeness of risks identified from the other continuous monitoring sources.

The identification phase is also when decision logs, active security and compliance exceptions, and mitigation work from previous risk assessments are reviewed.

## Assessment

Each identified risk is assessed using three metrics: impact, likelihood, and control deficiency.

- Impact refers to the damage that would occur to the service, business, or Microsoft if that risk were to be realized. The impact to Microsoft may include damage to reputation, loss of customers, or legal/compliance implications.
- Likelihood defines the probability of the potential risk being realized and is calculated by analyzing the probability and frequency with which it will occur.
- Control deficiency measures the effectiveness of implemented mitigation controls.

These metrics are used to calculate a risk score that represents the severity of each risk, accounting for existing mitigation strategies. Risks are aggregated and presented to key stakeholders from each service to verify the accuracy and completeness of Microsoft 365's risk posture.

## Response

Using the verified list of risks to Microsoft 365, the Trust team assigns risks to the affected service for risk response. Defined guidelines help determine the appropriate risk response strategy based on the risk score and control effectiveness. Risk response strategies fall into four categories:

- Tolerate: Areas of low-risk exposure with a low level of control.
- Operate: Areas of low-risk exposure where controls are deemed adequate.
- Monitor: Areas of high-risk exposure where controls are deemed adequate and should be monitored for effectiveness.
- Improve: Areas of high-risk exposure with a low level of control that are top priorities in addressing.

The Trust team coordinates with service teams to develop plans for addressing each risk. The severity level determines the appropriate level of review and approval for each plan. For risks that require action, existing engineering bug processes are used for tracking, managing, and making exception decisions. Using a process familiar to the engineering and operation teams makes risk response more efficient and effective.

## Monitoring and reporting

Risks identified as part of the risk assessment are monitored and reported to relevant stakeholders. Monitoring strategies include security monitoring, periodic risk reviews, penetration testing, and vulnerability scanning. These monitoring efforts act as data sources for reporting on key performance indicators, creating dashboards, and developing formal reports, all of which inform future risk decisions.

Multiple times a year, the Trust team meets with risk owners from each service to review risk scores, evaluate the effectiveness of their action plans, and make updates where needed. In addition, Microsoft 365's risk assessment activities contribute to the ERM program's Enterprise Risk Assessments, which provide a high-level overview of Microsoft's risk posture to Microsoft senior management and the ERM program.
