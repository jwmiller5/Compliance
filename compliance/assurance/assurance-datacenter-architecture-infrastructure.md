---
title: "Datacenter architecture and infrastructure"
description: "An overview of Microsoft datacenter architecture and infrastructure."
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
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
f1.keywords:
- NOCSH
titleSuffix: Microsoft Service Assurance
hideEdit: true
---

# Datacenter architecture and infrastructure

Microsoft datacenters are designed to implement a strategy of defense-in-depth, employing multiple layers of safeguards to reliably protect our cloud architecture, and supporting infrastructure. Redundancy is built into all systems at multiple levels to support datacenter availability.

Microsoft has highly secured datacenter facilities spread worldwide creating a distributed datacenter infrastructure, supporting thousands of online services. This globally distributed infrastructure is designed to bring applications closer to users, preserve data residency, and offer comprehensive compliance and resiliency options for customers.

Regions are sets of datacenters that are interconnected via a massive and resilient network. Regions are organized into geographies, granting customers with specific data-residency and compliance needs the ability to keep their data and applications close. Built-in fault tolerance allows geographies to withstand complete region failure through their connection to the dedicated, high-capacity networking infrastructure.

Physically separate locations within a region are referred to as availability zones, each being made up of one or more datacenters equipped with independent power, cooling, and networking. Availability zones allow for mission-critical applications to run with high availability and low-latency replication.

Geographically distributed datacenters enable Microsoft to bring services closer to customers, reduce network latency, and allow for geo-redundant backup and failover.

## Availability

Microsoft datacenters are engineered to provide 99.999% availability to meet customer SLAs and service needs. Microsoft invests significantly in the global operations, management, networks, and sustainability of facilities that deliver services 24x7x365.

## Compliance Standards and Requirements

Microsoft has invested over $15 billion building our global infrastructure and over $9 billion in research and development to increase efficiency and drive innovation. As a result, Microsoft's datacenters are evolving at a more rapid pace than many facilities in the industry, and thus do not follow prescriptive requirements outlined by traditional datacenter standards. In addition to the wealth of operational insight that comes with running one of the world's largest datacenter portfolios, Microsoft uses IEEE Gold Book data and third-party reliability simulation software to continuously improve our datacenter design standards. Microsoft datacenters are audited extensively as part of several regulatory audits as called out in the compliance portfolio. The level of maturity in Microsoft datacenters can be evaluated through the compliance portfolio and, for resiliency specifically, the ISO 22301 certification.

While Microsoft operates programs in alignment with the spirit of the ANSI/TIA-942 Telecommunications Infrastructure of Datacenters Standard, portions of this standard are not applicable to Microsoft or conflict with other regulatory and/or country-specific requirements. Moreover, Microsoft has chosen to use a more performance-based approach to match customer needs.

## Data and network redundancy

Critical datacenter facilities employ multiple layers of redundant systems to sustain faults and minimize service disruptions. Locally redundant storage at the disk level protects data within a region, with geo-redundant storage providing intra-region redundancy. To ensure reliable network communications, Microsoft owns and utilizes diverse fiber routes and redundant hardware to protect critical components from failure or service disruption.

Geo-replication is used to provide redundancy to alternate geographic locations. Data durability is obtained by synchronously replicating data across multiple databases in different datacenters. Restoration tests are performed for all backup data owned by the cloud. Disaster Recovery is achieved by asynchronous replication to a datacenter in a different geographical region.

## Capacity

Cloud Operations is a dedicated capacity team that forecasts future requirements to ensure necessary capacity is structured and available for customer and internal use. Systems are monitored to ensure acceptable service performance, availability, service utilization, storage utilization, network latency, and audit log capacity. Microsoft also protects datacenters against the effects of denial-of-service attacks on bandwidth, transactional capacity, and storage capacity.

All service teams include capacity planning as a key feature of their datacenter models and data replication plans to ensure that there is necessary capacity for information processing, telecommunications, and environmental support.

## Power

Microsoft's datacenters have dedicated 24x7 uninterruptible power supplies (UPSs) and emergency power support, which includes on-site generators that provide backup power. Regular maintenance and testing are conducted for both the UPS and generators, and operations teams have contractual agreements with local vendors for emergency fuel delivery. Datacenters also have a dedicated Facility Operations Center to monitor power systems, including critical electrical components.

Microsoft datacenters are equipped with protective spaces and appropriate labeling for cables. The power infrastructure equipment is placed in environments that have been engineered to protect from environmental risks. All portable online services' assets must be locked or fastened in place in order to provide protection against theft or movement damage. Power cables are run under the floors, overhead in cable trays, and within cabinets for protection from moving parts and accidental damage. All electrical spaces are behind card readers or additional key locks as appropriate. Access hallways, exterior entrances, and equipment yards are all monitored via video surveillance. Power systems also utilize redundancy as a form of protection, with multiple power/utility feeds into the facility and generators and UPS systems.

A long-term alternate power supply is implemented for the information system that is capable of maintaining power in a minimally required operational capability. When power fails or drops to an unacceptable voltage level, UPS systems instantly come online. This provides enough power for running the servers until the generators can take over. Emergency generators provide back-up power for extended outages, planned maintenance and can operate the datacenter with on-site fuel reserves if a natural disaster occurs.

Microsoft datacenters (both leased and fully managed) implement emergency lighting in the form of overhead emergency lighting on dedicated circuits backed up by UPS and generator systems. Automatic emergency lighting is implemented in accordance with the National Fire and Protection Association (NFPA) Life Safety Code or the applicable local code/law. If utility power is lost, the emergency lighting will automatically switch to power provided by the UPS and generator systems. The emergency lighting systems within the datacenters undergo routine maintenance to ensure that they remain in proper working order.

## Maintenance

System maintenance policy and procedures are in place in accordance with *Microsoft's Online Services Physical and Environmental Security Standard*. All Microsoft equipment and systems are regularly maintained in order to guarantee operational efficiency. Maintenance of any equipment or system must be performed in accordance with manufacturer's recommendations, carried out by authorized personnel, and recorded in a maintenance ticket.

There are two asset teams that maintain different types of systems:

- **Critical Environment (CE)** team:

    - CE is the team that provides facility management for electrical, mechanical, and physical systems that comprise the operating infrastructure of the facility. The CE team schedules, performs, documents, and reviews all maintenance activities performed on CE components. Microsoft datacenters rely on a computerized system to manage maintenance schedules and work orders.
    - Datacenter management (DCM) is responsible for all CE maintenance that is performed either on site or remotely. CE maintenance is prescribed in required step-by-step documents called Methods of Procedure (MOP). MOPs are reviewed/approved by datacenter management prior to any work beginning.

- **Site Services** team:

    - Site Services is the team that provides the servicing of Microsoft online service assets located at the Microsoft datacenter. The DC Site Services team provides a smart hands/break fix service for assets belonging to properties provisioning services from the datacenter. For example, assets requiring physical maintenance could request smart hands service from the DC Site Services team. All Site Services work on Microsoft assets is scheduled, performed, documented, and reviewed in work tickets within the workflow ticketing tool, and no work can occur without an approved work ticket.
    - The Technical Program Manager (TPM) and DCM team are responsible for all Site Services work that occurs in the datacenter and work that requires the asset to be transferred offsite. Site Services maintenance is performed in areas of the datacenter that are controlled and protected by physical security mechanisms.

If CE components are required to be removed from the facility, handling the equipment is approved by DCM. In most instances, CE components receive onsite maintenance and are not removed from the facility. Property assets (for example, network devices or servers) requiring transfer offsite must have explicit asset owner approval.

Digital media within the cloud may not be transported from the colocation space unless it is moved to be destroyed. When these assets are to be destroyed, they are stored in locked storage bins that are under CCTV camera coverage. When the assets are ready to be destroyed, a physical security officer and a Microsoft full-time employee from Asset Management must escort the locked bin from the colocation space to where the onsite shredding is to occur. As shredding occurs at the datacenter and under Microsoft supervision, Microsoft assets do not leave the controlled areas of the datacenter.

All maintenance work must be approved prior to work beginning, including access to system maintenance tools. Microsoft Infrastructure has implemented the maintenance tools control by creating an access level within the Datacenter Access Tool (DCAT). Each facility contains a restricted physical lock box or access-controlled room for the storage of specialized maintenance tools. Access to the lock box or storage room is controlled in the DCAT tool to prohibit unauthorized access to the maintenance tools. This program ensures that only personnel with approved access can access the tools. The Site Services team performs routine inventory checks to verify the status of all tools. On a quarterly basis, the datacenter management team and physical security teams perform audits of the DCAT access list to keep the access list of maintenance personnel current. Personnel terminations or transfers are reflected immediately through a manual update of the access list. Access to the lock box or maintenance storage room is tracked in the access badge reader logs, which are available for any investigations.

The Site Services team maintains an inventory of approved maintenance tools for use within the datacenter. Maintenance personnel are directed to use the provided maintenance tools. Datacenter Management (DCM) approval is required in order to use tools not provided by the datacenter. Physical hand tools are exempt from this type of control.

Microsoft datacenters maintain resident maintenance personnel to support critical datacenter infrastructure systems (the Critical Environment team) and datacenter operations (the Site Services team). The Critical Environment and Site Services teams have identified critical security and technology system components that they maintain spares for onsite. Critical information system services are provisioned from more than one datacenter to prevent an interruption in service due to an incident at one of the datacenters.
