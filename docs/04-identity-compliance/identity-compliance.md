# Lab 04 - Identity and Compliance



## Objective



Implement identity administration, role-based access control, device compliance, Conditional Access, Windows Hello for Business, and Windows LAPS in a Microsoft Endpoint Management lab.



## Environment



| Component | Configuration |

|---|---|

| Identity Platform | Microsoft Entra ID |

| Endpoint Management | Microsoft Intune |

| Managed Endpoint | MD102-CL02 |

| Device Group | Windows Device Group |

| Scope Tag | MD102-Windows-Scope |



## Entra ID Role Assignment



A Microsoft Entra built-in role was assigned to a test user to demonstrate role-based administration.



![Entra Role Assignment](../../screenshots/04-identity-compliance/01-entra-role-assignment.png)



![Assigned User](../../screenshots/04-identity-compliance/02-entra-role-assigned-user.png)



## Intune RBAC



The Intune `Help Desk Operator` role was assigned through a dedicated administrator security group.



The role assignment was scoped to the Windows device group.



![Intune RBAC Assignment](../../screenshots/04-identity-compliance/03-intune-helpdesk-role-assignment.png)



## Scope Tags



A custom scope tag named `MD102-Windows-Scope` was created and applied to support scoped administration.



![Scope Tag Assignment](../../screenshots/04-identity-compliance/04-intune-scope-tag-assignment.png)



## Device Compliance



A Windows compliance policy named `MD102-Windows-Compliance` was created.



The policy included security requirements such as BitLocker and Secure Boot.



![Compliance Policy](../../screenshots/04-identity-compliance/05-windows-compliance-policy.png)



The policy was assigned to `Windows Device Group`.



![Compliance Assignment](../../screenshots/04-identity-compliance/06-compliance-policy-assignment.png)



Compliance status was successfully evaluated for `MD102-CL02`.



![Compliance Status](../../screenshots/04-identity-compliance/09-compliance-device-status.png)



## Conditional Access



A Conditional Access policy named `MD102-Require-Compliant-Windows` was configured.



The policy evaluates Windows sign-ins and requires the device to be marked as compliant.



The policy was initially configured in report-only mode for safe testing.



![Conditional Access Policy](../../screenshots/04-identity-compliance/07-conditional-access-policy.png)



![Compliance Grant Control](../../screenshots/04-identity-compliance/08-conditional-access-compliance-grant.png)



## Windows Hello for Business



A Windows Hello for Business configuration policy was created and assigned to the Windows device group.



![Windows Hello Settings](../../screenshots/04-identity-compliance/10-windows-hello-policy-settings.png)



![Windows Hello Assignment](../../screenshots/04-identity-compliance/11-windows-hello-policy-assignment.png)



Windows Hello sign-in options were successfully made available on `MD102-CL02`.



![Windows Hello Verification](../../screenshots/04-identity-compliance/12-windows-hello-signin-options.png)



## Windows LAPS



Windows LAPS was enabled for the tenant and configured through Microsoft Intune.



The local administrator password was configured to be backed up to Microsoft Entra ID.



![LAPS Policy](../../screenshots/04-identity-compliance/13-laps-policy-settings.png)



![LAPS Assignment](../../screenshots/04-identity-compliance/14-laps-policy-assignment.png)



![Entra LAPS Enabled](../../screenshots/04-identity-compliance/15-entra-laps-enabled.png)



LAPS event logs confirmed successful local password rotation and Microsoft Entra ID backup.






## Result



The following tasks were completed:



- Implemented Microsoft Entra ID RBAC

- Implemented Microsoft Intune RBAC

- Configured scoped administration

- Created and assigned a Windows compliance policy

- Verified device compliance

- Created a Conditional Access policy based on device compliance

- Configured Windows Hello for Business

- Configured Windows LAPS

- Verified LAPS password rotation and Microsoft Entra ID backup


