\# Lab 02 - Microsoft Entra ID Device Management



\## Objective



Configure and validate Microsoft Entra ID device management concepts in a Windows 11 lab environment.



The objectives of this lab were to:



\- Understand Microsoft Entra device join types

\- Join a Windows 11 device directly to Microsoft Entra ID

\- Validate the device join state

\- Review Microsoft Entra registered devices

\- Create a security group for device management

\- Understand dynamic device membership concepts



\---



\## Environment



| Component | Configuration |

|---|---|

| Cloud Identity Platform | Microsoft Entra ID |

| Windows Endpoint | MD102-CL02 |

| Join Type | Microsoft Entra Joined |

| On-Premises Domain Membership | None |

| Device Management Group | Security Group |



\---



\## 1. Microsoft Entra Device Join Types



Microsoft Entra ID supports multiple device identity models.



\### Microsoft Entra Joined



Designed primarily for organization-owned devices that are joined directly to Microsoft Entra ID.



\### Microsoft Entra Registered



Typically used when a user connects a work or school account to a personally owned device.



\### Microsoft Entra Hybrid Joined



Used when a device is joined to an on-premises Active Directory domain and also registered with Microsoft Entra ID.



In this lab, `MD102-CL02` was configured as a Microsoft Entra Joined device.



\---



\## 2. Microsoft Entra Join



A Windows 11 virtual machine named:



`MD102-CL02`



was joined directly to Microsoft Entra ID.



The device was then verified from the Microsoft Entra admin center.



!\[Microsoft Entra Joined Device](../../screenshots/02-entra-id-device-management/01-entra-joined-device.png)



\---



\## 3. Device Join Verification



The Windows device registration status was validated locally by using:



```powershell

dsregcmd /status

