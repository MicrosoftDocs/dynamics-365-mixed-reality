---
author: MatthewJonPaul
description:  Technical requirements for deploying and using Microsoft Dynamics 365 Remote Assist
ms.author: mapau
ms.date: 11/21/2018
ms.service: crm-online
ms.topic: article
title: Requirements for Dynamics 365 Remote Assist
ms.reviewer: v-brycho
---

# Requirements for setting up Dynamics 365 Remote Assist

The following tables list technical requirements for deploying and using
Microsoft Dynamics 365 Remote Assist throughout your organization.

## Device requirements

| **Device**               | **OS requirements**                                                                                                                                                  | **Details**                                                                                                                                                                                                                    |
|--------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| HoloLens                 | Build 10.0.14393.0 or later. HoloLens build 10.0.14393.0 is the minimum that supports Remote Assist. We recommend updating HoloLens to newer versions when available. | See [Manage updates to HoloLens](https://docs.microsoft.com/en-us/HoloLens/hololens-updates) for instructions on using Windows Update for Business, Mobile Device Management (MDM), and Windows Server Update Services (WSUS). |
| Windows 10 PC (optional) | Any Windows 10 build                                                                                                                                                 | A Windows 10 PC can collaborate with HoloLens using Microsoft Teams.                                                                                                                                                           |

Licensing and product requirements
----------------------------------

| **Product required**                      | **Details**                                                                                                                                                                                                                                                             | **Learn more**                                                                                                         |
|-------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|
| Remote Assist                             | Remote Assist software<br></br>**Note** The Remote Assist subscription includes a subscription to Microsoft Teams, which is used by the Remote Assist user.                                                                                                                                                                                                                                                  | [Buy and deploy Remote Assist](../licensing/buy-and-deploy.md)                                                                                           |
| Azure Active Directory (Azure AD) account      | Required for: <ul><li>Purchasing subscription and assigning licenses. You’ll need an AAD account for each licensed user. </li><li>Distributing apps through Microsoft Store for Business. </li><li>Users when signing in to the app. </ul> | [Get started with Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/get-started-azure-ad) |
| Dynamics 365 for Field Service (optional). **Note** that Field Service version 8.2 or later is required. | Remote Assist requires a Dynamics 365 license if you want to view Dynamics 365 for Field Service bookings in Remote Assist. To view Power BI dashboards linked to Dynamics 365 for Field Service bookings in Remote Assist, users must have a valid Power BI license. | [Learn more about Dynamics 365 for Field Service](https://dynamics.microsoft.com/en-us/field-service/overview/)        |



## Network requirements

The recommended bandwidth for optimal performance of Remote Assist is 1.5 MB/s.
Though audio/video calls might be possible in environments with reduced
bandwidth, you might experience HoloLens feature degradation, limiting the user
experience. To test your company’s network bandwidth, follow these steps:

1.  Have a Teams user start a video call with another Teams user.

2.  Add a separate video call between a third and fourth user, and another for a
    fifth and sixth user.

3.  Continue adding video callers to stress-test your network bandwidth until
    you’re confident that multiple users can successfully connect on video calls
    at the same time.

See [Prepare your organization’s network for Microsoft
Teams](https://docs.microsoft.com/en-us/MicrosoftTeams/prepare-network) to learn
more.

### See also
[Overview of Remote Assist](index.md)<br/>
[Try or buy, and deploy](../licensing/buy-and-deploy.md)<br/>
[User Guide](user-guide.md)<br/>
[Set up and use Microsoft Teams with Remote Assist](use-microsoft-teams-with-remote-assist.md)<br/>
[How-to videos](https://go.microsoft.com/fwlink/p/?linkid=2021485)<br/>
[FAQ](faq.md)<br/>
