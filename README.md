# Microsoft Endpoint Management Lab

Hands-on Microsoft Endpoint Management lab created as part of my MD-102 Endpoint Administrator studies.

This repository documents the implementation, configuration, validation, and troubleshooting of Microsoft endpoint management technologies in a practical lab environment.

## Technologies

- Microsoft Intune
- Microsoft Entra ID
- Windows 11
- Windows Server 2022
- Active Directory Domain Services
- Microsoft Hyper-V
- Windows Autopilot
- Endpoint Security
- PowerShell
- Microsoft Graph

## Lab Progress

| Lab | Topic | Status |
|---|---|---|
| 01 | Lab Foundation & Active Directory | Completed |
| 02 | Microsoft Entra ID Device Management | Planned |
| 03 | Microsoft Intune Enrollment | Planned |
| 04 | Identity & Compliance | Completed |
| 05 | Windows Autopilot | Planned |
| 06 | Device Configuration | Planned |
| 07 | Remote Device Management | Planned |
| 08 | Endpoint Security | Planned |
| 09 | Update Management | Planned |
| 10 | Application Management | Planned |
| 11 | App Protection | Planned |
| 12 | PowerShell & Microsoft Graph Automation | Planned |

## Lab 01 - Lab Foundation

The initial environment includes:

- Hyper-V virtualization
- External virtual networking
- Windows Server 2022
- Active Directory Domain Services
- DNS
- Windows 11 endpoint
- Active Directory domain membership

[View Lab 01 Documentation](docs/01-lab-foundation/lab-environment.md)

## Repository Purpose

## Lab 02 - Microsoft Entra ID Device Management

Configured and validated Microsoft Entra ID device management using a Windows 11 endpoint.

Key tasks included:

- Joining MD102-CL02 directly to Microsoft Entra ID
- Verifying the device join state using `dsregcmd`
- Confirming the device in the Microsoft Entra admin center
- Creating a security group for device management

[View Lab 02 Documentation](docs/02-entra-id-device-management/entra-device-management.md)

## Lab 03 - Microsoft Intune Enrollment

Configured automatic Microsoft Intune enrollment for a Microsoft Entra Joined Windows 11 endpoint.

Key tasks included:

- Configuring the Intune MDM user scope
- Creating the `MD102-Intune-Users` security group
- Adding the test user to the enrollment scope
- Automatically enrolling MD102-CL02 into Microsoft Intune
- Verifying the managed device in the Intune admin center
- Troubleshooting an endpoint that initially appeared only in Microsoft Entra ID

[View Lab 03 Documentation](docs/03-intune-enrollment/intune-enrollment.md)

The purpose of this repository is to demonstrate practical Microsoft Endpoint Management skills through documented hands-on labs rather than only theoretical MD-102 exam preparation.
