# IT Home Lab

A small virtual company network built on VMware Workstation Pro, to practise the daily work of an IT support technician and junior system administrator.

By **Samuel-André Anténor**, DEP Soutien informatique student in Quebec. Bilingual French and English.

## Lab network

![Lab network diagram](lab-00-home-lab-setup/images/lab-network.png)

## Environment

| VM | OS | Role | IP address |
| --- | --- | --- | --- |
| DC01 | Windows Server 2025 Standard (Desktop Experience) | Future domain controller | 172.16.0.1 (LAB-NET), NAT for internet |
| CLIENT01 | Windows 11 | Employee PC | 172.16.0.10 (LAB-NET) |
| UBU01 | Ubuntu Server 26.04.1 LTS | Linux practice, SSH | DHCP from VMware NAT |

Host: Dell OptiPlex 5070 (Intel Core i7-8700, 32 GB RAM), lab VMs stored on an SSD.

Networks:
- **LAB-NET**: private VMware LAN segment, 172.16.0.0/24, internal lab traffic only.
- **NAT**: VMware's NAT network, used for internet access and updates.

## Labs

| # | Lab | Skills | Status | Date |
| --- | --- | --- | --- | --- |
| 00 | [Home lab setup](lab-00-home-lab-setup/) | VMware, Windows Server install, static IP, firewall, Ubuntu Server, SSH | In progress | 2026-11 |
| 01 | Active Directory domain controller | AD DS, DNS | Planned | |
| 02 | Users, groups and OUs | Active Directory administration | Planned | |
| 03 | DHCP on DC01 | DHCP, routing | Planned | |
| 04 | Group Policy | GPO, password policy, drive mapping | Planned | |
| 05 | PowerShell automation | Create users from CSV, reports | Planned | |

## Certifications

- CompTIA A+ (studying, target early 2027)
- Microsoft MD-102 Endpoint Administrator (planned)
- CompTIA Network+ (planned)

## Repository structure

```text
it-home-lab/
├── README.md                     this page
├── lab-00-home-lab-setup/
│   ├── README.md                 Lab 00 write-up
│   └── images/                   screenshots
├── scripts/                      PowerShell and Bash scripts
└── docs/
    └── troubleshooting-log.md    every problem, cause and fix
```

## Résumé en français

Laboratoire virtuel construit avec VMware Workstation Pro pour pratiquer le travail d'un technicien en soutien informatique : un serveur Windows Server 2025, un poste client Windows 11 et un serveur Ubuntu, reliés par un réseau interne privé. Chaque laboratoire est documenté avec des captures d'écran, les problèmes rencontrés et leurs solutions.
