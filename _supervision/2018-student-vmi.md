---
title: "VMI-based behaviour monitoring of malware"
collection: supervision
#category: supervision
type: "Student Assistant"
permalink: /supervision/2018-student-vmi
venue: "Saarland University, CISPA Helmholtz Center for Information Security"
date: 2018-08-15
---

Project by student assistant Patrick Schmelzeisen.
The goals was to extend our dynamic malware analysis sandbox ([Sandnet](https://dl.acm.org/doi/10.1145/1978672.1978682)) with capabilities to identify and hook dynamic libraries of user space malware via virtual machine introspection (VMI) techniques.
In particular, we aimed at using the [Drakvuf](https://drakvuf.com/) project for the [Xen hypervisor](https://xenproject.org/) to hook SSL/TLS libraries used by malware in order to monitor their unencrypted network traffic.

I have co-supervised the project together with Dr. Johannes Krupp, Michael Brengel, and Prof. Dr. Christian Rossow.