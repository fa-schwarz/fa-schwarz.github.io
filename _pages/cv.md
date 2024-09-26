---
layout: archive
title: "Curriculum Vitae (CV)"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

<head>
  <style>
      p {
          text-align: justify;
      }
  </style>
</head>

{% include base_path %}

_note: PDF versions of my CV are in progress (in EN/GER)_

## Education

* **Ph.D. (_with highest distinction_)** in Computer Science, Saarland University, August 2024  
  _thesis: "TEE-based Designs for Network Gateways, Web Authentication, and VM Introspection"_
* **M.Sc. (_grade: 1.1 / A_)** in Computer Science, Saarland University, November 2017  
  _thesis: "Kernel-based Process Monitoring of Network Services"_
* **B.Sc. (_grade: 1.3 / A_)** in Computer Science, Saarland University, September 2015  
  _thesis: "Security Analysis of Mobile Banking Apps"_

## Work experience

* **Research Assistant** (_full-time position, PhD Student_), 11/2017 -- 08/2024
  * _CISPA Helmholtz Center for Information Security & Saarland University_
  * Supervisor: Prof. Dr. Christian Rossow
  * Responsibilities included:
    * Research on attestable system and network security designs based on trusted execution environments for:  
    network gateways, firewalls, FIDO2 web authentication, and virtual machine introspection (forensics)
    * Design, implementation, and evaluation of research prototypes (proof of concepts)
    * Publication of research papers at international conferences, and presentation at conferences, workshops, and science outreach events (talks, posters)
    * Supervision of (under-)graduate students on cyber security projects, bachelor theses, and research projects

* **Research Immersion Lab**, 11/2016 -- 02/2017
  * _Information Security & Cryptography Chair, CISPA, Saarland University_
  * Supervisor: Dr. Sven Bugiel
  * Topic: "Android Middleware Instrumentation for Fuzzing Support"  
  _Statically instrumenting the Android middleware (system services) to provide middleware-targeting fuzzers with AFL-like code coverage information._

* **Research Immersion Lab**, 06/2016 -- 11/2016
  * _System Security Group, CISPA, Saarland University_
  * Supervisor: Prof. Dr. Christian Rossow
  * Topic: "Long-term Malware Monitoring"  
  _Setting up the Drakvuf execution tracer in our virtualization-based malware analysis framework.
  Evaluating memory deduplication features of hypervisors (KVM, Xen) for scaling the long-term tracing of in-VM malware._

* **Research Assistant** _(student helper)_, 11/2015 -- 02/2016
  * _System Security Group, CISPA, Saarland University_
  * Supervisor: Dr. Giancarlo Pellegrino and Prof. Dr. Christian Rossow
  * Topic: "Security Study of Data Compression in Mobile Services"  
  _Exploring the feasibility of data-flow analysis tools to detect zip bomb-like vulnerabilities in Android apps._

## Awards and Honors

* 2023: "especially noteworthy reviewer" at the RAID 2023 conference (Research in Attacks, Intrusions and Defenses)
* 01/2016 -- 10/2017: scholarship of the Saarbruecken Graduate School of Computer Science at Saarland University
* 05/2013 -- 10/2015: "Bachelor Honors Program" (~top 5% of students) of computer science at Saarland University
* 10/2012 -- 09/2013: scholarship "Deutschlandstipendium" (German public-private scholarship)

## Experience / Skills

During my PhD I have completed five research projects in the area of system, network, and web security, with a focus on designs based on trusted computing (or confidential computing) technologies and their remote attestation protocols.
I was responsible for identifying open research challenges, proposing research questions, designing conceptual solutions, as well as implementing and evaluating concrete technical architectures as prototypes.
Furthermore, I was responsible for publishing the results in the form of research papers and open-source prototypes, and presenting them at renowned international security conferences in the form of technical talks.
In four of the five projects I have been the main author and project lead.
In the fifth one I have been a co-leader.
The projects include intra- and inter-institutional cooperations, and sometimes involved student helpers.

As part of my research, I have gained experience in several technical and non-technical areas, including but not limited to:

* design and implementation of CPU-assisted system and network security architectures, in particular, new solutions based on trusted execution environments (TEEs) and remote attestation for attack isolation, prevention, or detection
* threat analysis with focus on user- and system-level attackers (e.g., malware, rootkits) and network attackers
* writing, publishing, and presenting research papers at international security conferences, and supporting the transfer of research results into a patent request

* practical (hands-on) experience in implementing low-level system security architectures and network services:
  * application areas: traffic-to-app attribution, per-application firewall policies, isolated network firewalls, virtual machine introspection (forensics), FIDO2 web authentication
  * use of trusted execution environments (TEEs) / confidential computing technologies:  
  Intel SGX, Arm TrustZone, AMD SEV (SEV-SNP), OP-TEE OS, Graphene-SGX (now: Gramine)
  * combining TEE-based remote attestation protocols with network (TLS, DTLS) and web protocols (WebAuthn)
  * Linux kernel, virtualization / hypervisor (esp. QEMU KVM), and (NIC) device driver extensions
  * extending user/kernel network services (e.g., TCP/IP stacks, firewalls, NIC interfaces, VPN-like services)
  * interaction with electronic IDs (e.g., ICAO-compliant ePassports with PACE, PA, and EAC)
  * implementation of a virtual FIDO2 authenticator (CTAP, WebAuthn)
  * system programming languages: C, C++, Rust, assembly (x86/arm);  
  others: Python, Go, Java (less experienced)

* other areas of experience include:
  * conceptual design of the hardware/software interface of a RISC-V CPU (co-processor) extension
  * non-TEE CPU extensions, e.g., Intel Keylocker, Intel Processor Trace
  * eBPF-based event tracing (as part of my [master thesis](https://fa-schwarz.github.io/publication/master))
  * understanding Android app permissions and binder IPC (as part of my [bachelor thesis](https://fa-schwarz.github.io/publication/bachelor))

For more details on my finished (research) projects, have a look at my [project portfolio](https://fa-schwarz.github.io/portfolio/) and [list of publications](https://fa-schwarz.github.io/publications/).

I am fluent in German (native language) and English.

## Publications

During my PhD I have published and presented several papers on international research conferences.
One additional publication on a RISC-V CPU extension is currently pending (under revision).

  <ul>{% for post in site.publications reversed %}
    {% if post.category != 'unpublished' and post.category != 'bachelor' and post.category != 'master' %}
      {% include archive-single-cv.html %}
    {% endif %}
  {% endfor %}</ul>

## Supervised Projects

During my PhD I have supervised cyber security projects and bachelor theses of (under-)graduate students.

  <ul>{% for post in site.supervision reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
## Academic Service

I have served as a voluntary helper at international academic conferences, workshops, and journals.

### Program Committee Member

* [RAID conference 2024](https://raid2024.github.io/) (+ award subcommittee)
* [AISCC workshop 2024](https://www.ndss-symposium.org/ndss2024/co-located-events/aiscc/) (co-located with NDSS conference)
* [RAID conference 2023](https://raid2023.org) (award: &quot;[noteworthy reviewer](https://x.com/chrossow/status/1715037102973309026)&quot;)

### Journal Reviewer

* [IEEE TIFS 2022/23](https://signalprocessingsociety.org/publications-resources/ieee-transactions-information-forensics-and-security)