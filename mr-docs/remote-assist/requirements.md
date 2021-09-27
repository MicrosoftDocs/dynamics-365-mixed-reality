---
author: sophiasysun
description:  Technical requirements for deploying and using Microsoft Dynamics 365 Remote Assist
ms.author: sopsun
ms.date: 07/06/2021
ms.service: crm-online
ms.topic: article
title: Requirements for Dynamics 365 Remote Assist
ms.reviewer: krbjoran
---

# Technical requirements for deploying and using Dynamics 365 Remote Assist

This article describes the technical requirements for deploying and using Microsoft Dynamics 365 Remote Assist.

## Definitions

**Dynamics 365 Remote Assist user:** Someone who uses the Dynamics 365 Remote Assist app on HoloLens or mobile devices.

**Teams user:** Someone who uses the Teams app on the desktop or mobile devices.

## Device requirements

Both Dynamics 365 Remote Assist users and Teams users can join a Dynamics 365 Remote Assist call. [Learn more about the different types of calls](./mobile-app/making-calls-on-remote-assist-mobile.md).

The Dynamics 365 Remote Assist app is available on HoloLens, HoloLens 2, and qualifying Android or iOS mobile devices.

If an individual wants to join a Dynamics 365 Remote Assist call using the Teams app, they must use the Teams app on Windows 10 PC or mobile devices.

### Device options and requirements for a Dynamics 365 Remote Assist user

| Device                                   | OS requirements                                                                                                                                                                                                          | Details                                                                                                                                                                                                                  |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Dynamics 365 Remote Assist on HoloLens or HoloLens 2 | HoloLens or HoloLens 2 running 10.0.17134.0 (Windows 10 April 2018) build or later. We recommend [updating](/hololens/hololens-updates) HoloLens to newer versions when available. | See [Manage updates to HoloLens](/HoloLens/hololens-updates) for instructions on using Windows Update for Business, Mobile Device Management (MDM), and Windows Server Update Services (WSUS). |
| Dynamics 365 Remote Assist on mobile devices          | Dynamics 365 Remote Assist mobile is available on all devices, including ARCore-enabled Android phones or tablets, ARKit-enabled iOS iPhones or iPads, and mobile devices without AR support.                                                                               | See [Android AR-supported devices](https://developers.google.com/ar/discover/supported-devices) and [iOS ARCore-supported devices](https://developers.google.com/ar/discover/supported-devices#ios). For more information on how to use Dynamics 365 Remote Assist on devices without AR support, see [Dynamics 365 Remote Assist mobile calls on mobile devices without augmented reality support](./mobile-app/calls-using-devices-without-ar.md).                                         |

### Device options and requirements for a Teams user

| Device                             | OS requirements                                             | Details                                                                                                                                                                                                                                                                                 |
| ---------------------------------- | ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Teams application on Windows 10 PC | Any Windows 10 build.                                       | A Windows 10 PC running the Teams PC application can collaborate with Dynamics 365 Remote Assist on HoloLens, HoloLens 2, or qualifying [Android](https://developers.google.com/ar/discover/supported-devices) or [iOS](https://www.apple.com/ios/augmented-reality/) mobile devices.                |
| Teams application on mobile device | Any iOS or Android phone or tablet running  Teams. | A phone or tablet running the Teams mobile application can collaborate with Dynamics 365 Remote Assist on HoloLens, HoloLens 2, or qualifying [Android](https://developers.google.com/ar/discover/supported-devices) or [iOS](https://www.apple.com/ios/augmented-reality/) mobile devices. |

> [!Note] 
> Dynamics 365 Remote Assist may not be available in your country. For more information, see [Dynamics 365 Remote Assist mobile availability](./mobile-app/faq-mobile.md).

## Licensing and product requirements per role

### Dynamics 365 Remote Assist app user

A Dynamics 365 Remote Assist license includes the following three products needed to use most features available in the Dynamics 365 Remote Assist HoloLens app, mobile app, or web app:

* Dynamics 365 Remote Assist 
* Microsoft Teams
* Microsoft Dataverse

> [!NOTE]
> Dynamics 365 Remote Assist does not currently comply with Microsoft Teams policies. 

| **Included with Dynamics 365 Remote Assist license** | **What capabilities are available?**                                                                                                                                                                                                                                                                                                       |
| --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Dynamics 365 Remote Assist and Teams**             | Use calling features via the Dynamics 365 Remote Assist app on HoloLens or mobile devices. Features include: </br> - Make a call </br> - Use mixed-reality annotations                                            |
| **Microsoft Dataverse**                 | - Access to the Dynamics 365 Remote Assist model-driven app </br> - [Create and manage assets](./asset-capture-overview.md) either within or outside a Dynamics 365 Remote Assist call </br> - Create and share one-time call links </br> - See analytics and insights based on your call records |

An Azure Active Directory account is also required for purchasing the Dynamics 365 Remote Assist subscription and for assigning licenses. You'll need an Azure AD account for each licensed user. They'll use this account when signing in to the app. 

> [!Note]
> The Dynamics 365 Remote Assist, Teams, and Dataverse licenses must be assigned to a native member of the tenant ([Azure AD member](/azure/active-directory/fundamentals/users-default-permissions#member-and-guest-users) account). Dynamics 365 Remote Assist does not support [Azure AD B2B](/azure/active-directory/external-identities/what-is-b2b); an individual cannot sign into Dynamics 365 Remote Assist using a Dynamics 365 Remote Assist license assigned to an Azure AD guest account. 

**With the following software, you can leverage even more capabilities.**

| **If you have this service:**                                                                                                          | **You can access these additional capabilities through Dynamics 365 Remote Assist:**                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| [OneDrive for Business](https://www.microsoft.com/en-us/microsoft-365/onedrive/compare-onedrive-plans?activetab=tab:primaryr2) | - Access and share OneDrive files </br> - Send snapshots </br> - Save snapshots to OneDrive </br> - Save photos received through text chat                                                                     |
| [Exchange Online](https://www.microsoft.com/en-us/microsoft-365/business/compare-all-microsoft-365-business-products-b?ef_id=b13c56e0ea01182d16fa364e92f99bec:G:s&OCID=AID2100137_SEM_b13c56e0ea01182d16fa364e92f99bec:G:s&lnkd=Bing_O365SMB_App&msclkid=b13c56e0ea01182d16fa364e92f99bec)| - Receive meeting invites to join meetings from Dynamics 365 Remote Assist<br>- Schedule a one-time call|
| [Dynamics 365 Field Service](https://dynamics.microsoft.com/en-us/field-service/overview/?ef_id=a6382fe92a19180023784f4753c4a638:G:s&OCID=AID2100366_SEM_a6382fe92a19180023784f4753c4a638:G:s&msclkid=a6382fe92a19180023784f4753c4a638)                                                                                                     | - Call an expert listed in a field service work order </br> - Save call artifacts (for example, call recording, files shared) to a Field Service work order <br>- Browse a Dynamics 365 Field Service booking and change the booking status directly from Dynamics 365 Remote Assist while doing the scheduled task |
| [Power BI](https://www.microsoft.com/en-us/resilience/business-insights-analytics-solutions?ef_id=b8a24caec6781d220ebc2c00bc6856aa:G:s&OCID=AID2100615_SEM_b8a24caec6781d220ebc2c00bc6856aa:G:s&msclkid=b8a24caec6781d220ebc2c00bc6856aa)                                                                                                                       | - View a Power BI dashboard embedded in a Field Service work order<br><br>Note that using the [Calls dashboard in the model-driven app](one-time-call.md) does not require a Power BI license.                                                                                   |
| [Microsoft Stream](https://www.microsoft.com/en-us/microsoft-365/microsoft-stream)                 | - [Record Remote Assist calls](./record-calls-hololens.md) either from within the Remote Assist app, or from the Teams app |


### Microsoft Teams app user

| **What license does the Teams user have?**                                                                                     | **Capabilities in a Dynamics 365 Remote Assist call:**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| None                                                                                                                           | - Teams desktop user can join a call using a [one-time call link](one-time-call.md) </br> - Teams desktop user can [join a meeting](./teams-pc-all.md) that allows anonymous participants </br> -  Use mixed-reality annotations                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Teams                                                                                                                          | The Teams user’s experience is **_identical_** regardless of whether the Teams user is: </br> - A member in the Dynamics 365 Remote Assist user’s tenant </br> - [A guest](./multi-tenant-deployment.md#solution-2-guest-access) in the Dynamics 365 Remote Assist user’s tenant </br> - A member in a tenant that’s [federated](./multi-tenant-deployment.md#solution-1-external-access-federation) with the Dynamics 365 Remote Assist user’s tenant (Teams desktop only) </br> **_EXCEPT_** </br> -  Any differences described [here](/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access). </br><br> Additional collaboration capabilities include: </br> -  Make a call </br> - Record a call |
| [OneDrive for Business](https://www.microsoft.com/microsoft-365/onedrive/compare-onedrive-plans?activetab=tab:primaryr2) | - Share OneDrive files </br> - Send snapshots </br> - Save snapshots to OneDrive    |

### Administrator

[Azure Active Directory (Azure AD)](/azure/active-directory/fundamentals/active-directory-whatis) account to assign licenses in Microsoft 365 admin portal and distribute applications through Microsoft Store for Business. [Learn more about how to deploy Dynamics 365 Remote Assist](deploy-remote-assist.md).

## Network requirements

A variety of network conditions, including bandwidth, latency, jitter, and packet loss, can impact your video calling experience. Although audio and video calls might be possible in environments with reduced bandwidth, you might experience feature degradation.

### Dynamics 365 Remote Assist mobile

When using Dynamics 365 Remote Assist on mobile devices, a minimum of 1.5 Mbps up/down is required for peer-to-peer HD quality video calling with resolution of HD 720p at 15fps.

If Dynamics 365 Remote Assist mobile autodetects that the technician is experiencing [poor network conditions](./mobile-app/poor-network-connectivity.md#poor-network-connectivity-is-determined-by-the-following-conditions), it will prompt the technician to share high-quality snapshots instead of transmitting a low-quality live video feed. See [Calls in low bandwidth](mobile-app/poor-network-connectivity.md) for more information.

### Dynamics 365 Remote Assist HoloLens

When using Dynamics 365 Remote Assist on HoloLens, a minimum of 1.5 Mbps up/down is required for peer-to-peer HD-quality video calling with resolution of HD 1080p at 30 fps. In general, when more bandwidth is available, quality and usage will increase to deliver the best experience. For **optimal** peer-to-peer HD-quality video calling with resolution of HD 1080p, 4-5 Mbps up/down is required. However, in some circumstances, even 4-5 Mbps up/down does not guarantee 1080p video calling at full quality. Circumstances include using HoloLens (first gen).

### URLs and ports
The following list contains the *minimum* URL end points and TCP/UDP ports utilized by Dynamics 365 Remote Assist. All must be reachable from the Dynamics 365 Remote Assist app. If you have specialized needs and/or scale, see the [Teams comprehensive list](/microsoftteams/prepare-network) for specifics.

#### Teams
- *.registrar.skype.com
- *.teams.microsoft.com
- UDP: 3478, 3479, 3480, 3481

#### Authentication
- login.microsoft.com
- login.microsoftonline.com
- login.live.com
- TCP: 80, 443

#### Microsoft GraphExplorer
- graph.microsoft.com
- TCP: 80, 443

#### Enterprise Configuration Service
- ecs.office.com
- TCP: 80, 443

#### Dynamics Services
- *.crm.dynamics.com
- TCP: 80, 443

#### Sharepoint / OneDrive
- *.sharepoint.com
- TCP: 80, 443

#### Windows Notification Service
- *.notify.windows.com
- *.wns.windows.com
- *.notify.live.net
- TCP: 80, 443

#### Connection Test
- *.msftconnecttest.com
- TCP: 80, 443


### Network optimization recommendations

The following tasks serve as a checklist for other potential optimizations for Dynamics 365 Remote Assist:

- [Monitor your network using CQD and call analytics](/MicrosoftTeams/prepare-network#best-practice-monitor-your-network-using-cqd-and-call-analytics).
- Review Teams' recommendations [for optimizing your network](/MicrosoftTeams/prepare-network#network-optimization).
- Be on a dedicated SSID. The dedicated SSID should be on the 5-Ghz band only; disable 2.4 Ghz.
- Use a router with MU-MIMO capabilities.

### Additional resources

- Learn how to troubleshoot and address internal infrastructure issues using [Teams Call Analytics](/MicrosoftTeams/use-call-analytics-to-troubleshoot-poor-call-quality#troubleshoot-call-quality-problems-using-call-analytics) or [Teams Call Quality Dashboard (CQD)](/MicrosoftTeams/quality-of-experience-review-guide).

- See [Prepare your organization's network for Microsoft Teams](/MicrosoftTeams/prepare-network) to learn more.

## See also

- [Overview of Dynamics 365 Remote Assist](ra-overview.md)
- [Try Dynamics 365 Remote Assist for free](try-remote-assist.md)
- [Buy Dynamics 365 Remote Assist](deploy-remote-assist.md)
- [Use Dynamics 365 Remote Assist on HoloLens](overview-hololens.md)
- [Set up and use Microsoft Teams with Dynamics 365 Remote Assist](teams-pc-all.md)
- [How-to videos](videos.md)



[!INCLUDE[footer-include](../includes/footer-banner.md)]
