---
title: Requirements for Dynamics 365 Remote Assist
description:  Technical requirements for deploying and using Microsoft Dynamics 365 Remote Assist
author: prashantyvr
ms.author: prashan
ms.date: 03/04/2025
ms.topic: article
ms.reviewer: v-wendysmith
ms.service: dynamics-365-remote-assist
ms.custom: bap-templates
---

# Requirements for deploying and using Dynamics 365 Remote Assist

[!INCLUDE[try-fs-guides-ra-license](../includes/fs-guides-ra-license.md)]

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

To deploy and use Dynamics 365 Remote Assist on a HoloLens, make sure you meet the following technical requirements.

## Device requirements

Review the supported devices and device requirements for Dynamics 365 Remote Assist.

### Supported devices

The Dynamics 365 Remote Assist application is supported on:

- [HoloLens](/hololens/hololens1-hardware)
- [HoloLens 2](/hololens/hololens2-hardware)

Dynamics 365 Remote Assist on HoloLens or HoloLens 2 must be running 10.0.17134.0 (Windows 10 April 2018) build or later. We recommend [updating](/hololens/hololens-updates) HoloLens to newer versions when available.  [Manage updates to HoloLens](/HoloLens/hololens-updates) to use Windows Update for Business, Mobile Device Management (MDM), and Windows Server Update Services (WSUS).

Individuals without the Dynamics 365 Remote Assist app can join a Dynamics 365 Remote Assist call using the Teams application on a [Windows 10 PC or Mac](teams-pc-all.md), or [mobile device](teams-mobile-all.md).


### Device options and requirements for a Teams user

Dynamics 365 Remote Assist supports new Teams seamlessly. No migration required. Learn more: [New Microsoft Teams app](https://adoption.microsoft.com/en-us/new-microsoft-teams/).

| Device                             | OS requirements                                             | Details                                                                                                                                                                                                                                                                                 |
| ---------------------------------- | ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Teams application on Windows 10 (or later) PC | Any Windows 10 (or later) build.                                       | A Windows 10 (or later) PC running the Teams PC application can collaborate with Dynamics 365 Remote Assist on [supported devices](#supported-devices).                |
| Teams application on Mac|There are no OS requirements|A Macintosh computer running the Teams application can collaborate with a Dynamics 365 Remote Assist user on [supported devices](#supported-devices).|
| Teams application on mobile device | Any iOS or Android phone or tablet running Teams. | A phone or tablet running the Teams mobile application can collaborate with Dynamics 365 Remote Assist on [supported devices](#supported-devices). |

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
| **Dynamics 365 Remote Assist and Teams**             | Use calling features through the Dynamics 365 Remote Assist app on HoloLens or the Microsoft Teams app on mobile devices. Features include: </br> - Make a call </br> - Use mixed-reality annotations                                            |
| **Microsoft Dataverse**                 | - Access to the Dynamics 365 Remote Assist model-driven app </br> - [Create and manage assets](./asset-capture-overview.md) either within or outside a Dynamics 365 Remote Assist call </br> - Create and share one-time call links </br> - See analytics and insights based on your call records |

A Microsoft Entra account is required for assigning licenses. You'll need a Microsoft Entra account for each licensed user. They'll use this account when signing in to the app.

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

> [!Note]
> The Dynamics 365 Remote Assist, Teams, and Dataverse licenses must be assigned to a native member of the tenant ([Microsoft Entra member](/azure/active-directory/fundamentals/users-default-permissions#member-and-guest-users) account). Dynamics 365 Remote Assist does not support [Microsoft Entra B2B](/azure/active-directory/external-identities/what-is-b2b); an individual cannot sign into Dynamics 365 Remote Assist using a Dynamics 365 Remote Assist license assigned to an Microsoft Entra guest account.

**Leverage even more capabilities with the following software:**

| **If you have this service:**                                                                                                          | **You can access these additional capabilities through Dynamics 365 Remote Assist:**                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| [OneDrive](https://www.microsoft.com/en-us/microsoft-365/onedrive/compare-onedrive-plans?activetab=tab:primaryr2) | - Access and share OneDrive files </br> - Send snapshots </br> - Save snapshots to OneDrive </br> - Save photos received through text chat                                                                     |
| [Exchange Online](https://www.microsoft.com/en-us/microsoft-365/business/compare-all-microsoft-365-business-products-b?ef_id=b13c56e0ea01182d16fa364e92f99bec:G:s&OCID=AID2100137_SEM_b13c56e0ea01182d16fa364e92f99bec:G:s&lnkd=Bing_O365SMB_App&msclkid=b13c56e0ea01182d16fa364e92f99bec)| - Receive meeting invites to join meetings from Dynamics 365 Remote Assist<br>- Schedule a one-time call|
| [Dynamics 365 Field Service](https://dynamics.microsoft.com/en-us/field-service/overview/?ef_id=a6382fe92a19180023784f4753c4a638:G:s&OCID=AID2100366_SEM_a6382fe92a19180023784f4753c4a638:G:s&msclkid=a6382fe92a19180023784f4753c4a638)                                                                                                     | - Call an expert listed in a Field Service work order </br> - Save call artifacts (for example, call recording, files shared) to a Field Service work order <br>- Browse a Field Service booking and change the booking status directly from Dynamics 365 Remote Assist while doing the scheduled task |
| Power BI                                                                                                                       | - View a Power BI dashboard embedded in a Field Service work order<br><br>Using the [Calls dashboard in the model-driven app](calls-dashboard.md) doesn't require a Power BI license.                                                                                   |
| [Microsoft Stream](https://www.microsoft.com/en-us/microsoft-365/microsoft-stream)                 | - [Record Remote Assist calls](./record-calls-hololens.md) either from within the Remote Assist app, or from the Teams app |


### Microsoft Teams app user

| **What license does the Teams user have?**                                                                                     | **Capabilities in a Dynamics 365 Remote Assist call:**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| None                                                                                                                           | The Teams PC or Mac user can: </br> - [Join a call](./teams-pc-all.md) </br> - [Join a meeting](./teams-pc-all.md) that allows anonymous participants </br> -  Use mixed-reality annotations                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Teams                                                                                                                          | The Teams user’s experience is **_identical_** regardless of whether the Teams user is: </br> - A member in the Dynamics 365 Remote Assist user’s tenant </br> - [A guest](./multi-tenant-deployment.md#solution-2-guest-access) in the Dynamics 365 Remote Assist user’s tenant </br> - A member in a tenant that’s [federated](./multi-tenant-deployment.md#solution-1-external-access-federation) with the Dynamics 365 Remote Assist user’s tenant (Teams desktop only) </br> **_EXCEPT_** </br> -  Any differences described [here](/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access). </br><br> More collaboration capabilities include: </br> -  Make a call </br> - Record a call |
| [OneDrive](https://www.microsoft.com/microsoft-365/onedrive/compare-onedrive-plans?activetab=tab:primaryr2) | - Share OneDrive files </br> - Send snapshots </br> - Save snapshots to OneDrive    |

### Administrator

[Microsoft Entra](/azure/active-directory/fundamentals/active-directory-whatis) account to assign licenses in Microsoft 365 admin portal and distribute applications through Microsoft Store for Business. [Learn more about how to deploy Dynamics 365 Remote Assist](deploy-remote-assist.md).

## Network requirements

Various network conditions, including bandwidth, latency, jitter, and packet loss, can impact your video calling experience. Although audio and video calls might be possible in environments with reduced bandwidth, you might experience feature degradation.

### Dynamics 365 Remote Assist HoloLens

When using Dynamics 365 Remote Assist on HoloLens:
- A minimum of 1.5 Mbps up/down is required for peer-to-peer HD-quality video calling with resolution of HD 1080p at 30 fps.
- For **optimal** peer-to-peer HD-quality video calling with resolution of HD 1080p, 4-5 Mbps up/down is required. In some circumstances, such as using the first gen HoloLens, even 4-5 Mbps up/down doesn't guarantee 1080p video calling at full quality.

### URLs and ports

Review the *minimum* URL end points and TCP/UDP ports utilized by Dynamics 365 Remote Assist. All must be reachable from the Dynamics 365 Remote Assist app. If you have specialized needs or scale, see the [Teams comprehensive list](/microsoftteams/prepare-network).

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
|Sharepoint/OneDrive|*.sharepoint.com|TCP: 80, 443|
|Windows Notification Service|See [Enterprise Firewall Configurations to Support WNS Traffic](/windows/apps/design/shell/tiles-and-notifications/firewall-allowlist-config)| |
|Connection Test|*.msftconnecttest.com|TCP: 80, 443|

### Network optimization recommendations

Potential optimizations for Dynamics 365 Remote Assist include:

- [Monitor your network using CQD and call analytics](/MicrosoftTeams/prepare-network#best-practice-monitor-your-network-using-cqd-and-call-analytics).
- Review Teams' recommendations [for optimizing your network](/MicrosoftTeams/prepare-network#network-optimization).
- Be on a dedicated SSID. The dedicated SSID should be on the 5-Ghz band only; disable 2.4 Ghz.
- Use a router with MU-MIMO capabilities.

### More resources

- Troubleshoot and address internal infrastructure issues using [Teams Call Analytics](/MicrosoftTeams/use-call-analytics-to-troubleshoot-poor-call-quality#troubleshoot-call-quality-problems-using-call-analytics) or [Teams Call Quality Dashboard (CQD)](/MicrosoftTeams/quality-of-experience-review-guide).
- [Prepare your organization's network for Microsoft Teams](/MicrosoftTeams/prepare-network).

## Next steps

- [Overview of Dynamics 365 Remote Assist](ra-overview.md)
- [Buy Dynamics 365 Remote Assist](deploy-remote-assist.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
