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
| 02 | Microsoft Entra ID Device Management | Completed |
| 03 | Microsoft Intune Enrollment | Completed |
| 04 | Identity & Compliance | Completed |
| 05 | Windows Autopilot | Completed |
| 06 | Device Configuration | Completed |
| 07 | Intune Suite Add-on Capabilities | Completed |
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

## Lab 04 - Identity and Compliance

Implemented identity, access control, device compliance, and endpoint security capabilities using Microsoft Entra ID and Microsoft Intune.

Key tasks included:

- Configuring Microsoft Entra ID role assignments
- Implementing Microsoft Intune RBAC
- Configuring scope tags and scoped administration
- Creating and assigning a Windows compliance policy
- Monitoring device compliance
- Configuring Conditional Access based on device compliance
- Deploying Windows Hello for Business
- Configuring Windows LAPS
- Verifying LAPS password rotation and Microsoft Entra ID backup

[View Lab 04 Documentation](docs/04-identity-compliance/identity-compliance.md)

## Lab 05 - Windows Autopilot

Implemented and validated a Windows Autopilot deployment using Microsoft Intune.

Key tasks included:

- Registering MD102-CL02 with Windows Autopilot
- Creating a user-driven Autopilot deployment profile
- Configuring Microsoft Entra join
- Creating an Enrollment Status Page
- Resetting the Windows endpoint to OOBE
- Successfully validating the Autopilot deployment workflow

[View Lab 05 Documentation](docs/05-windows-autopilot/windows-autopilot.md)

## Lab 06 - Device Configuration

Implemented and validated Windows device configuration using Microsoft Intune.

Key tasks included:

- Creating a Windows Settings Catalog profile
- Assigning configuration policies to managed Windows devices
- Monitoring configuration profile deployment
- Creating and testing a single-app Microsoft Edge kiosk
- Validating kiosk mode on MD102-CL02
- Reviewing Android and iOS configuration concepts

[View Lab 06 Documentation](docs/06-device-configuration/device-configuration.md)

## Lab 07 - Intune Suite Add-on Capabilities

Explored selected Microsoft Intune Suite capabilities.

Key tasks included:

- Enabling Endpoint Analytics
- Reviewing endpoint performance reporting
- Enabling Microsoft Remote Help
- Configuring Remote Help tenant settings
- Validating the Remote Help client on MD102-CL02
- Reviewing Microsoft Tunnel architecture

[View Lab 07 Documentation](docs/07-intune-suite-addons/intune-suite-addons.md)

## Repository Purpose

The purpose of this repository is to demonstrate practical Microsoft Endpoint Management skills through documented hands-on labs rather than only theoretical MD-102 exam preparation.

