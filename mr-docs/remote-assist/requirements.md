---
author: sophiasysun
description:  Technical requirements for deploying and using Microsoft Dynamics 365 Remote Assist
ms.author: sopsun
ms.date: 04/28/2021
ms.service: crm-online
ms.topic: article
title: Requirements for Dynamics 365 Remote Assist
ms.reviewer: krbjoran
---

# Technical requirements for deploying and using Dynamics 365 Remote Assist

[!INCLUDE[cc-data-platform-banner](../includes/cc-data-platform-banner.md)]

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
| Dynamics 365 Remote Assist on HoloLens or HoloLens 2 | HoloLens or HoloLens 2 running 10.0.17134.0 (Windows 10 April 2018) build or later. We recommend [updating](https://docs.microsoft.com/hololens/hololens-updates) HoloLens to newer versions when available. | See [Manage updates to HoloLens](https://docs.microsoft.com/HoloLens/hololens-updates) for instructions on using Windows Update for Business, Mobile Device Management (MDM), and Windows Server Update Services (WSUS). |
| Dynamics 365 Remote Assist on mobile devices          | Dynamics 365 Remote Assist mobile is available on all devices, including ARCore-enabled Android phones or tablets, ARKit-enabled iOS iPhones or iPads, and mobile devices without AR support.                                                                               | See [Android AR-supported devices](https://developers.google.com/ar/discover/supported-devices) and [iOS ARCore-supported devices](https://developers.google.com/ar/discover/supported-devices#ios). For more information on how to use Dynamics 365 Remote Assist on devices without AR support, see [Dynamics 365 Remote Assist mobile calls on mobile devices without augmented reality support](mobile-app/using-devices-without-AR.md).                                         |

### Device options and requirements for a Teams user

| Device                             | OS requirements                                             | Details                                                                                                                                                                                                                                                                                 |
| ---------------------------------- | ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Teams application on Windows 10 PC | Any Windows 10 build.                                       | A Windows 10 PC running the Teams PC application can collaborate with Dynamics 365 Remote Assist on HoloLens, HoloLens 2, or qualifying [Android](https://developers.google.com/ar/discover/supported-devices) or [iOS](https://www.apple.com/ios/augmented-reality/) mobile devices.                |
| Teams application on mobile device | Any iOS or Android phone or tablet running  Teams. | A phone or tablet running the Teams mobile application can collaborate with Dynamics 365 Remote Assist on HoloLens, HoloLens 2, or qualifying [Android](https://developers.google.com/ar/discover/supported-devices) or [iOS](https://www.apple.com/ios/augmented-reality/) mobile devices. |

> [!Note] 
> Dynamics 365 Remote Assist may not be available in your country. For more information, see [Dynamics 365 Remote Assist mobile availability](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/mobile-app/faq-mobile#what-countries-is-dynamics-365-remote-assist-for-mobile-supported).

## Licensing and product requirements per role

### Dynamics 365 Remote Assist app user

A Dynamics 365 Remote Assist license includes the following three products needed to use most features available in the Dynamics 365 Remote Assist HoloLens app, mobile app, or web app:

* Dynamics 365 Remote Assist 
* Microsoft Teams
* Microsoft Dataverse

| **Included with Dynamics 365 Remote Assist license** | **What capabilities are available?**                                                                                                                                                                                                                                                                                                       |
| --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Dynamics 365 Remote Assist and Teams**             | Use calling features via the Dynamics 365 Remote Assist app on HoloLens or mobile devices. Features include: </br> - Make a call </br> - Use mixed reality annotations                                             |
| **Microsoft Dataverse**                 | - Access to the Dynamics 365 Remote Assist model-driven app </br> - [Create and manage assets](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/asset-capture-overview) either within or outside a Dynamics 365 Remote Assist call </br> - Create and share one-time call links </br> - See analytics and insights based on your call records |

An Azure Active Directory account is also required for purchasing the Dynamics 365 Remote Assist subscription and for assigning licenses. You'll need an Azure AD account for each licensed user. They'll use this account when signing in to the app. 

>![Note]: The Dynamics 365 Remote Assist, Teams, and Dataverse licenses must be assigned to a native member of the tenant ([Azure AD member](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions#member-and-guest-users) account). Dynamics 365 Remote Assist does not support [Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/what-is-b2b); an individual cannot sign into Dynamics 365 Remote Assist using a Dynamics 365 Remote Assist license assigned to an Azure AD guest account. 

**With the following software, you can leverage even more capabilities.**

| **If you have this…**                                                                                                          | **Additional capabilities accessible through Dynamics 365 Remote Assist:**                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| [OneDrive for Business](https://www.microsoft.com/en-us/microsoft-365/onedrive/compare-onedrive-plans?activetab=tab:primaryr2) | - Share OneDrive files </br> - Send snapshots </br> - Save snapshots to OneDrive                                                                           |
| Dynamics 365 Field Service                                                                                                     | - Call an expert listed in your field service work order </br> - Save call artifacts (for example, call recording, files shared) to a Field Service work order |
| Power BI                                                                                                                       | - View a Power BI dashboard embedded in a Field Service work order                                                                                   |
| Microsoft Stream                 | - [Record Remote Assist calls](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/record-calls-hololens) either from within the Remote Assist app, or from the Teams client |


### Microsoft Teams app user

| **What license does the Teams user have?**                                                                                     | **Capabilities in a Dynamics 365 Remote Assist call include:**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| None                                                                                                                           | - Teams desktop user can join a call using a [one-time call link](one-time-call.md) </br> - Teams desktop user can [join a meeting](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/teams-pc-all#join-a-teams-meeting--with-dynamics-365-remote-assist-hololens-user-only) that allows anonymous participants </br> -  Use mixed reality annotations                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Teams                                                                                                                          | The Teams user’s experience is **_identical_** regardless of whether the Teams user is: </br> - a member in the Dynamics 365 Remote Assist user’s tenant </br> - [a guest](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/multi-tenant-deployment#solution-2-guest-access) in the Dynamics 365 Remote Assist user’s tenant </br> - a member in a tenant that’s [federated](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/multi-tenant-deployment#solution-1-external-access-federation) with the Dynamics 365 Remote Assist user’s tenant (Teams desktop only) </br> **_EXCEPT_** </br> -  any differences described [here](https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access). </br> Additional collaboration capabilities include: </br> -  Make a call </br> - Record a call |
| [OneDrive for Business](https://www.microsoft.com/microsoft-365/onedrive/compare-onedrive-plans?activetab=tab:primaryr2) | - Share OneDrive files </br> - Send snapshots </br> - Save snapshots to OneDrive    |

### Administrator

[Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis) account to assign licenses in Microsoft 365 admin portal and distribute applications through Microsoft Store for Business. Learn more about how to deploy Dynamics 365 Remote Assist [here](https://github.com/docs.microsoft.com/dynamics365/mixed-reality/remote-assist/deploy-remote-assist).

## Network requirements

A variety of network conditions, including bandwidth, latency, jitter, and packet loss, can impact your video calling experience. Although audio and video calls might be possible in environments with reduced bandwidth, you might experience feature degradation.

### Dynamics 365 Remote Assist mobile

When using Dynamics 365 Remote Assist on mobile devices, a minimum of 1.5 Mbps up/down is required for peer-to-peer HD quality video calling with resolution of HD 720p at 15fps.

If Dynamics 365 Remote Assist mobile autodetects that the technician is experiencing [poor network conditions](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/mobile-app/poor-network-connectivity#poor-network-connectivity-is-determined-by-the-following-conditions), it will prompt the technician to share high-quality snapshots instead of transmitting a low-quality live video feed. See [Calls in low bandwidth](mobile-app/poor-network-connectivity.md) for more information.

### Dynamics 365 Remote Assist HoloLens

When using Dynamics 365 Remote Assist on HoloLens, a minimum of 1.5 Mbps up/down is required for peer-to-peer HD quality video calling with resolution of HD 1080p at 30 fps. In general, when more bandwidth is available, quality and usage will increase to deliver the best experience. For **optimal** peer-to-peer HD quality video calling with resolution of HD 1080p, 4-5 Mbps up/down should be expected. However, in some circumstances, even 4-5 Mbps up/down does not guarantee 1080p video calling at full quality. Circumstances include using HoloLens (first gen).

### URLs and ports
The following list contains the *minimum* URL end points and TCP/UDP ports utilized by Dynamics 365 Remote Assist. All must be reachable from the Dynamics 365 Remote Assist client. If you have specialized needs and/or scale, see the [Teams comprehensive list](https://docs.microsoft.com/microsoftteams/prepare-network) for specifics.

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

- [Monitor your network using CQD and call analytics](https://docs.microsoft.com/MicrosoftTeams/prepare-network#best-practice-monitor-your-network-using-cqd-and-call-analytics).
- Review Teams' recommendations [for optimizing your network](https://docs.microsoft.com/MicrosoftTeams/prepare-network#network-optimization).
- Be on a dedicated SSID. The dedicated SSID should be on the 5-Ghz band only; disable 2.4 Ghz.
- Use a router with MU-MIMO capabilities.

### Additional resources

- Learn how to troubleshoot and address internal infrastructure issues using [Teams Call Analytics](https://docs.microsoft.com/MicrosoftTeams/use-call-analytics-to-troubleshoot-poor-call-quality#troubleshoot-call-quality-problems-using-call-analytics) or [Teams Call Quality Dashboard (CQD)](https://docs.microsoft.com/MicrosoftTeams/quality-of-experience-review-guide).

- See [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/prepare-network) to learn more.

## See also

- [Overview of Dynamics 365 Remote Assist](ra-overview.md)
- [Try Dynamics 365 Remote Assist for free](try-remote-assist.md)
- [Buy Dynamics 365 Remote Assist](deploy-remote-assist.md)
- [Using Dynamics 365 Remote Assist on HoloLens](overview-hololens.md)
- [Setup and use Microsoft Teams with Dynamics 365 Remote Assist](teams-pc-all.md)
- [How-to videos](videos.md)



[!INCLUDE[footer-include](../includes/footer-banner.md)]
