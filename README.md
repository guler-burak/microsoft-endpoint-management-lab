# Microsoft Endpoint Management Lab

Hands-on Microsoft Endpoint Management portfolio focused on the deployment, configuration, security, administration, and automation of modern Windows endpoints.

This repository documents a practical lab environment built while studying Microsoft MD-102 Endpoint Administrator technologies.

The project focuses on real implementation and validation rather than course notes. Each lab documents the configuration performed, supporting evidence, troubleshooting where applicable, and the final result.

---

## Project Scope

The lab environment is designed to cover enterprise endpoint management technologies including:

- Microsoft Intune
- Microsoft Entra ID
- Windows 11
- Windows Server 2022
- Active Directory Domain Services
- Windows Autopilot
- Endpoint Security
- Microsoft Defender
- Windows Update Management
- Application Deployment
- Mobile Application Management
- PowerShell
- Microsoft Graph

---

## Lab Architecture

```text
                         Microsoft Cloud
                +------------------------------+
                | Microsoft Entra ID           |
                | Microsoft Intune             |
                | Microsoft Defender           |
                | Microsoft Graph              |
                +--------------+---------------+
                               |
                               |
                        Managed Endpoints
                               |
              +----------------+----------------+
              |                                 |
              v                                 v
         MD102-CL01                         MD102-CL02
         Windows 11                         Windows 11
        On-Premises                         Cloud Managed
              |
              |
        md102lab.test
              |
              v
         MD102-DC01
     Windows Server 2022
        AD DS + DNS
```

---

## Core Technologies

| Technology | Usage |
|---|---|
| Microsoft Intune | Endpoint configuration and management |
| Microsoft Entra ID | Cloud identity and device management |
| Windows 11 | Managed endpoint platform |
| Windows Server 2022 | On-premises infrastructure |
| Active Directory Domain Services | Domain identity services |
| Microsoft Hyper-V | Virtualization platform |
| Windows Autopilot | Modern Windows provisioning |
| Microsoft Defender | Endpoint security |
| PowerShell | Administration and automation |
| Microsoft Graph | Cloud management and automation |

---

## Lab Progress

| Lab | Topic | Status |
|---|---|---|
| 01 | Hyper-V, Active Directory and Windows 11 Foundation | Completed |
| 02 | Microsoft Entra ID Device Management | Completed |
| 03 | Microsoft Intune Enrollment | Completed |
| 04 | Identity and Compliance | Completed |

---

## Lab 01 - Hyper-V, Active Directory and Windows 11 Foundation

Built the core infrastructure required for the endpoint management environment.

Key implementation areas include Hyper-V virtualization, Windows Server 2022, Active Directory Domain Services, DNS, Windows 11 deployment, domain membership, and infrastructure validation.

[View Lab 01 Documentation](docs/01-lab-foundation/lab-environment.md)

---


## Lab 02 - Microsoft Entra ID Device Management

Joined `MD102-CL02` directly to Microsoft Entra ID and validated the device identity using both the Entra admin center and `dsregcmd`.

A device security group was also created for later Intune policy and application targeting.

[View Lab 02 Documentation](docs/02-entra-id-device-management/entra-device-management.md)

---

## Lab 03 - Microsoft Intune Enrollment

Configured automatic MDM enrollment and enrolled `MD102-CL02` into Microsoft Intune.

The lab includes MDM user scope configuration, enrollment verification, and troubleshooting an endpoint that initially appeared only in Microsoft Entra ID.

[View Lab 03 Documentation](docs/03-intune-enrollment/intune-enrollment.md)

---

## Lab 04 - Identity and Compliance

Configured Microsoft Entra and Intune administrative access, Windows compliance, Conditional Access, Windows Hello for Business, and Windows LAPS.

The lab includes scoped administration, compliance validation on `MD102-CL02`, and LAPS password backup to Microsoft Entra ID.

[View Lab 04 Documentation](docs/04-identity-compliance/identity-compliance.md)

---
## Repository Structure

```text
docs/
    Technical lab documentation

screenshots/
    Validation evidence and configuration screenshots

scripts/
    PowerShell and Microsoft Graph automation scripts

assets/
    Supporting project resources
```

---

## Documentation Approach

Each lab follows a practical documentation structure:

`Objective → Environment → Implementation → Validation → Troubleshooting → Result`

Only configurations that were implemented or explicitly reviewed in the lab environment are documented as such.

---

## Purpose

The purpose of this repository is to demonstrate practical Microsoft Endpoint Management experience through reproducible technical labs and documented validation.

The project is intended to serve as a technical portfolio for Endpoint Administrator, IT Specialist, Modern Workplace, and Microsoft Intune-related roles.




