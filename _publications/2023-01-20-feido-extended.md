---
title: "FeIDo: Recoverable FIDO2 Tokens Using Electronic IDs (Extended Version)"
collection: publications
category: techreports
permalink: /publication/feido-extended
talk: 'n'
excerpt: 'This technical report is an extended version of our [FeIDo research paper](http://fa-schwarz.github.io/publication/2022-11-07-feido). FeIDo addresses the cost and recovery issues of FIDO2 web authentication by combining electronic IDs with a TEE-protected credential service to derive secure attribute-based FIDO2 credentials.'
date: 2023-01-20
venue: 'Publication Database of CISPA Helmholtz Center for Information Security (research paper: ACM CCS 2022)'
paperurl: 'https://fa-schwarz.github.io/files/schwarz-feido-extended-jan2023.pdf'
protourl: 'https://github.com/feido-token'
citation: 'Schwarz, F., Do, K., Heide, G., Hanzlik, L., and Rossow, C., &quot;FeIDo: Recoverable FIDO2 Tokens Using Electronic IDs&quot;. Technical Report. January 2023'
---

This technical report is an extended version of our [FeIDo research paper](http://fa-schwarz.github.io/publication/feido).

Two-factor authentication (2FA) mitigates the security risks of passwords as sole authentication factor. FIDO2---the de facto standard for interoperable web authentication---leverages strong, hardware-backed second factors. However, practical challenges hinder wider FIDO2 user adoption for 2FA tokens, such as the extra costs (20-30 per token) or the risk of inaccessible accounts upon token loss/theft.

To tackle the above challenges, we propose FeIDo, a virtual FIDO2 token that combines the security and interoperability of FIDO2 2FA authentication with the prevalence of existing eIDs (e.g., electronic passports). Our core idea is to derive FIDO2 credentials based on personally-identifying and verifiable attributes---name, date of birth, and place of birth---that we obtain from the user's eID. As these attributes do not change even for refreshed eID documents, the credentials "survive" token loss. Even though FeIDo operates on privacy-critical data, all personal data and resulting FIDO2 credentials stay unlinkable, are never leaked to third parties, and are securely managed in attestable hardware containers (e.g., SGX enclaves). In contrast to existing FIDO2 tokens, FeIDo can also derive and share verifiable meta attributes (anonymous credentials) with web services. These enable verified but pseudonymous user checks, e.g., for age verification (e.g., "is adult").