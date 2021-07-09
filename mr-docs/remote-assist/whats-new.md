---
title: What's new in Dynamics 365 Remote Assist
author: BryceHolmes
description: Overview of what's new in Dynamics 365 Remote Assist
ms.author: soanigbo
ms.date: 08/04/2021
ms.service: crm-online
ms.topic: article
ms.reviewer: v-bholmes
---

# What's new in Dynamics 365 Remote Assist

This article describes new features for Dynamics 365 Remote Assist.

For more detailed information about new and upcoming features for Dynamics 365 Remote Assist, see [the Dynamics 365 and Power Platform release plans](/dynamics365/release-plans/).

## August 4, 2021

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|XXX|

### Bugs fixed

XXX

## June 24, 2021

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|304.2106.23002|

### Bugs fixed

Fix for video freezing in the HoloLens app 

## June 2, 2021

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|304.2105.24005.0|
|iOS mobile app|2021.6.1|
|Android mobile app|2021.6.1|

### Bug fixes

**Remote Assist Mobile, quality improvements**

- Fix for sharing files when there is a guest user on the call
- Fix for one-time-call link prompting for sign-in due to missing special characters in the url
- Improvements to energy saver mode
- Fix for annotations availability when user rejoins one-time-call
- Fix for misleading “Annotations Unavailable” message in calls with devices without augmented reality support
- Fix for user presence status that was not showing correctly at times
- Support for France digital accessibility requirements
- Fix for annotations after coming back from on hold
- Fix for footer overlap in the post call screen
- Fix for missing recording icon in the participants list
- Fix for screen rotation after leaving Snapshot mode
- Fix for camera and microphone buttons state when connecting to a call
- Fix for duplicated assets in assets capture
- Fix for **Save to chat** button in a one-time-call
- Accessibility and stability improvements

**Remote Assist on Hololens 2, quality improvements**

- Fix for recent contacts sometimes disappearing unexpectedly
- Fix for user not being able to navigate back from contact search in rare cases
- Fix for file sharing issues (receiving files from other call/meeting participants)
- Added voice commands for additional scenarios (saving a photo, navigating through hints)
- Addressed issue causing windows not returning to the correct position after losing and re-gaining tracking
- Fix for pinned state of the main window not staying in the correct position when the call is ended
- Improved handling of menu panels when manipulated by user (grabbed and moved)
- Fix for button states representing the active tool (Arrow, Ink) not always reflecting the current state
- Visual improvements: addressed unexpected panel flickering when user interacted with panel edges; fixed images loaded in 3D space appearing washed out when overlaid on top of other panels
- Various improvements to data logging to make it easier to investigate issues reported by customers 

## May 7, 2021

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2|303.2105.4005|

### Bug fixes

-	Fix for Calls dashboard to improve logging reliability

## April 29, 2021

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2021.4.3|
|Android mobile app|2021.4.3|

### Bug fixes

-	Fix for one-time-call sessions – for users who weren't able to take and annotate snapshots during sessions.
-	Fix for Bluetooth headset – Dynamics 365 Remote Assist will now properly use the headset microphone. 


## April 1, 2021

> [!IMPORTANT]
> Dynamics 365 Remote Assist on HoloLens (1st gen) has entered Long Term Servicing state. Future updates for HoloLens (1st gen) will focus on issues and security fixes, while maintaining feature parity with the February 2021 release (version 302.2102.2003).

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
|Long Term Servicing for Dynamics 365 Remote Assist on HoloLens (1st gen)||

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
