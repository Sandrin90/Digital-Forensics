# CIP-B103: Network Forensics Fundamentals - Lab Reports

## Student & Course Information
* **Institution:** International Cybersecurity and Digital Forensics Academy (ICDFA)
* **Course:** CIP-B103: Network Forensics Fundamentals
* **Student Name:** Wihbedimbom Sandrin
* **Student ID:** C11/26/DFIT/17292 
* **Instructor Name:** Dr. Sarah James
* **Submission Date:** August 7, 2026
* **Repository Status:** Complete / Ready for Grading

---

## Overview
This repository contains the complete lab reports and documentation for **Labs 4, 5, and 6** of the CIP-B103 module. Each report is formatted according to the ICDFA Lab Assignment Template Guide and includes executive summaries, detailed technical methodologies, command logs, packet capture timeline analysis tables, forensic findings, and recommended security mitigations.

---

## Repository Contents

| Lab ID | Module / Subject | Document File | Key Topics & Tools |
| :--- | :--- | :--- | :--- |
| **Lab 4** | **SMTP Email Traffic Forensics** | | Wireshark, tshark, Python Base64 offline decoding, TCP stream reassembly, MIME encapsulation, plaintext SMTP port 25. |
| **Lab 5** | **ARP Poisoning Forensics** | Scapy, ARP request/reply field structures, Man-In-The-Middle (MITM) detection, duplicate IP/MAC analysis, Dynamic ARP Inspection (DAI). |
| **Lab 6** | **Firewall Traffic Control & Verification** |  | `iptables`, Netfilter, `curl`, Apache2, `DROP` vs. `REJECT` traffic signature analysis, TCP SYN retransmissions, firewall hit counters. |

---

## Summary of Completed Exercises

### Lab 4: SMTP Email Traffic Forensics
* Reassembled unencrypted TCP streams to extract full MIME headers and email body payloads.
* Decoded Base64 authentication parameters offline using Python (`base64` module) to extract credentials safely.
* Identified network identifiers, user agent software (Outlook 12.0), and extracted plain-text attached files (`NEWS.txt`).

### Lab 5: ARP Poisoning Forensics
* Compared standard broadcast ARP resolution with malicious unicast ARP poisoning traffic.
* Analyzed an active MITM capture (`arp.pcap`) where an attacker system intercepted gateway and victim traffic.
* Simulated controlled ARP poisoning in a virtual lab and restored system ARP caches using cleanup routines.

### Lab 6: Firewall Traffic Control and Forensic Verification
* Configured host-based filtering rules using Linux `iptables` on an Apache web server.
* Captured and analyzed network behavior during `-j DROP` rule enforcement.
* Correlated client application timeouts (`curl: (28) Connection timed out`) with packet retransmissions and `iptables` byte counter statistics.

-
