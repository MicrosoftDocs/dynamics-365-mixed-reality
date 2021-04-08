---
title: What's new in Dynamics 365 Remote Assist
author: krbjoran 
description: Overview of what's new in Dynamics 365 Remote Assist
ms.author: krbjoran
ms.date: 04/06/2021
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
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
|Support for recording Teams meetings||
|Improvement to the Microsoft Dataverse Environment selection||
|Instinctual interaction improvements on HoloLens 2||
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





## February 2021

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|302.2102.2003|
|iOS mobile app|2021.2.10|
|Android mobile app|2021.2.10|

### Bug fixes

#### HoloLens 1 and 2

- Fixed bugs related to file sharing with Teams users.
- Fixed bugs related to voice commands.
- Fixed bugs related to contact searching.
- Improved error handling when selecting Dynamics 365 environment.

#### iOS and Android mobile app

- Fix for video issues on devices with limited GPU support for texture copy, like Samsung Galaxy J4+.
- Fix for removed Dynamics 365 environment selection after app relaunch.
- Fix for missing meetings on user today’s list.
- Fix for annotations being removed when technician navigates to text chat or participants list.
- Fix for annotations toolbar state when a Teams desktop user joins the meeting.
- Improvements for role switching in the one-time call scenario.
- Fix for users not being able to place annotations on iOS after a few minutes in the call.
- Support for contact search with names written in non-Latin scripts, like Arabic, Hebrew, and more.
- Stability improvements.





## January 2021

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|301.2101.6001|
|iOS mobile app|2021.1.8|
|Android mobile app|2021.01.05|

### Bug fixes

#### HoloLens 1 and 2

- Important bug fixes and stability improvements.

#### iOS and Android mobile app

- Important bug fixes and stability improvements.





## December 12, 2020

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.12.12|
|Android mobile app|2019.12.09|

### Bug fixes

#### iOS and Android mobile app

- If you don’t have the Company Portal or the Microsoft Authenticator app installed, the app doesn’t crash when you sign in.
- After tapping the Search button when searching for contacts, the “Start type to search text” doesn’t overlap with the recent list of contacts.
- You can sign in with an MSA account.
- The app is localized into 43 languages.
- When you disconnect from a call by closing the app, you’re notified of subsequent calls.
- The app is available in the Apple and Google Play app stores for all supported devices.
- When you take a snapshot for the first time, the snapshot is saved to the camera roll and the video feed doesn’t freeze.
- The Taskbar at the bottom of the screen is now visible on Android 10.
- When you send a message in text chat, the keyboard is automatically closed.
- Calls from Teams desktop to the app are connected and continue with no problems.
- When using Teams on a tablet, annotations are normal size.
- The Speaker button is only visible when there is more than one audio output source.
- All buttons are responsive and can be tapped.
- Fixed app crashes.





## December 2020

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|301.2012.9002|
|iOS mobile app|2020.12.09|
|Android mobile app|2020.12.09|                                                                                       

### Bug fixes

#### HoloLens 1 and 2

- Improvements around selecting Dynamics 365 environment.
- Fixed "Post to Work Order" not working under certain conditions, and sometimes showing the dialog unnecessarily.
- Added voice commands to additional elements on the UI to ensure easy access.
- Addressed visual glitches around window positioning, text flickering and unexpected button highlight.
- Improved reliability of messaging when call recording starts/stops.
- Fixed issue preventing consecutive attempts to call the contact listed in Field Service booking.
- Fixed issue affecting the ability to change the status of a booking.
- Improvements for inking, to ensure that the lines are drawn continuously under all conditions.
- Various visual fixes to unify the look between different windows.
- Fixed issue preventing the access to files shared from Teams in some cases.
- Improved support of file sharing and text chat in Teams channel meetings.

#### iOS and Android mobile app

- Fix for the video not being available in one to one and group calls.
- Fix for “Tracking lost” message. Now it will show only when needed.
- Fix for a call connection coming from Remote Assist on nonAR devices to Remote Assist on AR device.
- Support for annotations made with S pen on Android tablets.
- Fix for guest user search in the contact list.
- Fix for the UI not being responsive with green rectangle only on app launch.
- Fix for picture in picture mode not being available when recording started.
- Fix for “D365 something wrong” generic error that sometimes showed up at the end of the call.
- UI improvements for post to work order scenario, one time call and contacts list.
- Fix for a guest user name displayed in a one time call.





## October 31, 2020

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.10.31|
|Android mobile app|2019.10.22|

### Bug fixes

#### iOS and Android mobile app

- The Screenshot button is removed from the toolbar. You can edit a screenshot by selecting the Snapshot and annotate button instead.
- If there's a network disconnection, you’re automatically rejoined to the call when the network is restored. If there’s no network connection, the call is ended.
- If you’re using a screen reader and access the tutorial page accessed from the Learn the Tools or Try It button, you can access the Arrow tool.
- If you tap the Try It button on the Sign-in page, and then select the back button on your device, you return to the Sign-in page.
- The end-user license agreement (EULA) link on the Sign-in page goes to the appropriate page (Android or iOS) based on your device.
- On the tutorial page, the buttons now read: Restart Tutorial and Exit Practice.
- If you’re using Dynamics 365 Field Service with Dynamics 365 Remote Assist, the Post to Dynamics 365 pop-up will disappear when you receive or accept a call, but will reappear after the call has ended.
- The “NullReferenceException: Object reference not set to an instance of an object” error message does not appear when starting a call, whether system-generated logs are enabled or not.





## October 2020

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|300.2010.1002|
|iOS mobile app|2020.10.1|
|Android mobile app|2020.10.03|

### Bug fixes

#### HoloLens 2

- Improved reliability of voice commands (for photo capture, moving and scaling windows, and more).
- Improved reliability and performance of taking photo captures.
- Improvement for placement of media objects when opening images and documents.
- Improved contact search performance.
- Fixed visual issues with thumbnails when browsing OneDrive files.
- Fixed issue with arrow annotations being placed at incorrect angles under certain conditions.
- Fixed issue where some buttons were difficult to interact with.
- Unified visual styles between tabs (call, files, assets) for various UI elements.
- Call recording is now also available in group calls.
- Camera tool was moved from the toolbar into text chat.

#### iOS and Android mobile app

- Improvements to the UI for group calling participants list.
- Improved the view space switching logic for when only one participant is sharing their space in a group call.
- Fix for annotations not being removed after participants leave a group call.
- Fix for call participants in a group call unable to post call content to a Dynamics 365 Field Service work order.
- Fix for getting stuck on loading screen after sign-in.
- Fix for disappearing annotations after saving a snapshot in the call.
- Incoming call notification sound is not present when the device is on silent mode.
- Improved support for Bluetooth headset on iPads and tablets.
- Improved annotations toolbar visibility in Teams clients when in calls with mobile devices without augmented reality (AR) support.

> [!TIP]
> Looking for earlier features? Go to [version history for Dynamics 365 Remote Assist](version-history.md). 

## Locate your version number

### HoloLens

To find which version of Dynamics 365 Remote Assist HoloLens you have, go to **Settings**, and then find the version number in the **About** section.

### Mobile app

To find which version of Dynamics 365 Remote Assist mobile you have, go to the menu and select the **Information** option. You'll see the **App Version** there. See the following screenshot for reference.

> [!div class="mx-imgBorder"]
> ![Screenshot of Dynamics 365 Remote Assist on a mobile device, showing the information option and the app version listed.](./media/ram-version-history-locate.png)

