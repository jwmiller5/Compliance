---
title: "Create a well-designed data classification framework"
description: In this article, you can find an overview of how to create a well-designed data classification framework for Microsoft 365.
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

# Create a well-designed data classification framework

As you develop, revamp, or refine your data classification framework, consider the following leading practices:

- **Do not expect to go from 0-100 on day 1**: Microsoft recommends a crawl-walk-run approach, prioritizing features critical to the organization and mapping them against a timeline. Complete the first step, ensure it was successful, and then move on to the next phase applying lessons learned. Remember that your organization may still be exposed to risk while you design your data classification framework, so it is okay to start small with just a few classification levels and expand later as needed.
- **You are not just writing for cybersecurity professionals**: Data classification frameworks are meant for a broad audience, including your average staff member, your legal and compliance teams, and your IT team. It is important to write clear, easy-to-understand definitions for your data classification levels, providing real-world examples wherever possible. Try to avoid jargon and consider a glossary for acronyms and highly technical terms. For example, use 'Personally Identifiable Information' and provide a definition instead of simply saying 'PII'.
- **Data classification frameworks are meant to be implemented**: For data classification frameworks to be successful, they must be implemented. It is especially relevant when crafting the control requirements for each data classification level. Make sure requirements are clearly defined and that they anticipate and address any ambiguity that might arise during implementation. For example, if you have a control around Personally Identifiable Information, make sure to spell out exactly what that control means, such as Social Security or passport number.
- **Only go granular if you need to**: Data classification frameworks typically contain anywhere from 3-5 data classification levels. But just because you *can* include five levels does not mean you *should*. Consider the following criteria when deciding on the number of classification levels you need:

    - Your industry and your associated regulatory obligations (highly regulated industries tend to need more classification levels)
    - The operational overhead required to maintain a more complex framework
    - Your users and their ability to comply with the increased complexity and nuance associated with more classification levels
    - User experience and accessibility when seeking to apply manual classification across multiple device types

- **Get the right people involved**: Having a senior stakeholder is critical for success, as many projects struggle to start or take longer without senior management backing. Data classification frameworks are typically owned by information technology teams, but they may have legal, compliance, privacy, and change management implications. To ensure you are creating a framework that helps protect your business, be sure to include privacy and legal stakeholders such as your Chief Privacy Officer and the Office of General Counsel in the development of your policy. If your organization has a Compliance division, information governance professionals, or a records management team, they may also have valuable input. As your framework is rolled out to the business, your Communications department also has a key role to play for internal messaging and adoption.
- **Balance security against convenience**: A common mistake is to draft a secure but overly restrictive data classification framework. This framework may have been designed with security in mind but is often difficult to implement in practice. If users need to follow complex, rigid, and time-consuming procedures to apply the framework in their daily lives, there always is a risk that they may no longer believe in its value and will eventually stop following procedures. This risk exists at all levels of the organization, including executive-level (C-suite) managers within the organization. A good balance of security against convenience alongside easy-to-use tools usually lead to wider user adoption and use. If there are gaps in your framework, do not wait until everything is perfect to start implementation. Instead, assess the risk or gap, create a plan to mitigate, and continue moving forward. Remember that information protection is a journey, it is not something that is activated overnight and then done. Plan, implement some capabilities, confirm success, and iterate to the next milestone as tools evolve and users gain maturity and experience.

Also keep in mind that a data classification framework only addresses *what* your organization should do to protect sensitive data. Data classification frameworks are often accompanied by data handling rules or guidelines that define *how* to put these policies in place from a technical and technology perspective. In the following sections, we turn to some practical guidance on how to take your data classification framework from a policy document to a fully implemented and actionable initiative.

## Pain points in creating a data classification framework

Data classification efforts are by nature wide-reaching, touching nearly every business function within an enterprise. Because of this broad scope and the complexity of managing content in modern digital environments, companies often face challenges in knowing where to start, how to manage a successful implementation, and how to measure their progress. Common pain points often include:

- Designing a robust and easy-to-understand data classification framework, including determining classification levels and associated security controls.
- Developing an implementation plan that includes confirming the appropriate technology solution, aligning the plan to existing business processes, and identifying impact to the workforce.
- Setting up a data classification framework within the chosen technology solution and addressing any gaps between the technology capabilities of the tool and the framework itself.
- Establishing a governance structure that oversees the on-going maintenance and health of data classification efforts.
- Identifying specific key performance indicators (KPIs) to monitor and measure progress.
- Increasing awareness and understanding of data classification policies, why they are important, and how to comply with them.
- Complying with internal audit reviews that target data loss and cybersecurity controls.
- Training and engaging users so that they become mindful of the need for correct classification in their daily work and apply the right classification measures.

## Change management and training

Organizations today use tools such as Microsoft 365 to implement their data classification framework. The purpose is to try to automate the classification of data and not increase the burden on your workforce. This structure does not mean that your organization has no responsibility to increase awareness of the need to manage content and protect the organization from the risks discussed in this paper. The leading practice continues to be to conduct awareness training across the organization as part of the annual training schedule. Our experience shows that putting robust and comprehensive effort into training your users, who are the key audience performing this work, increases their 'buy-in' to the effort and can increase adoption and quality. Adding [label recommendations](/microsoft-365/compliance/apply-sensitivity-label-automatically#recommend-that-the-user-apply-a-sensitivity-label) and in-app tips can amplify these efforts. This training does not need to be an extensive standalone course. Your organization may incorporate it into other regular training such as your information security annual training and then include an overview of data classification levels and definitions. The main point is that your workforce has the understanding that even though the tool is automating the classifying of data, that does not eliminate each user's overall responsibility for protecting the data in accordance with your company policy.

In addition, you should consider more in-depth training for IT and information security teams to reinforce operational readiness. The teams that manage the tool and the data classification framework must be on the same page. This coordination may require you to invest in a more robust training schedule that may be more often than annually. Investment in more frequent training represents another avenue to reduce risk to your organization. This team is responsible for the implementation and therefore could be a point of failure if not trained on the tool and the policy.

If you need to manually tag content in the tool, developing a group of super-users that have received more advanced training is appropriate. These super users would be engaged for situations where users are required to manually tag documents with data sensitivity labels and would have deep understanding of your organization's data classification framework and regulatory requirements.

Finally, your leadership should prioritize the championing of information security behaviors to reinforce to the workforce the importance of risk management initiatives. These include developing and implementing a robust data classification framework and assigning key leaders to promote the initiative, sometimes referred to as ambassadors or champions of the change.

## Governance and maintenance

After you have developed and implemented your data classification framework, ongoing governance and maintenance will be critical to your success. In addition to tracking how sensitivity labels are used in practice, you will need to update your control requirements based on changes in regulations, cybersecurity leading practices, and the nature of the content you manage. Governance and maintenance efforts may include:

- Establishing a governance body dedicated to data classification or adding a data classification responsibility to the charter of an existing information security body.
- Defining roles and responsibilities for users overseeing data classification.
- Establishing KPIs to monitor and measure progress.
- Tracking cybersecurity leading practices and regulatory changes.
- Developing standard operating procedures that support and enforce a data classification framework.

## Industry considerations

While the basic principles for developing a strong data classification framework are universal, the details of your framework will depend on the nature of your industry and the unique compliance and security factors your data demands.

For example, financial services firms may need to consider compliance with several regulatory frameworks depending on the scope of their business and the regions in which they operate. Securities firms in the United States must conform to account regulations like [SEC Rule 17a-4(f)](/compliance/regulatory/offering-sec-17a-4) or [FINRA Rule 4511](/microsoft-365/compliance/offering-finra-4511) which address requirements around the security and retention of books and records. Similarly, firms operating in the United Kingdom need to consider [FCA compliance](/microsoft-365/compliance/offering-fca-uk).

Government agencies face various regulations governing their data, which vary based on territory and the nature of their work. In the United States, for instance, government agencies and their agents that access federal tax information (FTI) are subject to [IRS 1075](/microsoft-365/compliance/offering-irs-1075), which aims to minimize the risk of loss, breach, or misuse of federal tax information.

While financial services firms and government agencies are among the most heavily regulated organizations in the world, most businesses have industry-specific considerations that need to be considered. Some examples include:

- Health industry organizations [ensuring compliance with HIPAA](/microsoft-365/compliance/offering-hipaa-hitech).
- Education institutions, from K-12 schools to universities, managing [FERPA compliance](/microsoft-365/compliance/offering-ferpa).
- Drug manufacturers working to comply with [GxP guidelines](/microsoft-365/compliance/offering-gxp) in their country or region around information security.
- Media, retail, and many other companies dealing with [GDPR compliance](/microsoft-365/compliance/gdpr).
- Delivery and storage of entertainment, software, and information content dealing with [CDSA](/microsoft-365/compliance/offering-cdsa).
- Energy industry information security complying with [NERC CIP standard](/microsoft-365/compliance/offering-nerc-cip).

## Implementing your data classification framework in Microsoft 365

Once you have developed your data classification framework, your next step is implementation. The [Microsoft 365 compliance center](https://compliance.microsoft.com/) allows administrators to discover, classify, review, and monitor their data in accordance with their data classification framework. Sensitivity labels can be used to help protect your data by enforcing various protections such as encryption and content marking. They can be applied to data manually; by default, based on policy settings; or automatically, as the result of a condition such as identified PII.

For smaller organizations or organizations with a relatively streamlined data classification framework, creating a single sensitivity label for each of your data classification levels may suffice. The following example shows a one-to-one data classification level to sensitivity label mapping:

|**Classification label**|**Sensitivity label**|**Label settings**|**Published to**|
|:-----------------------|:--------------------|:-----------------|:---------------|
| Unrestricted | Unrestricted | Apply 'Unrestricted' footer | All users |
| General | General | Apply 'General' footer | All users |

>[!TIP]
>During a Microsoft internal information protection pilot, there were difficulties with the understanding and use of the 'Personal' label. Users were confused as to whether this meant PII or merely related to a personal matter. The label was changed to 'non-business' to be clearer. This example shows that taxonomy does not need to be perfect from the start. Start with what you think is right, pilot it, and adjust the label based on feedback if needed

For larger organizations with a global reach or more complex information security needs, you may find this one-to-one relationship between the number of classification levels in your policy and the number of sensitivity labels in your Microsoft 365 environment to be a challenge. This challenge is especially true in global organizations where a given data classification level such as 'Restricted' may have a different definition or different set of controls depending on region.

For more information on implementation, see [Understand data classification](/microsoft-365/compliance/data-classification-overview) and [Learn about sensitivity labels](/microsoft-365/compliance/sensitivity-labels).

## References

- [Microsoft compliance offerings](/microsoft-365/compliance/offering-home)
