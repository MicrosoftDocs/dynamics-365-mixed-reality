---
title: What's new in Dynamics 365 Remote Assist
author: amaraanigbo
description: Overview of what's new in Dynamics 365 Remote Assist
ms.author: soanigbo
ms.date: 04/20/2022
ms.topic: article
ms.reviewer: v-bholmes
---

# What's new in Dynamics 365 Remote Assist

This article describes details about the **current wave of features (April 2022 through September 2022)** for Dynamics 365 Remote Assist, organized by release date. To see a comprehensive list of released and upcoming features, see [Dynamics 365 and Power Platform release plans](/dynamics365/release-plans/). You can also see a complete list of [features organized by previous waves](version-history.md).

## April 13, 2022

### Features

|Feature|How to|
|-----------------------------------------------|----------------------------------------------------|
|[Support for screen sharing in the mobile app](https://docs.microsoft.com/dynamics365-release-plan/2022wave1/remote-assist/dynamics365-remote-assist/support-screen-sharing-mobile-app)|[Share your screen in the mobile app](mobile-app/share-screen.md)|
|Restrict users from signing out of the HoloLens app|[Restrict users from signing out of the HoloLens app](restricted-mode-signout.md)|
|Adjusting outgoing video on a call to lower HoloLens device temperature |[How Dynamics 365 Remote Assist adjusts HoloLens device temperature](hololens-thermal-adjusting.md)|
|New voice commands for navigating app settings and managing windows|[Voice commands for Dynamics 365 Remote Assist on HoloLens](voice-commands-hololens.md)|
|Use Microsoft Teams policy to turn off ability to send files|[Microsoft Teams policies supported by Dynamics 365 Remote Assist](teams-policies.md#file-sharing-policies)|
|[Improvement to incoming call notifications on Android](https://docs.microsoft.com/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/improvement-incoming-call-notifications-android)|[Make calls between Dynamics 365 Remote Assist mobile and Microsoft Teams](mobile-app/remote-assist-mobile-to-teams-calls.md#what-happens-when-dynamics-365-remote-assist-mobile-and-teams-mobile-are-installed-on-the-same-device)|

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|309.2204.06001|
|iOS mobile app|2022.4.13|
|Android mobile app|2022.4.13|

### Bugs fixed 

#### HoloLens 2

- Added support for three new locales (nb-NO, pt-BR, sv-SE)
- Addressed a problem where the ability to record a call was unavailable, unexpectedly
- Bug fixes and stability improvements

#### Mobile

- Fix for **Camera** button status when joining a meeting 
- Improvement to **Microphone** and **Speaker** buttons status 
- Improvements for annotations accuracy on Android devices
- Fix for the video recording owner displayed in the text chat 
- Fix for the Recent contacts list not always appearing
- Update for the Third-Party Software links in the application 
- User interface improvements for the **More** (ellipsis) menu 

> [!TIP]
> Looking for a list of features from earlier waves? Go to [Version history for Dynamics 365 Remote Assist](version-history.md).

## Locate your version number

### HoloLens

To find which version of Dynamics 365 Remote Assist HoloLens you have, go to **Settings**, and then find the version number in the **About** section.

### Mobile

To find which version of Dynamics 365 Remote Assist mobile you have, go to the menu and select the **Information** option. You'll see the **App Version** there. See the following screenshot for reference.

> [!div class="mx-imgBorder"]
> ![Screenshot of Dynamics 365 Remote Assist on a mobile device, showing the information option and the app version listed.](./media/ram-version-history-locate.png)

## See also

[Version history](version-history.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
