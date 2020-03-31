---
author: sophiasysun
description:  Technical requirements for deploying and using Microsoft Dynamics 365 Remote Assist
ms.author: sopsun
ms.date: 03/31/2020
ms.service: crm-online
ms.topic: article
title: Requirements for Dynamics 365 Remote Assist
ms.reviewer: krbjoran
---

# Technical requirements for deploying and using Microsoft Dynamics 365 Remote Assist

The following tables list technical requirements for deploying and using
[!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] throughout your organization.

## Device requirements for using Remote Assist 

Remote Assist is available on HoloLens 1, HoloLens 2, and AR-capable mobile devices. 

| Device                   | OS                                                                                                                                                                                                        | Details                                                                                                                                                                                                                                                                              |
|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| HoloLens 1 or HoloLens 2 | Build 10.0.14393.0 or later. HoloLens build 10.0.14393.0 is the minimum that supports Remote Assist.                                                                                                      | We recommend updating HoloLens to newer versions when available. See  [Manage updates to HoloLens](https://docs.microsoft.com/HoloLens/hololens-updates) for instructions on using Windows Update for Business, Mobile Device Management (MDM), and Windows Server Update Services (WSUS). |
| Mobile device            | Any [iOS phone or tablet with ARKit enabled](https://www.apple.com/ios/augmented-reality) or [Android phone or tablet with ARCore enabled](https://developers.google.com/ar/discover/supported-devices)  | (Not sure what to put here)                                                                                                                                                                                                                                                                |

## Device requirements for using Microsoft Teams to communicate with Remote Assist users 

To collaborate with a Remote Assist user, you may use Microsoft Teams desktop application ("desktop" or "PC"?) or mobile application. 

| Device         | OS                                                                     | Details                                                                                                                                     |
|----------------|------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|
| Windows 10 PC  | Any Windows 10 device.                                                 | A Windows 10 PC running Microsoft Teams PC app can collaborate with Remote Assist HoloLens or Remote Assist mobile user.                    |
| Mobile device  | Any iOS or Android phone or tablet running Microsoft Teams mobile app. | Any iOS or Android phone or tablet running Microsoft Teams PC app can collaborate with Remote Assist HoloLens or Remote Assist mobile user. |


## Licensing and product requirements

| **Product required**|**Details**|**Learn more**|
|---------------|-------------------------------------------------------|----------------------------------------------------------|
|[!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)]|[!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] software<br></br>**Note** [!include[pn-microsoft-teams](../includes/pn-microsoft-teams.md)] is included in the [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] subscription for individuals using a [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] license on [!include[pn-hololens](../includes/pn-hololens.md)]. A [!include[pn-microsoft-teams](../includes/pn-microsoft-teams.md)] license is also required for individuals (experts) who communicate with a [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] user on [!include[pn-hololens](../includes/pn-hololens.md)]. [!include[pn-teams](../includes/pn-teams.md)] may be available [as a free download](https://teams.microsoft.com/downloads) for these users.| [Buy](buy-remote-assist.md) and [deploy](deploy-remote-assist.md) Dynamics 365 Remote Assist|
|[!include[pn-azure](../includes/pn-azure.md)] Active Directory ([!include[pn-azure](../includes/pn-azure.md)] AD) account|Required for: <ul><li>Purchasing subscription and assigning licenses. You’ll need an [!include[pn-azure](../includes/pn-azure.md)] AD account for each licensed user. </li><li>Distributing apps through [!include[cc-microsoft](../includes/cc-microsoft.md)] Store for Business. </li><li>Users when signing in to the app. </ul> | [Get started with Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/get-started-azure-ad) |
| [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] (optional). **Note** that [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] version 8.2 or later is required. |[!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] requires a [!include[pn-dyn-365](../includes/pn-dyn-365.md)] license if you want to view [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] bookings in [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)]. To view [!include[pn-power-bi](../includes/pn-power-bi.md)] dashboards linked to [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] bookings in [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)], users must have a valid [!include[pn-power-bi](../includes/pn-power-bi.md)] license. | [Learn more about Dynamics 365 Field Service](https://dynamics.microsoft.com/field-service/overview/)|

## Network requirements

The recommended bandwidth for optimal performance of [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] is 1.5 Mbps.
Though audio/video calls might be possible in environments with reduced
bandwidth, you might experience [!include[pn-hololens](../includes/pn-hololens.md)] feature degradation, limiting the user
experience. To test your company’s network bandwidth, follow these steps:

1.  Have a [!include[pn-teams](../includes/pn-teams.md)] user start a video call with another [!include[pn-teams](../includes/pn-teams.md)] user.

2.  Add a separate video call between a third and fourth user, and another for a
    fifth and sixth user.

3.  Continue adding video callers to stress-test your network bandwidth until
    you’re confident that multiple users can successfully connect on video calls
    at the same time.

See [Prepare your organization’s network for Microsoft
Teams](https://docs.microsoft.com/MicrosoftTeams/prepare-network) to learn
more.

### See also
- [Overview of Dynamics 365 Remote Assist](ra-overview.md)
- [Try Dynamics 365 Remote Assist for free](try-remote-assist.md)
- [Buy Dynamics 365 Remote Assist](deploy-remote-assist.md)
- [Using Remote Assist on HoloLens](overview-hololens.md)
- [Set up and use Microsoft Teams with Dynamics 365 Remote Assist](teams-pc-all.md)
- [How-to videos](videos.md)
- [FAQ](faq.md)
