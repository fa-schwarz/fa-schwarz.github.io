---
title: "App-grained Netfilter Policies (SENG-Netfilter)"
collection: supervision
#category: supervision
type: "Student Assistant"
permalink: /supervision/2020-student-netfilter
venue: "Saarland University, CISPA Helmholtz Center for Information Security"
date: 2020-06-30
---

Project by student assistant Leon Trampert.
The goal was to implement a Linux Netfilter extension for our [SENG research project](https://fa-schwarz.github.io/publications/2020-08-12-seng), which enables the specification and enforcement of per-application firewall policies.

The SENG-Netfilter extension trades in SENG's support for unmodified Linux applications for direct integration into the Netfilter subsystem.
That way, SENG's per-application firewall policies can be directly specified using common firewall configuration tools like `iptables`, instead of relying on SENG's original traffic-to-appliaction attribution based on app-specific IP subnetworks.

My responsibility was to come up with the conceptual and technical design of the SENG-Netfilter extension.
In addition, I guided and supervised Leon while he was implementing a research prototype of SENG-Netfilter.
The result has been published as [an open-source project at Github](https://github.com/sengsgx/seng-netfilter).