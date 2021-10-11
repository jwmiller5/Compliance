---
title: "Datacenter physical access security"
description: "Learn more about Microsoft datacenter physical access security."
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

# Datacenter physical access security

Microsoft understands the importance of protecting customer data and is committed to securing the datacenters that contain it. Microsoft datacenters are designed, built, and operated to strictly limit physical access to the areas where customer data is stored.

Physical security at datacenters is in alignment with the defense-in-depth principle. Multiple security measures are implemented to reduce the risk of unauthorized users accessing data and other datacenter resources.

- **Perimeter security**: Microsoft datacenters are nondescript buildings with perimeter fencing and 24-hour exterior lighting. Tall fences made of steel and concrete encompass every inch of the perimeter and all entry to the datacenter campus must go through a well-defined access point. Camera-monitored entrance gates and security guard patrols ensure entry and exit are restricted to designated areas. Bollards and other measures protect the datacenter exterior from potential threats, including unauthorized access.
- **Entering the datacenter**: The datacenter entrance is staffed with professional security officers who have undergone rigorous training and background checks. Security officers routinely patrol the datacenter and video feeds from cameras inside the datacenter are always monitored.
- **Inside the datacenter**: Upon entering the building, two-factor authentication with biometrics is required to continue moving through the datacenter. Once authenticated, access is granted to the authorized portion of the datacenter and only for the time approved. Within the datacenter, areas designated as highly sensitive require additional two-factor authentication.
- **Datacenter floor**: The datacenter floor can only be accessed with prior approval and after a full body metal detection screening at the time of entry. To reduce the risk of unauthorized data entering or leaving the datacenter, only approved devices can make their way onto the datacenter floor. Additionally, video cameras monitor the front and back of every server rack. When exiting the datacenter floor, all individuals are subject to an additional full body metal detection screening.
- **Leaving the datacenter**: To leave the datacenter facility, each person must go through a final security checkpoint and all visitors must surrender their temporary badges. After collection, all visitor badges have their access levels removed before they are reused for future visits.

## Access provisioning

The Datacenter Management (DCM) team has implemented operational procedures to restrict physical access to only authorized employees, contractors, and visitors. Temporary or permanent access requests are tracked using a ticketing system. Badges are either issued or activated for personnel requiring access after verification of identification. Physical keys and temporary access badges are secured within the security operations center (SOC).

Microsoft datacenters are subject to a least privileged access policy, meaning datacenter access is restricted to personnel with an approved business need, with no more access than necessary. Access requests are time-limited and are only renewed if the requestor's business need remains valid.

Datacenter access records are maintained in the form of approved requests. Requests can only be approved by the DCM team, and visitor access requests to datacenters are recorded and made available for any future investigations

## Datacenter security personnel

Security personnel throughout the datacenter facilities and campus are responsible for the following activities:

- Operate workstations located at the Security Operations Center within the primary administration building.
- Conduct periodic inspections through facility walkthroughs and patrols of the grounds.
- Respond to fire alarms and safety issues
- Dispatch security personnel to assist service requests and emergencies
- Provide Datacenter Management team with periodic updates about security events and entry logs
- Operate and monitor alarm, access control, and surveillance systems

## Visitor access

Security verification and check-in is required for personnel requiring temporary access to the interior of the datacenter facility, including tour groups and other visitors. Datacenter visitors must sign a non-disclosure agreement, undergo datacenter management review, and obtain approval by datacenter management before their scheduled visit. Upon initial arrival, datacenter visitors are processed with temporary, least privileged access credentials. Additionally, a Microsoft full-time employee (FTE) or authorized designee approved by datacenter management is assigned to escort visitors during the visit.

All visitors that have approved access to the datacenter are designated as *Escort Only* on their badges and are required to always remain with their escorts. Escorted visitors do not have any access levels granted to them and can only travel on the access of their escorts. The escort is responsible for reviewing the actions and access of their visitor during their visit to the datacenter.

Visitor access is monitored by the assigned escort and by the Control Room Supervisor via closed circuit television (CCTV) and the alarm monitoring system. Visitors with an approved access request have their access request reviewed at the time their identification is verified against a form of government-issued identification or Microsoft-issued badge. Visitors approved for escorted access are issued a self-expiring sticky badge, and upon return the access record within the tool is terminated. If a visitor leaves with their badge, the badge automatically expires within 24 hours.

Temporary access badges are stored within the access-controlled SOC and inventoried at the beginning and end of each shift. Security officers are staffed 24x7, and physical keys are stored in an electronic key management system that is linked to the physical access system requiring a security officer's PIN and access badge to gain access.

## Access review and deprovisioning

The DCM team is responsible for reviewing datacenter access regularly and for conducting a quarterly audit to verify individual access is still required.

For terminations or transfers, the person's access is immediately removed from the system and their access badge is removed. This removes any datacenter access the person may have had. DCM teams also perform quarterly access reviews to validate the appropriateness of the datacenter access list in the system.

## Key management

Physical/hard keys are checked out to specific personnel by matching the person's access badge to the physical key. A person must have the appropriate access level in the tool to check out specific keys. Keys are not allowed offsite.

The hard keys and badges are kept under strict control by Microsoft and are audited daily. Microsoft also mitigates risks by implementing strict assignment of access levels, and controlled distribution and management of keys. The primary access methods at datacenters are electronic access badges and biometrics, which allows for immediate revocation of access as required. Microsoft has procedures in place to determine appropriate action commensurate with the risk for all lost keys. These actions could require the rekeying of a single-server rack or door and up to the rekeying of the entire datacenter facility.

## Access logging and monitoring

Access requests and entrance/exit events are logged and retained as part of an electronic audit trail, allowing after the fact data interrogation and reconciliation. Access control system reports and data analysis allow further anomaly detection to identify and prevent unnecessary and unauthorized access.

Datacenter surveillance systems monitor critical datacenter areas like datacenter main entry/exit, datacenter colocations entry/exit, cages, locked cabinets, aisle ways, shipping and receiving areas, critical environments, perimeter doors, and parking areas. Surveillance recordings are retained for a minimum of 90 days unless local law dictates otherwise.

A Control Room Supervisor is always in the SOC to provide monitoring of physical access in the datacenter. Video surveillance is employed to monitor physical access to the datacenter and information system. The video surveillance system is linked to the building alarm monitoring system to support physical access monitoring of alarm points. Security officers ensure that only those personnel with proper authorization are allowed access and verify that anyone bringing equipment in and out of critical infrastructure facilities follows proper procedures.

Security events that occur within the datacenter are documented by the security team in a report called a Security Event Notification (SEN). SEN reports capture the details of a security event and are required to be documented after an event occurs to capture details as accurately as possible. SEN reports also contain the investigative analysis conducted in an After Action Report (AAR), which documents the investigation of a security event, attempts to identify the root cause of the event, and records any remediation actions and lessons learned. Remediation actions and lessons learned are utilized to improve security procedures and reduce the likeliness of the event repeating. If an incident impacts Microsoft assets or services, the Security Incident Management (SIM) team has detailed procedures in place to respond.

In addition to the 24x7 onsite security, Microsoft datacenters utilize alarm monitoring systems that provide real-time alarm and video monitoring. Datacenter doors have alarms that report on each opening and when they remain open past a programmed length of time. The security system is programmed to display live video image when a door alarm is triggered. Access card and biometric readers are programmed and monitored through the alarm monitoring system. Alarms are monitored and responded to 24x7 by the Control Room Supervisor who utilizes cameras in the area of the incident being investigated to give the responder real-time information.
