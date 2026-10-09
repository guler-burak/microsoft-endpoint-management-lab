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

## Lab 08 - Remote Device Management

Performed and reviewed common Microsoft Intune remote device management actions.

Key tasks included:

- Triggering a device Sync
- Reviewing bulk device actions
- Triggering a Microsoft Defender security intelligence update
- Reviewing BitLocker recovery key rotation
- Creating and assigning a BitLocker disk encryption policy
- Reviewing Intune Device Query with KQL
- Triggering a remote Windows restart
- Reviewing Retire and Wipe without executing destructive actions

[View Lab 08 Documentation](docs/08-remote-device-management/remote-device-management.md)


## Lab 09 - Endpoint Security

Configured and validated Microsoft Intune endpoint security capabilities for a managed Windows 11 endpoint.

Key tasks included:

- Creating a Windows Security Baseline
- Configuring Microsoft Defender Antivirus
- Configuring Microsoft Defender Firewall
- Creating an Endpoint Detection and Response policy
- Creating an Attack Surface Reduction policy
- Connecting Microsoft Intune with Microsoft Defender for Endpoint
- Onboarding `MD102-CL02` to Microsoft Defender for Endpoint
- Validating the device as Active in Defender Device Inventory

[View Lab 09 Documentation](docs/09-endpoint-security/endpoint-security.md)


## Lab 10 - Update Management

Configured and reviewed Windows update management capabilities using Microsoft Intune.

Key tasks included:

- Creating a Windows Update Ring
- Configuring quality and feature update deferrals
- Configuring active hours and update deadlines
- Monitoring Windows update deployment status
- Reviewing update troubleshooting workflows
- Reviewing Android and Apple update management
- Creating a Delivery Optimization policy
- Configuring peer-to-peer update delivery for Windows devices

[View Lab 10 Documentation](docs/10-update-management/update-management.md)


## Lab 11 - Application Management

Configured and reviewed application deployment capabilities using Microsoft Intune.

Key tasks included:

- Deploying VLC through Microsoft Store (new)
- Creating a Microsoft 365 Apps configuration
- Assigning Microsoft 365 Apps to the Windows Device Group
- Reviewing Office Deployment Tool and Office Customization Tool
- Configuring Microsoft 365 Apps Cloud Policy
- Reviewing platform-specific application store deployment

[View Lab 11 Documentation](docs/11-application-management/application-management.md)


## Lab 12 - App Protection & App Configuration

Configured Microsoft Intune Mobile Application Management and app configuration capabilities.

Key tasks included:

- Creating an iOS/iPadOS App Protection Policy
- Configuring organizational data protection controls
- Assigning App Protection to the MD102-Intune-Users group
- Creating a Conditional Access policy requiring App Protection
- Configuring Conditional Access in Report-only mode
- Creating an Outlook App Configuration Policy
- Reviewing managed apps and managed device scenarios

[View Lab 12 Documentation](docs/12-app-protection/app-protection.md)


## Lab 13 - PowerShell & Microsoft Graph Automation

Used PowerShell and Microsoft Graph to query Microsoft Entra ID and Microsoft Intune resources.

Key tasks included:

- Installing the Microsoft Graph PowerShell SDK
- Connecting PowerShell to Microsoft Graph
- Querying Microsoft Entra ID users
- Querying Microsoft Entra ID groups
- Querying Microsoft Intune managed devices
- Reviewing endpoint management automation scenarios
- Reviewing Microsoft Security Copilot concepts and integrations

[View Lab 13 Documentation](docs/13-graph-automation/graph-automation.md)


## Lab 14 - Windows Personalization & Corporate Branding

Implemented centralized Windows corporate branding using Microsoft Intune.

Key tasks included:

- Creating a Windows Settings Catalog personalization policy
- Configuring desktop wallpaper through Intune
- Configuring the Windows lock screen image
- Hosting branding assets in GitHub
- Assigning the policy to the Windows Device Group
- Validating the policy on MD102-CL02
- Verifying successful desktop and lock screen configuration

[View Lab 14 Documentation](docs/14-windows-personalization/windows-personalization.md)

## Repository Purpose

The purpose of this repository is to demonstrate practical Microsoft Endpoint Management skills through documented hands-on labs rather than only theoretical MD-102 exam preparation.








