---
title: "Microsoft 365 denial-of-service defense strategy"
description: In this article, you can find an overview of Microsoft defense strategy for denial-of-service (DoS) attacks.
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: None
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

# Microsoft 365 denial-of-service defense strategy

## Core principles of defense against denial-of-service attacks

There are three core principles when defending against network-based denial-of-service (DoS) attacks: absorption, detection, and mitigation. Absorption happens before detection, and detection must occur before mitigation can begin. If even a small DoS attack cannot be absorbed, then services will not survive long enough for the attack to be detected. By detecting an attack before the system is overwhelmed, defenders can implement a response plan.

The following formula helps approximate the time to impact of a DoS attack:

  **Maximum Capacity (in bytes/sec) / Growth Rate (in bytes/sec) = Time to Impact (in sec)**

If the time-to-detection is longer than the time-to-impact, the DoS attack will likely be successful. If the time-to-detection is shorter than the time-to-impact, the attacked services should remain online and accessible if mitigation strategies are successful.

Thus, there are two primary strategies for defending against DoS attacks:

- Increase capacity to raise the ceiling of maximum capacity (which in turn provides more time to detect an attack); or
- Decrease the time to detect an attack.

One security benefit of using Microsoft cloud services is how large-scale Microsoft services provide strong network protection to cloud customers in a cost-effective manner. Even on a large scale, there must be a balance between absorption, detection, and mitigation. To find that balance, Microsoft studies attack growth rates to estimate how much Microsoft services need to absorb.

## Denial-of-service defense strategy

Microsoft's strategy to defend against network-based DoS attacks is unique due to our scale and global footprint. This scale allows Microsoft to utilize strategies and techniques that are unavailable to most other organizations. The cornerstone of our DoS strategy is our global presence. Microsoft engages with Internet providers, peering providers (public and private), and private corporations all over the world. This engagement gives Microsoft a significant Internet presence and enables Microsoft to absorb attacks across a large surface area.

As Microsoft's edge capacity has grown over time, the significance of attacks against individual edges has substantially diminished. Because of this decrease, Microsoft has separated the detection and mitigation components of its DoS prevention system. Microsoft deploys multi-tiered detection systems at regional datacenters to detect attacks closer to their saturation points while maintaining global mitigation at the edge nodes. This strategy ensures that Microsoft services can handle multiple simultaneous attacks.

One of the most effective and low-cost defenses employed by Microsoft against DoS attacks is reducing service attack surfaces. Unwanted traffic is dropped at the network edge instead of analyzing, processing, and scrubbing the data inline.

At the interface with the public network, Microsoft uses special-purpose security devices for firewall, network address translation, and IP filtering functions. Microsoft also uses global equal-cost multi-path (ECMP) routing. Global ECMP routing is a network framework to ensure that there are multiple global paths to reach a service. With multiple paths to each service, DoS attacks are limited to the region from which the attack originates. Other regions should be unaffected by the attack, as end users would use other paths to reach the service in those regions. Microsoft has also developed internal DoS correlation and detection systems that use flow data, performance metrics, and other information to rapidly detect DoS attacks.

To further protect our cloud services, Microsoft 365 uses a distributed denial-of-service (DDoS) defense system built into Microsoft Azure's continuous monitoring and penetration-testing processes. The Azure DDoS defense system is designed not only to withstand external attacks, but also attacks from other Azure tenants. Azure uses standard detection and mitigation techniques such as SYN cookies, rate limiting, and connection limits to protect against DDoS attacks. To support our automated protections, a cross-workload DoS incident response team identifies the roles and responsibilities across teams, the criteria for escalations, and the protocols for incident handling across affected teams.

Most DoS attacks launched against targets are at the Network (L3) and Transport (L4) layers of the [Open Systems Interconnection](/windows-hardware/drivers/network/windows-network-architecture-and-the-osi-model) (OSI) model. Attacks directed at the L3 and L4 layers are designed to flood a network interface or service with attack traffic to overwhelm resources and deny the ability to respond to legitimate traffic. To guard against L3 and L4 attacks, Microsoft's DoS solutions use traffic sampling data from datacenter routers to safeguard the infrastructure and customer targets. Traffic sampling data is analyzed by a network monitoring service to detect attacks. When an attack is detected, automated defense mechanisms kick in to mitigate the attack and ensure that attack traffic directed at one customer does not result in collateral damage or diminished network quality of service for other customers.

## Application-level defenses

Microsoft engineering teams follow the rigorous standards set by [Microsoft Operational Security Assurance](https://www.microsoft.com/SDL/OperationalSecurityAssurance) to help protect customer data. Microsoft's cloud services are intentionally built to support high loads, which helps protect against application-level DoS attacks. Microsoft 365's scaled-out architecture distributes services across multiple global datacenters with regional isolation and workload-specific throttling features for relevant workloads.

Each customer's country or region, which the customer's administrator identifies during the initial setup of the services, determines the primary storage location for that customer's data. Customer data is replicated between redundant datacenters according to a primary/backup strategy. A primary datacenter hosts the application software along with all the primary customer data running on the software. A backup datacenter provides automatic failover. If the primary datacenter ceases to function for any reason, requests are redirected to the copy of the software and customer data in the backup datacenter. At any given time, customer data may be processed in either the primary or the backup datacenter. Distributing data across multiple datacenters reduces the affected surface area in case one datacenter is attacked. Furthermore, the services in the affected datacenter can be quickly redirected to the secondary datacenter to maintain availability during an attack and redirected back to the primary datacenter once an attack has been mitigated.

As another mitigation against DoS attacks, individual workloads include built-in features that manage resource utilization. For example, the throttling mechanisms in Exchange Online and SharePoint Online are part of a multi-layered approach to defending against DoS attacks.
