---
title: "KeyVisor -- A Lightweight ISA Extension for Protected Key Handles with CPU-enforced Usage Policies"
collection: publications
category: unpublished
permalink: /publication/keyvisor
# talk: 'n'
excerpt: 'This paper presents a lightweight security extension for RISC-V CPUs that protects AES keys against local attackers and enforces secure key usage policies. The paper is currently under revision.'
# date: 2024-08-14
# venue: 'tba'
# slidesurl: 'https://fa-schwarz.github.io/files/'
# paperurl: 'https://fa-schwarz.github.io/files/'
# protourl: 'https://github.com/'
# citation: 'Schwarz, F., Rossow, C., tba., &quot;tba&quot;. In: <i>tba</i>. tba 2024'
---

This paper has not been published in a peer-reviewed conference yet but is under revision.
A preprint is available at [arXiv:2410.01777](https://arxiv.org/abs/2410.01777).

**Abstract** (preprint)

The confidentiality of cryptographic keys is essential for the security of protection schemes used for communication, file encryption, and outsourced computation. Beyond cryptanalytic attacks, adversaries can steal keys from memory via software exploits or side channels, enabling them to, e.g., tamper with secrets or impersonate key owners. Therefore, existing defenses protect keys in dedicated devices or isolated memory, or store them only in encrypted form. However, these designs often provide unfavorable tradeoffs, sacrificing performance, fine-grained access control, or deployability.

In this paper, we present KeyVisor, a lightweight ISA extension that securely offloads the handling of cryptographic keys to the CPU. KeyVisor provides CPU instructions that enable applications to request protected key handles and perform AEAD cipher operations on them. The underlying keys are accessible only by KeyVisor, and thus never leak to memory. KeyVisor's direct CPU integration enables fast crypto operations and hardware-enforced key usage restrictions, e.g., keys usable only for de-/encryption, with a limited lifetime, or with a process binding. Furthermore, privileged software, e.g., the monitor firmware of TEEs, can revoke keys or bind them to a specific process/TEE. We implement KeyVisor for RISC-V based on Rocket Chip, evaluate its performance, and demonstrate real-world use cases, including key-value databases, automotive feature licensing, and a read-only network middlebox.
