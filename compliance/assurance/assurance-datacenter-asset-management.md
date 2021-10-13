---
title: "Datacenter asset management"
description: "An overview of Microsoft datacenter asset management."
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

# Datacenter asset management

Microsoft datacenters are made up of various physical and virtual components, each of which is referred to as an asset. The Microsoft Cloud Operations and Innovation (CO+I) engineering group follows secure standardized processes for the deployment, tracking, and decommissioning of both physical and virtual assets.

## Supply chain integrity

Securing assets begins with securing the supply chain. Microsoft is committed to supply chain integrity and end-to-end supply chain security. Suppliers follow strict chain-of-custody procedures when transporting our cloud components to reduce the risk of alteration and tampering. All inbound and outbound inventory is carefully inspected and monitored to ensure firmware and component integrity.

Information system component deliveries to Microsoft datacenters are typically scheduled. For unscheduled deliveries, Microsoft thoroughly inspects and ensures they are approved for entry to a Microsoft computer room prior to physical entry. When an information system component enters the building, the Asset Management team compares the received item against the referenced ticket and scans the device into the asset management tool. All information system components received or shipped are tracked by the workflow ticketing tool and in the shipping logs in the asset management tool. Visitors are prohibited from using personal laptops and cell phones (except for emergency calling and taking notes), although they are allowed in the production environment (colocations). Plugging cellphones into a device or taking photos are prohibited per datacenter policy. If the equipment entering the datacenter is used for maintenance purposes, the equipment requires Datacenter Management approval in the Datacenter Access Tool system.

## Asset inventory

Microsoft requires all datacenter assets to be accounted for and to have a designated owner. Owners are responsible for maintaining up-to-date asset information for their physical and virtual assets. When new physical assets are added to a datacenter, they are signed for, scanned, uniquely tagged, and checked-in to the inventory control systems. Automated monitoring tools help track both physical and virtual assets.

## Asset maintenance

Microsoft has two teams that provide different types of asset maintenance: the Critical Environment (CE) and Site Services teams. The CE team provides facility management for electrical, mechanical, and physical systems that comprise the operating infrastructure of the facility. They also schedule, perform, document, and review all maintenance activities performed on CE components. Microsoft datacenters rely on a computerized maintenance management system to manage maintenance schedules and work orders. The Site Services team services all the Microsoft online service assets located at the Microsoft datacenters. Additionally, the Site Services team provides on-site technical support and break-fix service for assets belonging to properties provisioning services from the datacenter.

## Asset classification

Microsoft assets - including data - are classified in accordance with Enterprise Data Taxonomy guidelines. These guidelines promote standardization across the enterprise and are reviewed and updated annually. The asset classification and asset protection standards outline the security procedures employees must follow when interacting with each asset. Customers are considered the owner of their data stored in the Microsoft cloud environment. Data assets classified as customer content or customer data are protected by applicable security procedures.

Microsoft considers all documentation to be categorized as a system asset. The Site Services team is responsible for classifying its assets and employing the associated safeguards according to the asset classification and asset protection standards, as well as any additional requirements defined by the service team.

Asset owners are required to assign their assets an asset classification, without exception. In Microsoft datacenter environments, assets refer to servers and network devices. Other digital media like USB flash drives, external hard drives, or CD/DVDs are not used for services operation. Non-digital media is not used in datacenters.

## Media storage

Microsoft digital media assets are physically and securely stored within Microsoft datacenter colocation rooms. Multiple layers of physical access controls and video surveillance are in place to protect and monitor these assets. When digital media assets reach the end of their lifecycle, they are cleared, purged, or destroyed using methods consistent with NIST SP 800-88 prior to disposal. The [data-bearing device destruction](assurance-data-bearing-device-destruction.md) article covers the process of secure disposal of assets.

## Media transport

Microsoft restricts asset transport activities to authorized personnel through chain of custody protections. The use of locks, tamper-proof seals, and required validation of the asset inventory ensures that only authorized personnel are involved in the asset transport.

All media being transported from Microsoft datacenters requires accurate tracking. Microsoft has contracted with several approved vendors to provide secure shipping services. Secure transport begins with an accurate inventory and chain of custody. At the delivery location, the transport company's approved personnel must witness the removal of the tamper-proof seal and unlocking of the container. The receiving personnel inventories the shipment and sends a message confirming the receipt of the assets. Microsoft also contracts with a vendor to provide equipment destruction. Depending on the asset classification, some equipment is required to be destroyed onsite.

The transport of Microsoft digital media outside of the security-controlled space requires the supervision of two Datacenter Operations team members. The assets are continuously accompanied and supervised by authorized personnel until they are destroyed.

The Datacenter Management team controls the delivery and removal of information system components through tickets tracked in the ticketing tool. Delivery and removal of information system components is authorized by system owners.

## Asset retention

Microsoft owned assets are retained as appropriate based on retention requirements set by Corporate Records Management, the asset classification, or contractual requirements. For more information about data retention, see [Data retention, deletion, and destruction in Microsoft 365](assurance-data-retention-deletion-and-destruction-overview.md).
