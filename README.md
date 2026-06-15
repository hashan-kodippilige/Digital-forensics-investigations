# Digital Forensics Investigations

<p align="center">
  <img src="https://img.shields.io/badge/CAINE%20Linux-333333?style=for-the-badge&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white" />
  <img src="https://img.shields.io/badge/Guymager-4EAA25?style=for-the-badge&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Chain%20of%20Custody-E22C2C?style=for-the-badge&logo=target&logoColor=white" />
  <img src="https://img.shields.io/badge/NIST%20Guidelines-003087?style=for-the-badge&logo=nist&logoColor=white" />
</p>

> Graduate-level digital forensics portfolio covering forensic imaging, evidence preservation, chain of custody, MITM attack detection, ARP poisoning investigation, source code exfiltration analysis, and cybercrime investigation — following NIST forensic methodology throughout.

---

## Overview

This repository documents hands-on digital forensics investigations completed during **graduate-level Digital Forensics coursework** at Minnesota State University Moorhead. Each investigation follows the standard forensic methodology — identification, preservation, collection, examination, analysis, and reporting — using industry-standard tools and legally defensible procedures.

**Notable:** This repo includes actual **Chain of Custody forms** and **Examiner Notes** as `.xlsx` files — artifacts that demonstrate professional forensic practice beyond typical academic coursework.

---

## Forensic Methodology

```
1. Identification   →   Scope the incident and identify evidence sources
2. Preservation     →   Write-block and hash verification to protect evidence integrity
3. Collection       →   Forensic imaging using Guymager / dcfldd
4. Examination      →   Mount images read-only, extract artifacts
5. Analysis         →   Timeline reconstruction, traffic analysis, correlation
6. Reporting        →   Examiner notes, chain of custody, findings report
```

---

## Contents at a Glance

| # | Type | Title | Key Tools |
|---|------|-------|-----------|
| Lab 1 | Lab | Local Bank File Server Breach Investigation | NIST, CFAA, GLBA |
| Project 1 | Project | Forensic Lab Setup & Disk Imaging | CAINE, Guymager, dcfldd |
| Project 2 | Project | MITM Attack Detection via ARP Poisoning | Wireshark, ARP Analysis |
| Project 3 | Project | Source Code Exfiltration Investigation | Wireshark, SMB, Chain of Custody |

---

## Lab 1 — Local Bank File Server Breach Investigation

**Scenario:** A local bank suspects unauthorized access to its file server. Conduct a preliminary investigation following legal and regulatory guidelines.

| Topic | Details |
|-------|---------|
| Legal Framework | Computer Fraud and Abuse Act (CFAA) |
| Regulatory | Gramm-Leach-Bliley Act (GLBA) compliance considerations |
| Data Types | Volatile vs. Non-Volatile data acquisition procedures |
| Guidelines | NIST SP 800-86 forensic methodology |
| Output | Evidence collection plan and legal considerations report |

**Skills:** Legal Frameworks · Evidence Collection Planning · Volatile Data Acquisition · NIST Guidelines

---

## Project 1 — Forensic Lab Setup & Disk Imaging

**Objective:** Build a professional forensic workstation and perform evidence-grade disk imaging with cryptographic verification.

| Task | Tool | Details |
|------|------|---------|
| Forensic workstation setup | CAINE Linux + VirtualBox | Bootable forensic environment |
| Write-blocking | Hardware write blocker | Evidence integrity protection |
| Disk imaging | Guymager | Bit-for-bit forensic image creation |
| Disk imaging (CLI) | dcfldd | Command-line imaging with built-in hashing |
| Integrity verification | MD5 + SHA256 | Cryptographic hash matching |
| Read-only mounting | CAINE Linux | Evidence examined without modification |

**Key Outcome:** Successfully created forensically sound disk images with verified hash values, establishing a legally defensible evidence chain.

**Skills:** CAINE Linux · Guymager · dcfldd · MD5/SHA256 Hashing · Evidence Preservation · Write Blocking

---

## Project 2 — MITM Attack Detection via ARP Poisoning

**Scenario:** Analyze a suspicious packet capture to determine whether a Man-in-the-Middle attack occurred on the network.

### Investigation Process

```
PCAP Acquired  →  Wireshark Analysis  →  ARP Table Inspection
      →  MAC Address Correlation  →  MITM Confirmed  →  Report
```

### Key Findings

| Finding | Evidence |
|---------|---------|
| ARP poisoning confirmed | Duplicate ARP replies from attacker MAC |
| Attacker MAC identified | Isolated via Wireshark endpoint analysis |
| Traffic redirection verified | Victim traffic routing through attacker host |
| MITM attack validated | TCP session reconstruction confirmed interception |

**Traffic Analysis:** IPv4 · TCP · UDP · ARP protocols examined

**Skills:** Wireshark · ARP Analysis · MITM Detection · Packet Analysis · MAC Address Investigation · Incident Validation

---

## Project 3 — Source Code Exfiltration Investigation

**Scenario:** A company suspects an insider threat has exfiltrated proprietary source code via the network. Investigate and produce a court-ready forensic report.

### Investigation Findings

| Stage | Finding |
|-------|---------|
| SMB Traffic Analysis | Authenticated SMB access to shared folder confirmed |
| File Access | Proprietary source code files accessed and copied |
| Outbound Communications | Encrypted outbound traffic to external IP identified |
| Source Code Recovery | Source code file recovered from packet capture |
| Conclusion | Evidence consistent with deliberate data exfiltration |

### Deliverables Produced
- Full forensic investigation report
- **Chain of Custody Form** (`.xlsx`) — legally defensible evidence tracking
- **Examiner Notes** (`.xlsx`) — timestamped investigation log
- Presentation slide deck

**Skills:** SMB Analysis · Timeline Reconstruction · Insider Threat Investigation · Source Code Recovery · Chain of Custody · Forensic Reporting · Evidence Correlation

---

## Repository Contents

```
Digital-forensics-investigations
├── 📄 README.md
├── 📋 Digital Forensics - Lab 1 - Hashan Kodippilige.pdf
├── 📋 Digital Forensics - Project 1 - Hashan Kodippilige.pdf
├── 📋 Digital Forensics - Project 2 - Hashan Kodippilige.pdf
├── 📋 Digital Forensics_Project 2_Hashan Kodippilige.pdf       ← Presentation
├── 📋 Digital Forensics_project 3_Hashan Kodippilige.pdf
├── 📊 Chain of Custody Form_DF_Proj3_Hashan Kodippilige.xlsx   ← Evidence Form
└── 📊 Examiners Notes_DF_Proj3_Hashan Kodippilige.xlsx         ← Investigation Log
```

---

## Tools & Technologies

| Category | Tools |
|----------|-------|
| Forensic Acquisition | CAINE Linux, Guymager, dcfldd |
| Network Forensics | Wireshark |
| Hash Verification | MD5, SHA256 |
| Documentation | Microsoft Excel (Chain of Custody, Examiner Notes) |
| Virtualization | Oracle VirtualBox, Azure Lab |

---

## Skills Demonstrated

`Digital Forensics` `Evidence Acquisition` `Forensic Imaging` `Chain of Custody` `CAINE Linux` `Guymager` `dcfldd` `Wireshark` `ARP Poisoning` `MITM Detection` `SMB Analysis` `Source Code Exfiltration` `Timeline Reconstruction` `Incident Response` `NIST SP 800-86` `CFAA` `GLBA` `Forensic Reporting`

---

## Real-World Relevance

This portfolio maps directly to:
- **Digital Forensics Analyst** roles — full investigation lifecycle from imaging to court-ready reporting
- **Incident Responder** roles — MITM detection, exfiltration analysis, timeline reconstruction
- **SOC Analyst** roles — network traffic forensics and insider threat detection
- **PhD Research** — empirical forensic methodology, legal frameworks, evidence integrity

---

## Disclaimer

All investigations were conducted in **authorized, isolated educational lab environments** using synthetic evidence and simulated scenarios for academic purposes only. No real systems, networks, or individuals were targeted.

---

## Author

**Hashan Kodippilige**  
M.S. Cybersecurity — Minnesota State University Moorhead  
📧 hashansharindu@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/hashankodippilige/)  
🐙 [GitHub](https://github.com/hashan-kodippilige)
