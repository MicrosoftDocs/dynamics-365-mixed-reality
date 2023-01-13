---
author: amaraanigbo
description:  Technical requirements for deploying and using Microsoft Dynamics 365 Remote Assist
ms.author: soanigbo
ms.date: 10/14/2022
ms.topic: conceptual
title: Requirements for Dynamics 365 Remote Assist
ms.reviewer: v-wendysmith
ms.service: dynamics-365-remote-assist
ms.custom: bap-templates
---

# Technical requirements for deploying and using Dynamics 365 Remote Assist

Review the supported devices and device requirements for Dynamics 365 Remote Assist.

## Device requirements

### Supported devices

The Dynamics 365 Remote Assist application is supported on:
- [HoloLens](./hololens/hololens1-hardware.md)
- [HoloLens 2](./hololens/hololens2-hardware)
- Qualifying [Android](https://developers.google.com/ar/discover/supported-devices) mobile phones or tablets
- Qualifying [iOS](https://www.apple.com/ios/augmented-reality/) mobile phones and tablets

Individuals without the Dynamics 365 Remote Assist app can join a [Dynamics 365 Remote Assist call](./mobile-app/making-calls-on-remote-assist-mobile.md) using the Teams application on a [Windows 10 PC](teams-pc-all.md), Mac, or qualifying [mobile device](teams-mobile-all.md).

> [!NOTE]
> Accuracy of annotations is highly dependent on the capabilities of the device. Use Android devices that have a time-of-flight (ToF) sensor and support the [Depth API](https://developers.google.com/ar/discover/supported-devices) and iOS devices that have a LiDAR sensor [(see LiDAR sensor in the tables listed for iOS and iPadOS devices)](https://en.wikipedia.org/wiki/List_of_iOS_and_iPadOS_devices) for a better augmented reality (AR) experience.

### Device options and requirements for a Dynamics 365 Remote Assist user

| Device                                   | OS requirements                                                                                                                                                                                                          | Details                                                                                                                                                                                                                  |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Dynamics 365 Remote Assist on HoloLens or HoloLens 2 | HoloLens or HoloLens 2 running 10.0.17134.0 (Windows 10 April 2018) build or later. We recommend [updating](/hololens/hololens-updates) HoloLens to newer versions when available. | See [Manage updates to HoloLens](/HoloLens/hololens-updates) to use Windows Update for Business, Mobile Device Management (MDM), and Windows Server Update Services (WSUS). |
| Dynamics 365 Remote Assist on mobile devices          | Dynamics 365 Remote Assist mobile is available on all devices, including ARCore-enabled Android phones or tablets, ARKit-enabled iOS iPhones or iPads, and mobile devices without AR support. <p><p>**For Android devices, the minimum operating system required is Android 7.0. For iOS devices, the minimum operating system required is iOS 12.2.**                                                                              | See [Android AR-supported devices](https://developers.google.com/ar/discover/supported-devices), [iOS ARCore-supported devices](https://developers.google.com/ar/discover/supported-devices#ios), or [Dynamics 365 Remote Assist mobile calls on mobile devices without AR support](./mobile-app/calls-using-devices-without-ar.md).                                         |
  
> [!IMPORTANT]
> When you use Dynamics 365 Remote Assist on a non-Windows device, the operating system of the device processes some personal data to enable push and incoming call notifications. Microsoft may, accordingly, send data to the external, third-party notification services so users can see who is calling or be notified of a chat message. Google Firebase Cloud Messaging (FCM) and Apple Push Notification services are not provisioned in a dedicated data center for exclusive use by you and are governed by their own service-specific terms and privacy statements, which you should carefully review.

### Device options and requirements for a Teams user

| Device                             | OS requirements                                             | Details                                                                                                                                                                                                                                                                                 |
| ---------------------------------- | ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Teams application on Windows 10 (or later) PC | Any Windows 10 (or later) build.                                       | A Windows 10 (or later) PC running the Teams PC application can collaborate with Dynamics 365 Remote Assist on [supported devices](#supported-devices).                |
| Teams application on Mac|There are no OS requirements|A Macintosh computer running the Teams application can collaborate with a Dynamics 365 Remote Assist user on [supported devices](#supported-devices).|
| Teams application on mobile device | Any iOS or Android phone or tablet running  Teams. | A phone or tablet running the Teams mobile application can collaborate with Dynamics 365 Remote Assist on [supported devices](#supported-devices). |

> [!Note] 
> Dynamics 365 Remote Assist may not be available in your country. For more information, see [Dynamics 365 Remote Assist mobile availability](./mobile-app/faq-mobile.md).

## Licensing and product requirements per role

Review the licensing and product requirements by user role.

### Dynamics 365 Remote Assist app user

A Dynamics 365 Remote Assist license includes the following three products:

- Dynamics 365 Remote Assist
- Microsoft Teams
- Microsoft Dataverse

> [!NOTE]
> Dynamics 365 Remote Assist [supports a subset of Microsoft Teams policies](teams-policies.md).

| **Included with Dynamics 365 Remote Assist license** | **What capabilities are available?**                                                                                                                                                                                                                                                                                                       |
| --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Dynamics 365 Remote Assist and Teams**             | Use calling features through the Dynamics 365 Remote Assist app on HoloLens or mobile devices. Features include: </br> - Make a call </br> - Use mixed-reality annotations                                            |
| **Microsoft Dataverse**                 | - Access to the Dynamics 365 Remote Assist model-driven app </br> - [Create and manage assets](./asset-capture-overview.md) either within or outside a Dynamics 365 Remote Assist call </br> - Create and share one-time call links </br> - See analytics and insights based on your call records |

An Azure Active Directory account is also required for purchasing the Dynamics 365 Remote Assist subscription and for assigning licenses. You'll need an Azure AD account for each licensed user. They'll use this account when signing in to the app.

> [!Note]
> The Dynamics 365 Remote Assist, Teams, and Dataverse licenses must be assigned to a native member of the tenant ([Azure AD member](/azure/active-directory/fundamentals/users-default-permissions#member-and-guest-users) account). Dynamics 365 Remote Assist does not support [Azure AD B2B](/azure/active-directory/external-identities/what-is-b2b); an individual cannot sign into Dynamics 365 Remote Assist using a Dynamics 365 Remote Assist license assigned to an Azure AD guest account.

**Leverage even more capabilities with the following software:**

| **If you have this service:**                                                                                                          | **You can access these additional capabilities through Dynamics 365 Remote Assist:**                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| [OneDrive for Business](https://www.microsoft.com/en-us/microsoft-365/onedrive/compare-onedrive-plans?activetab=tab:primaryr2) | - Access and share OneDrive files </br> - Send snapshots </br> - Save snapshots to OneDrive </br> - Save photos received through text chat                                                                     |
| [Exchange Online](https://www.microsoft.com/en-us/microsoft-365/business/compare-all-microsoft-365-business-products-b?ef_id=b13c56e0ea01182d16fa364e92f99bec:G:s&OCID=AID2100137_SEM_b13c56e0ea01182d16fa364e92f99bec:G:s&lnkd=Bing_O365SMB_App&msclkid=b13c56e0ea01182d16fa364e92f99bec)| - Receive meeting invites to join meetings from Dynamics 365 Remote Assist<br>- Schedule a one-time call|
| [Dynamics 365 Field Service](https://dynamics.microsoft.com/en-us/field-service/overview/?ef_id=a6382fe92a19180023784f4753c4a638:G:s&OCID=AID2100366_SEM_a6382fe92a19180023784f4753c4a638:G:s&msclkid=a6382fe92a19180023784f4753c4a638)                                                                                                     | - Call an expert listed in a Field Service work order </br> - Save call artifacts (for example, call recording, files shared) to a Field Service work order <br>- Browse a Field Service booking and change the booking status directly from Dynamics 365 Remote Assist while doing the scheduled task |
| [Power BI](https://www.microsoft.com/en-us/resilience/business-insights-analytics-solutions?ef_id=b8a24caec6781d220ebc2c00bc6856aa:G:s&OCID=AID2100615_SEM_b8a24caec6781d220ebc2c00bc6856aa:G:s&msclkid=b8a24caec6781d220ebc2c00bc6856aa)                                                                                                                       | - View a Power BI dashboard embedded in a Field Service work order<br><br>Using the [Calls dashboard in the model-driven app](one-time-call.md) does not require a Power BI license.                                                                                   |
| [Microsoft Stream](https://www.microsoft.com/en-us/microsoft-365/microsoft-stream)                 | - [Record Remote Assist calls](./record-calls-hololens.md) either from within the Remote Assist app, or from the Teams app |


### Microsoft Teams app user

| **What license does the Teams user have?**                                                                                     | **Capabilities in a Dynamics 365 Remote Assist call:**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| None                                                                                                                           | The Teams PC or Mac user can: </br> - Join a call using a [one-time call link](one-time-call.md) </br> - [Join a meeting](./teams-pc-all.md) that allows anonymous participants </br> -  Use mixed-reality annotations                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Teams                                                                                                                          | The Teams user’s experience is **_identical_** regardless of whether the Teams user is: </br> - A member in the Dynamics 365 Remote Assist user’s tenant </br> - [A guest](./multi-tenant-deployment.md#solution-2-guest-access) in the Dynamics 365 Remote Assist user’s tenant </br> - A member in a tenant that’s [federated](./multi-tenant-deployment.md#solution-1-external-access-federation) with the Dynamics 365 Remote Assist user’s tenant (Teams desktop only) </br> **_EXCEPT_** </br> -  Any differences described [here](/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access). </br><br> Additional collaboration capabilities include: </br> -  Make a call </br> - Record a call |
| [OneDrive for Business](https://www.microsoft.com/microsoft-365/onedrive/compare-onedrive-plans?activetab=tab:primaryr2) | - Share OneDrive files </br> - Send snapshots </br> - Save snapshots to OneDrive    |

### Administrator

[Azure Active Directory (Azure AD)](/azure/active-directory/fundamentals/active-directory-whatis) account to assign licenses in Microsoft 365 admin portal and distribute applications through Microsoft Store for Business. [Learn more about how to deploy Dynamics 365 Remote Assist](deploy-remote-assist.md).

## Network requirements

A variety of network conditions, including bandwidth, latency, jitter, and packet loss, can impact your video calling experience. Although audio and video calls might be possible in environments with reduced bandwidth, you might experience feature degradation.

### Dynamics 365 Remote Assist mobile

When using Dynamics 365 Remote Assist on mobile devices:
- A minimum of 1.5 Mbps up/down is required for peer-to-peer HD quality video calling with resolution of HD 720p at 15fps.

If Dynamics 365 Remote Assist mobile autodetects that the technician is experiencing [poor network conditions](./mobile-app/poor-network-connectivity.md#poor-network-connectivity-is-determined-by-the-following-conditions), it will prompt the technician to share high-quality snapshots instead of transmitting a low-quality live video feed. See [Calls in low bandwidth](mobile-app/poor-network-connectivity.md) for more information.

### Dynamics 365 Remote Assist HoloLens

When using Dynamics 365 Remote Assist on HoloLens:
- A minimum of 1.5 Mbps up/down is required for peer-to-peer HD-quality video calling with resolution of HD 1080p at 30 fps.
- For **optimal** peer-to-peer HD-quality video calling with resolution of HD 1080p, 4-5 Mbps up/down is required. In some circumstances, such as using the first gen HoloLens, even 4-5 Mbps up/down does not guarantee 1080p video calling at full quality.

### URLs and ports

Review the *minimum* URL end points and TCP/UDP ports utilized by Dynamics 365 Remote Assist. All must be reachable from the Dynamics 365 Remote Assist app. If you have specialized needs and/or scale, see the [Teams comprehensive list](/microsoftteams/prepare-network).

> [!NOTE]
> US Government Community Cloud (GCC) environments require additional URLs to be added to the allowlist. For more information, see the following topics:
> - [Office 365 U.S. Government GCC High endpoints](/microsoft-365/enterprise/microsoft-365-u-s-government-gcc-high-endpoints)
> - [Dynamics 365 US Government](/power-platform/admin/microsoft-dynamics-365-government)
> - [Power Apps US Government](/power-platform/admin/powerapps-us-government)  

|Service/App|Minimum URL endpoints|TCP/UDP ports|
|----------|-----------|------------|
|Teams|- *.registrar.skype.com </br> - *.teams.microsoft.com|UDP: 3478, 3479, 3480, 3481|
|Authentication|- login.microsoft.com </br> - login.microsoftonline.com </br> - login.live.com </br> - sts.windows.net|TCP: 80, 443|
|Microsoft Graph|graph.microsoft.com|TCP: 80, 443|
|Enterprise Configuration Service|ecs.office.com|TCP: 80, 443|
|Dynamics Services|*.crm.dynamics.com|TCP: 80, 443|
|Sharepoint / OneDrive|*.sharepoint.com|TCP: 80, 443|
|Windows Notification Service|See [Enterprise Firewall Configurations to Support WNS Traffic](/windows/apps/design/shell/tiles-and-notifications/firewall-allowlist-config)| |
|Connection Test|*.msftconnecttest.com|TCP: 80, 443|

### Network optimization recommendations

Potential optimizations for Dynamics 365 Remote Assist include:

- [Monitor your network using CQD and call analytics](/MicrosoftTeams/prepare-network#best-practice-monitor-your-network-using-cqd-and-call-analytics).
- Review Teams' recommendations [for optimizing your network](/MicrosoftTeams/prepare-network#network-optimization).
- Be on a dedicated SSID. The dedicated SSID should be on the 5-Ghz band only; disable 2.4 Ghz.
- Use a router with MU-MIMO capabilities.

### Additional resources

- Troubleshoot and address internal infrastructure issues using [Teams Call Analytics](/MicrosoftTeams/use-call-analytics-to-troubleshoot-poor-call-quality#troubleshoot-call-quality-problems-using-call-analytics) or [Teams Call Quality Dashboard (CQD)](/MicrosoftTeams/quality-of-experience-review-guide).
- [Prepare your organization's network for Microsoft Teams](/MicrosoftTeams/prepare-network).

## Next steps

- [Overview of Dynamics 365 Remote Assist](ra-overview.md)
- [Try Dynamics 365 Remote Assist for free](try-remote-assist.md)
- [Buy Dynamics 365 Remote Assist](deploy-remote-assist.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
