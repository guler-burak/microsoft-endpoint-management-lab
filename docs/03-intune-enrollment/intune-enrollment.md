\# Lab 03 - Microsoft Intune Enrollment



\## Objective



Configure automatic Microsoft Intune enrollment for a Windows 11 endpoint and verify successful MDM management.



\## Environment



| Component | Configuration |

|---|---|

| Endpoint | MD102-CL02 |

| Operating System | Windows 11 |

| Identity | Microsoft Entra Joined |

| MDM Platform | Microsoft Intune |

| Enrollment Method | Automatic MDM Enrollment |



\## Automatic Enrollment



A Microsoft Entra security group named `MD102-Intune-Users` was created for Intune enrollment targeting.



The Microsoft Intune MDM user scope was configured to include this user group.



!\[Automatic Enrollment Scope](../../screenshots/03-intune-enrollment/01-automatic-enrollment-mdm-scope.png)



\## Intune Enrollment



`MD102-CL02` was rejoined to Microsoft Entra ID after the MDM user scope was configured.



During the Microsoft Entra join process, automatic MDM enrollment registered the device with Microsoft Intune.



The device was then verified in the Microsoft Intune admin center.



!\[Intune Enrolled Device](../../screenshots/03-intune-enrollment/02-intune-enrolled-device.png)



\## Troubleshooting



The device initially appeared in Microsoft Entra ID but did not appear in Microsoft Intune.



The cause was that the device had been joined to Microsoft Entra ID before the Intune MDM user scope was configured.



After configuring the MDM user scope and rejoining the endpoint to Microsoft Entra ID, automatic Intune enrollment completed successfully.



\## Result



The following tasks were completed:



\- Configured Microsoft Intune automatic MDM enrollment

\- Created an Intune enrollment user group

\- Added the test user to the enrollment scope

\- Enrolled a Microsoft Entra Joined Windows 11 device into Intune

\- Verified the device in the Microsoft Intune admin center

\- Troubleshot an existing device that was not automatically enrolled

