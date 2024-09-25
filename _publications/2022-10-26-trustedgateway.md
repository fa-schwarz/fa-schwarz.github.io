---
title: "TrustedGateway: TEE-Assisted Routing and Firewall Enforcement using ARM TrustZone"
collection: publications
category: conferences
permalink: /publication/trugw
talk: 'y'
excerpt: 'This paper presents a new design for standalone gateway routers that protects their network traffic and policy enforcement against system-level attackers using the Arm TrustZone system-level TEE.'
date: 2022-10-16
accept-rate: '25.2%'
venue: '25th International Symposium on Research in Attacks, Intrusions and Defenses'
#slidesurl: 'https://academicpages.github.io/files/slides2.pdf'
paperurl: 'https://fa-schwarz.github.io/files/schwarz-trustedgateway-raid2022.pdf'
protourl: 'https://github.com/trugw'
citation: 'Schwarz, F., &quot;TrustedGateway: TEE-Assisted Routing and Firewall Enforcement using ARM TrustZone&quot;. In: <i>Proceedings of the 25th International Symposium on Research in Attacks, Intrusions and Defenses</i>. ACM, October 2022.'
---

Gateway routers are at the heart of every network infrastructure, interconnecting subnetworks and enforcing access control policies using firewalls. However, their central position makes them high-value targets for network compromises. Typically, gateways are erroneously assumed to be hardened against software vulnerabilities (“bastion host”). In fact, though, they inherit the attack surface of their underlying commodity OSes which together with the wealth of auxiliary services available on both consumer and enterprise gateways—web and VoIP, file sharing, remote logins, monitoring, etc.—undermines this belief. This is underlined by a plethora of recent CVEs for commodity OSes and services of popular routers which resulted in authentication bypass or remote code execution thus enabling attackers full control over their security policies.

We present TrustedGateway (TruGW), a new gateway architecture, which isolates “core” networking features—routing and firewall—from error-prone auxiliary services and gateway OSes. TruGW leverages a TEE-assisted design to protect the network path and policies while staying compatible with commodity gateway platforms. TruGW uses ARM TrustZone to protect the NIC and traffic processing from a fully-compromised gateway and permits policy updates only by trusted remote administrators. That way, TruGW can readily guarantee the secure enforcement of trusted policies on commodity gateways. TruGW’s small attack surface is a key enabler to regain trust in core network infrastructures.