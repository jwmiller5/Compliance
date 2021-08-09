---
title: "Data classification & sensitivity label taxonomy"
description: In this article, you can find an overview of using data classification & sensitivity label taxonomy with Microsoft 365.
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: Normal
search.appverid:
- MET150
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
---

# Data classification & sensitivity label taxonomy

Sensitive data presents significant risk to a company if it is stolen, inadvertently shared, or exposed through a breach. Risk factors include reputational damage, financial impact, and loss of competitive advantage. Protecting the data and information your business manages is a top priority for your organization, but you may find it difficult to know if your efforts are truly effective, given the amount of content held by your enterprise.

In addition to volume, your content may range in importance from highly sensitive and impactful to trivial and transient. It can also be under the purview of various regulatory compliance requirements. Knowing what to prioritize and where to apply controls can be a challenge. Read on to learn about *data classification*, an important tool for protecting your content from theft, sabotage, or inadvertent destruction, and how Microsoft 365 can help you meet your information security goals.

## What is data classification?

[Data classification](/microsoft-365/compliance/data-classification-overview) is a specialized term used in the fields of cybersecurity and information governance to describe the process of identifying, categorizing, and protecting content according to its sensitivity or impact level. In its most basic form, data classification is a means of protecting your data from unauthorized disclosure, alteration, or destruction based on how sensitive or impactful it is.

## What is a data classification framework?

Often codified in a formal, enterprise-wide policy, a data classification framework (sometimes called a 'data classification policy') is typically comprised of 3-5 classification levels. These usually include three elements: a name, description, and real-world examples. Microsoft recommends no more than five top-level parent labels, each with five sub-labels (25 total) to keep the user interface (UI) manageable. Levels are typically arranged from least to most sensitive such as *Public*, *Internal*, *Confidential*, and *Highly*
*Confidential*. Other level name variations you may encounter include *Restricted*, *Unrestricted*, and *Consumer Protected*. Microsoft recommends label names that are self-descriptive and that highlight their relative sensitivity clearly. For example, *Confidential* and *Restricted* may leave users guessing which label is appropriate, while *Confidential* and *Highly Confidential* are clearer on which is more sensitive. 

The following table shows an example of a *Highly Confidential* data classification framework level:

|**Classification level**|**Description**|**Examples**|
|:-----------------------|:--------------|:-----------|
| Highly Confidential | Highly Confidential data is the most sensitive type of data stored or managed by the enterprise and may require legal notifications if breached or otherwise disclosed. <br><br> Restricted Data requires the highest level of control and security, and access should be limited to "need-to- know." | Sensitive Personally Identifiable Information (Sensitive PII) <br> Cardholder Data <br> Protected Health Information (PHI) <br> Bank Account Data |

>[!TIP]
>Microsoft's corporate data classification framework originally used a category and label named 'Internal' during pilot phase but found that there were legitimate reasons for a document to be shared externally and shifted to using 'General'.

Another important component of a data classification framework is the controls associated with each level. Data classification levels by themselves are simply labels (or tags) that indicate the value or sensitivity of the content. To *protect* that content, data classification frameworks define the controls that should be in place for each of your data classification levels. These controls may include requirements related to:

- Storage type and location
- Encryption
- Access control
- Data destruction
- Data loss prevention
- Public disclosure
- Logging and tracking access
- Other control objectives, as needed

Your security controls will vary by data classification level, such that the protective measures defined in your framework increase commensurate with the sensitivity of your content. For example, your data storage control requirements will vary depending upon the media that is being used as well as upon the classification level applied to a given piece of content. The following table shows an example of data classification controls for a specific storage type:

|**Storage type**|**Confidential**|**Internal**|**Unrestricted**|
|:---------------|:---------------|:-----------|:---------------|
| Removable Storage | Prohibited | Prohibited unless encrypted | No control required |

Correctly applying the right level of data classification can be complex in real-life situations and may sometimes overwhelm end users. Once a policy or standard has been created that defines the required levels of data classification, it is important to guide end users on how to bring this framework to life in their daily work. This area is where data classification handling rules or guidelines come in.

Data classification handling guidelines will help end users with specific guidance on how to handle each level of data appropriately, for different storage media throughout their lifecycle. These guidelines help end users to correctly apply rules in practice, for instance when sharing documents, sending emails, or collaborating across different platforms and organizations.

Microsoft customers indicate that approximately 50% of an Information Protection project is business focused rather than technical, so end-user training and communication is critical to success.
