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

The following tables list technical requirements for deploying and using Microsoft Dynamics 365 Remote Assist throughout your organization. 

## Device requirements 

A Remote Assist call is between a Remote Assist user and a Microsoft Teams user. 
Remote Assist is available on HoloLens, HoloLens 2, and qualifying Android or iOS mobile devices
To collaborate with a Remote Assist user, a Microsoft Teams user may only use the Teams application on Windows 10 PC or mobile devices.
                                                                                                                       |

### Device options and requirements for a Remote Assist user 

| Device                                   | OS requirements                                                                                                                                                                                                          | Details                                                                                                                                                                                                                  |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Remote Assist on HoloLens  or HoloLens 2 | HoloLens or HoloLens 2 running 10.0.17134.0 (i.e., Windows 10 April 2018) build or later. We recommend [updating](https://docs.microsoft.com/en-us/hololens/hololens-updates) HoloLens to newer versions when available. | See [Manage updates to HoloLens](https://docs.microsoft.com/HoloLens/hololens-updates) for instructions on using Windows Update for Business, Mobile Device Management (MDM), and Windows Server Update Services (WSUS). |
| Remote Assist on mobile devices          | Dynamics 365 Remote Assist mobile is available on Android devices with ARCore-enabled devices and iOS devices with ARKit-enabled devices.                                                                                | These are the lists of AR-supported devices on [Android](https://developers.google.com/ar/discover/supported-devices) and [iOS](https://www.apple.com/ios/augmented-reality/).                                           |


### Device options and requirements for a remote collaborator using Teams 

| Device                             | OS requirements                                             | Details                                                                                                                                                                                                                                                                                 |
| ---------------------------------- | ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Teams application on Windows 10 PC | Any Windows 10 build.                                       | A Windows 10 PC running the Teams PC application can collaborate with Remote Assist on HoloLens, HoloLens 2, or qualifying [Android](https://developers.google.com/ar/discover/supported-devices) or [iOS](https://www.apple.com/ios/augmented-reality/) mobile devices.                |
| Teams application on mobile device | Any iOS or Android phone or tablet running Microsoft Teams. | A phone or tablet running the Microsoft Teams Mobile application can collaborate with Remote Assist on HoloLens, HoloLens 2, or qualifying [Android](https://developers.google.com/ar/discover/supported-devices) or [iOS](https://www.apple.com/ios/augmented-reality/) mobile devices |



##  Licensing and product requirements per role

| Role                                       | Software needed                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Administrator                              | *   [Azure Active Directory (AAD)](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/active-directory-whatis) account to assign licenses in M365 Admin portal and distribute apps through Microsoft Store for Business. Learn more about how to deploy Remote Assist \[here\]([https://docs.microsoft.com/en-us/dynamics365/mixed-reality/remote-assist/deploy-remote-assist](https://docs.microsoft.com/en-us/dynamics365/mixed-reality/remote-assist/deploy-remote-assist)).                                                                                                                                                                                                                                                                                                                                                |
| Dynamics 365 Remote Assist user            | *   [Azure Active Directory (AAD)](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/active-directory-whatis) account
*   Teams license (included with Remote Assist license)
*   Remote Assist license
*   Remote Assist app on HoloLens, HoloLens 2, or qualifying [Android](https://developers.google.com/ar/discover/supported-devices)or [iOS](https://www.apple.com/ios/augmented-reality/) device
*   (Optional) Dynamics 365 Field Service license\*
*   (Optional) PowerBI license\*\*                                                                                                                                                                                                                                                                                                                               |
| Remote collaborator (Uses Microsoft Teams) | Teams requirements to communicate with a Remote Assist user:

*   Teams license 
*   Teams mobile app or the Windows 10 Teams PC application

Note: It is possible to use Teams to communicate with a Remote Assist user without acquiring a Teams license. Teams supports [guest access](https://docs.microsoft.com/en-us/MicrosoftTeams/guest-access), which lets an organization add individual users from outside their organization into their teams and channels. Anyone with a business or consumer email account, such as Outlook, Gmail, or others, can use Teams as a guest in another organization's tenant. 

Note: The remote collaborator can use Teams for free, which offers [limited functionality](https://docs.microsoft.com/en-us/microsoftteams/upgrade-freemium#how-does-teams-free-compare-to-the-full-version-of-teams). |



* *To use Remote Assist to view Dynamics 365 Field Service bookings, users will need both a Remote Assist and Field Service license version 8.2 or later. [Learn more about Dynamics 365 Field Service](https://dynamics.microsoft.com/en-us/field-service/overview/).
* **To use Remote Assist to open Power BI dashboards linked to Dynamics 365 Field Service bookings, users must have a valid PowerBI license. [Learn more about PowerBI.](https://powerbi.microsoft.com/en-us/)

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
