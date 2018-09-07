---
title: Requirements for setting up Dynamics 365 Remote Assist
---

# Requirements for setting up Dynamics 365 Remote Assist

The following tables list technical requirements for deploying and using
Microsoft Dynamics 365 Remote Assist throughout your organization.

## Device requirements

| **Device**               | **OS requirements**                                                                                                                                                  | **Details**                                                                                                                                                                                                                    |
|--------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| HoloLens                 | Build 10.0.14393.0 or later HoloLens build 10.0.14393.0 is the minimum that supports Remote Assist. We recommend updating HoloLens to newer versions when available. | See [Manage updates to HoloLens](https://docs.microsoft.com/en-us/HoloLens/hololens-updates) for instructions on using Windows Update for Business, Mobile Device Management (MDM), and Windows Server Update Services (WSUS). |
| Windows 10 PC (optional) | Any Windows 10 build                                                                                                                                                 | A Windows 10 PC can collaborate with HoloLens using Microsoft Teams.                                                                                                                                                           |

Licensing and product requirements
----------------------------------

| **Product required**                      | **Details**                                                                                                                                                                                                                                                             | **Learn more**                                                                                                         |
|-------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|
| Remote Assist                             | Remote Assist software                                                                                                                                                                                                                                                  | Buy and deploy Remote Assist                                                                                           |
| Azure Active Directory (AAD) account      | Required for:                                                                                                                                                                                                                                                           | [Get started with Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/get-started-azure-ad) |
| Microsoft Teams                           | Microsoft Teams facilitates communication in Remote Assist. Microsoft Teams must be installed on any device that will make calls to the HoloLens. Note that a free download of Microsoft Teams is available for experts communicating with Remote Assist users.         | [Overview of Microsoft Teams](https://docs.microsoft.com/en-us/MicrosoftTeams/teams-overview)                          |
| Microsoft Office 365                      | Because Microsoft Teams is part of Office 365, the Remote Assist user will need an Office 365 license.                                                                                                                                                                  | [Office 365 licensing for Microsoft Teams](https://docs.microsoft.com/en-us/MicrosoftTeams/office-365-licensing)       |
| Dynamics 365 for Field Service (optional) | Remote Assist requires a Dynamics 365 license if you want to pull Dynamics 365 for Field Service bookings into Remote Assist. To view Power BI dashboards linked to Dynamics 365 for Field Service bookings in Remote Assist, users must have a valid Power BI license. | [Learn more about Dynamics 365 for Field Service](https://dynamics.microsoft.com/en-us/field-service/overview/)        |

-   Purchasing subscription and assigning licenses. You’ll need an AAD account
    for each licensed user.

-   Distributing apps through Microsoft Store for Business.

-   Users when signing in to the app.

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
[Overview of Remote Assist](index.md)
[Buy and deploy](../licensing/buy-and-deploy.md)
[User Guide](user-guide.md)
[Set up and use Microsoft Teams with Remote Assist](use-microsoft-teams-with-remote-assist.md)
[How-to videos](videos.md)
[FAQ](faq.md)
Support