---
title: "Microsoft denial-of-service defense strategy"
description: In this article, you can find an overview of the Microsoft defense strategy for denial-of-service (DoS) attacks.
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

# Microsoft denial-of-service defense strategy

## Denial-of-service defense strategy

Microsoft's strategy to defend against network-based distributed denial-of-service (DDoS) attacks is unique due to a large global footprint, allowing Microsoft to utilize strategies and techniques that are unavailable to most other organizations. Additionally, Microsoft contributes to and draws from collective knowledge aggregated by an extensive threat intelligence network, which includes Microsoft partners and the broader internet security community. This intelligence, along with information gathered from online services and Microsoft's global customer base, continuously improves Microsoft's DDoS defense system that protects all of Microsoft online services' assets.

The cornerstone of Microsoft's DDoS strategy is global presence. Microsoft engages with Internet providers, peering providers (public and private), and private corporations all over the world. This engagement gives Microsoft a significant Internet presence and enables Microsoft to absorb attacks across a large surface area

As Microsoft's edge capacity has grown over time, the significance of attacks against individual edges has substantially diminished. Because of this decrease, Microsoft has separated the detection and mitigation components of its DDoS prevention system. Microsoft deploys multi-tiered detection systems at regional datacenters to detect attacks closer to their saturation points while maintaining global mitigation at the edge nodes. This strategy ensures that Microsoft services can handle multiple simultaneous attacks.

One of the most effective and low-cost defenses employed by Microsoft against DDoS attacks is reducing service attack surfaces. Unwanted traffic is dropped at the network edge instead of analyzing, processing, and scrubbing the data inline.

At the interface with the public network, Microsoft uses special-purpose security devices for firewall, network address translation, and IP filtering functions. Microsoft also uses global equal-cost multi-path (ECMP) routing. Global ECMP routing is a network framework to ensure that there are multiple global paths to reach a service. With multiple paths to each service, DDoS attacks are limited to the region from which the attack originates. Other regions should be unaffected by the attack, as end users would use other paths to reach the service in those regions. Microsoft has also developed internal DDoS correlation and detection systems that use flow data, performance metrics, and other information to rapidly detect DDoS attacks.

To further protect cloud services, Microsoft uses Azure DDoS Protection, a DDoS defense system built into Microsoft Azure's continuous monitoring and penetration-testing processes. Azure DDoS Protection is designed not only to withstand external attacks, but also attacks from other Azure tenants. Azure uses standard detection and mitigation techniques such as SYN cookies, rate limiting, and connection limits to protect against DDoS attacks. To support automated protections, a cross-workload DDoS incident response team identifies the roles and responsibilities across teams, the criteria for escalations, and the protocols for incident handling across affected teams.

Most DDoS attacks launched against targets are at the Network (L3) and Transport (L4) layers of the [Open Systems Interconnection](/windows-hardware/drivers/network/windows-network-architecture-and-the-osi-model) (OSI) model. Attacks directed at the L3 and L4 layers are designed to flood a network interface or service with attack traffic to overwhelm resources and deny the ability to respond to legitimate traffic. To guard against L3 and L4 attacks, Microsoft's DDoS solutions use traffic sampling data from datacenter routers to safeguard the infrastructure and customer targets. Traffic sampling data is analyzed by a network monitoring service to detect attacks. When an attack is detected, automated defense mechanisms kick in to mitigate the attack and ensure that attack traffic directed at one customer does not result in collateral damage or diminished network quality of service for other customers.

Microsoft also takes an offensive approach to DDoS defense. Botnets are a common source of command and control for conducting DDoS attacks to amplify attacks and maintain anonymity. The Microsoft Digital Crimes Unit (DCU) focuses on identifying, investigating, and disrupting malware distribution and communications infrastructure to reduce the scale and impact of botnets.

## Application-level defenses

Microsoft's cloud services are intentionally built to support high loads, which help to protect against application-level DDoS attacks. Microsoft's scaled-out architecture distributes services across multiple global datacenters with regional isolation and workload-specific throttling features for relevant workloads.

Each customer's country or region, which the customer's administrator identifies during the initial configuration of the services, determines the primary storage location for that customer's data. Customer data is replicated between redundant datacenters according to a primary/backup strategy. A primary datacenter hosts the application software along with all the primary customer data running on the software. A backup datacenter provides automatic failover. If the primary datacenter ceases to function for any reason, requests are redirected to the copy of the software and customer data in the backup datacenter. At any given time, customer data may be processed in either the primary or the backup datacenter. Distributing data across multiple datacenters reduces the affected surface area in case one datacenter is attacked. Furthermore, the services in the affected datacenter can be quickly redirected to the secondary datacenter to maintain availability during an attack and redirected back to the primary datacenter once an attack has been mitigated.

As another mitigation against DDoS attacks, individual workloads include built-in features that manage resource utilization. For example, the throttling mechanisms in Exchange Online and SharePoint Online are part of a multi-layered approach to defending against DDoS attacks.

Azure SQL Database has an extra layer of security in the form of a gateway service called DoSGuard that tracks failed login attempts based on IP address. If the threshold for failed login attempts from the same IP is reached, DoSGuard blocks the address for a pre-determined amount of time.

## Resources

- [Azure DDoS Protection Standard overview](/azure/ddos-protection/ddos-protection-overview)
- [Azure DDoS Protection Standard fundamental best practices](/azure/ddos-protection/fundamental-best-practices)
- [Components of a DDoS response strategy](/azure/ddos-protection/ddos-response-strategy)
