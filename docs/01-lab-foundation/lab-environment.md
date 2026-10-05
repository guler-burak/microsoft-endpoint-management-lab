# Lab 01 - Hyper-V, Active Directory and Windows 11 Foundation

## Objective

Build the base infrastructure required for the Microsoft Endpoint Management lab.

The environment will be used throughout later labs involving Microsoft Entra ID, Microsoft Intune, Windows Autopilot, compliance, endpoint security, application deployment, update management, PowerShell, and Microsoft Graph.

## Environment

| Component | Configuration |
|---|---|
| Hypervisor | Microsoft Hyper-V |
| Virtual Switch | MD102-External |
| Domain Controller | MD102-DC01 |
| Client | MD102-CL01 |
| Server OS | Windows Server 2022 Datacenter Evaluation |
| Client OS | Windows 11 |
| Active Directory Domain | md102lab.test |
| DNS | Active Directory integrated DNS |

---

## 1. Hyper-V Configuration

Microsoft Hyper-V was enabled on the host computer to provide the virtualization platform for the lab.

![Hyper-V Enabled](../../screenshots/01-lab-foundation/01-hyperv-enabled.png)

---

## 2. External Virtual Switch

An external Hyper-V virtual switch named `MD102-External` was created to provide network connectivity to the virtual machines.

![External Virtual Switch](../../screenshots/01-lab-foundation/02-external-virtual-switch.png)

### Troubleshooting

During the initial configuration, Hyper-V was unable to create the external virtual switch because the physical wireless adapter was already associated with an existing Windows Network Bridge.

The conflicting Network Bridge was removed and the external Hyper-V switch was then created successfully.

---

## 3. Windows Server 2022 Deployment

A Windows Server 2022 virtual machine was deployed in Hyper-V.

Computer name:

`MD102-DC01`

![Windows Server 2022](../../screenshots/01-lab-foundation/03-server-2022-installed.png)

---

## 4. Windows 11 Endpoint

A Windows 11 virtual machine was deployed as the primary managed endpoint.

Computer name:

`MD102-CL01`

![Windows 11 Endpoint](../../screenshots/01-lab-foundation/04-windows11-system-about.png)

---

## 5. Active Directory Domain Services

Active Directory Domain Services and DNS were configured on `MD102-DC01`.

The Active Directory domain created for the lab is:

`md102lab.test`

Domain Controller functionality and core Active Directory services were validated using PowerShell.

Commands used:

```powershell
Get-ADDomainController
Get-Service DNS,Netlogon,NTDS
```

![Domain Controller Verification](../../screenshots/01-lab-foundation/05-domain-controller-verification.png)

---

## 6. Windows 11 Domain Join

`MD102-CL01` was joined to the `md102lab.test` Active Directory domain.

The domain join and communication with the domain controller were successfully verified.

Validation included:

- Domain membership
- DNS resolution
- Domain Controller discovery
- Active Directory connectivity

![Windows 11 Domain Join Verification](../../screenshots/01-lab-foundation/06-windows11-domain-join-verification.png)

---

## Result

The base infrastructure for the Microsoft Endpoint Management lab was successfully deployed and validated.

The completed environment includes:

- Microsoft Hyper-V
- External virtual networking
- Windows Server 2022
- Active Directory Domain Services
- Active Directory integrated DNS
- Domain Controller `MD102-DC01`
- Active Directory domain `md102lab.test`
- Windows 11 endpoint `MD102-CL01`
- Successful Windows 11 domain join

This environment provides the foundation for the remaining Microsoft Endpoint Management and MD-102 labs.
