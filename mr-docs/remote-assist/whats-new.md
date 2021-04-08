---
title: What's new in Dynamics 365 Remote Assist
author: BryceHolmes
description: Overview of what's new in Dynamics 365 Remote Assist
ms.author: soanigbo
ms.date: 04/08/2021
ms.service: crm-online
ms.topic: article
ms.reviewer: v-bholmes
---

# What's new in Dynamics 365 Remote Assist

This article describes new features for Dynamics 365 Remote Assist.

For more detailed information about new and upcoming features for Dynamics 365 Remote Assist, see [the Dynamics 365 and Power Platform release plans](https://docs.microsoft.com/dynamics365/release-plans/).

For detailed version histories, see: 

- [Dynamics 365 Remote Assist for HoloLens 1 + 2 version history](version-history-remote-assist-hololens.md)
- [Dynamics 365 Remote Assist mobile app version history](version-history-remote-assist-mobile.md)


## April 1, 2021

> [!IMPORTANT]
> Dynamics 365 Remote Assist on HoloLens 1 has entered Long Term Servicing state. Future updates for HoloLens 1 will focus on issues and security fixes, while maintaining feature parity with the February 2021 release (version 302.2102.2003).

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2|303.2103.29002|
|iOS mobile app|2021.4.1|
|Android mobile app|2021.4.1|

### Features

|Feature|How to|
|-----------------------------------------------|----------------------------------------------------|
|Support for low-bandwidth situations|- [HoloLens 2](hololens-low-bandwidth.md)<br><br>- [Mobile app](./mobile-app/low-bandwidth-mode.md)|
|Support for meeting recordings on HoloLens|[Record calls in Dynamics 365 Remote Assist on HoloLens](record-calls-hololens.md)|
|Improvement to the Microsoft Dataverse Environment selection||
|Instinctual interaction improvements on HoloLens 2|[HoloLens voice commands and gestures](voice-commands-hololens.md#gestures)|
|Long Term Servicing for Dynamics 365 Remote Assist on HoloLens 1||

### Bug fixes

#### HoloLens 2

- Fixed date format for Calls Dashboard. 
- Addressed an issue where contact presence wasn't displayed in some instances.
- Fixed a problem with setting permissions for a photo shared from HoloLens in a call chat with guest participants.

#### iOS and Android mobile app

- Fix for posting to work order files that were shared and not visible when in a call with Dynamics 365 Remote Assist users. 
- Fix for video recording on devices that don't support H.265 HEVC. 
- Fix for deleting annotations placed before the recording was started. 
- Fix for annotations when call is in “on hold” state. 
- Fix for losing annotations for the collaborator when technicians are turning off the camera. 
- Fix for missing video recording link from the meeting. 
- Fix for annotations toolbar being disabled in one-time-call and meetings. 
- Fix for dates not being properly localized in the Calls dashboard. 
- Improvement for text chat availability in calls with poor network connections. 
- Improvement for annotation thickness after annotations are placed in close distance. 
- Fix for unnecessary Dynamics error showing up in the app. 
- Fix for video freezing, end-call availability, and blocked annotations on iOS during a call. 

> [!TIP]
> Looking for earlier features? Go to [version history for Dynamics 365 Remote Assist](version-history.md). 

## Locate your version number

### HoloLens

To find which version of Dynamics 365 Remote Assist HoloLens you have, go to **Settings**, and then find the version number in the **About** section.

### Mobile app

To find which version of Dynamics 365 Remote Assist mobile you have, go to the menu and select the **Information** option. You'll see the **App Version** there. See the following screenshot for reference.

> [!div class="mx-imgBorder"]
> ![Screenshot of Dynamics 365 Remote Assist on a mobile device, showing the information option and the app version listed.](./media/ram-version-history-locate.png)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
