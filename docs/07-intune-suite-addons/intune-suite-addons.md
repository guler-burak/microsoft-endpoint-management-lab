\# Lab 07 - Intune Suite Add-on Capabilities



\## Objective



Explore and configure selected Microsoft Intune Suite capabilities, including Endpoint Analytics and Remote Help.



\## Environment



| Component | Configuration |

|---|---|

| Endpoint | MD102-CL02 |

| Management Platform | Microsoft Intune |

| Identity Platform | Microsoft Entra ID |

| Remote Support | Microsoft Remote Help |



\## Endpoint Analytics



Endpoint Analytics was enabled to collect performance and user experience data from managed devices.



The feature provides visibility into areas such as:



\- Startup performance

\- Application reliability

\- Resource performance

\- Work from anywhere

\- Battery health



!\[Endpoint Analytics Overview](../../screenshots/07-intune-suite-addons/01-endpoint-analytics-overview.png)



The environment initially reported insufficient data because Endpoint Analytics requires time to collect and process device telemetry.



\## Remote Help



Microsoft Remote Help was enabled in the Intune tenant.



Remote Help was configured to support remote assistance scenarios, including support for unenrolled devices.



!\[Remote Help Settings](../../screenshots/07-intune-suite-addons/02-remote-help-settings.png)



The Remote Help application was installed and successfully opened on `MD102-CL02`.



The device was ready to either request help or generate a security code for a remote assistance session.



!\[Remote Help Ready](../../screenshots/07-intune-suite-addons/03-remote-help-ready.png)



\## Microsoft Tunnel



Microsoft Tunnel architecture and use cases were reviewed.



Microsoft Tunnel provides secure VPN connectivity for managed mobile devices to access on-premises resources.



A Tunnel gateway was not deployed in this lab because the environment does not include the required Linux gateway and mobile device infrastructure.



\## Result



The following tasks were completed:



\- Enabled Microsoft Endpoint Analytics

\- Reviewed endpoint performance and experience reporting

\- Enabled Microsoft Remote Help

\- Configured Remote Help tenant settings

\- Installed and validated the Remote Help client

\- Reviewed Microsoft Tunnel architecture and use cases

