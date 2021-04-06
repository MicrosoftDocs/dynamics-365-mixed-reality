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




## April 2021

The April release includes the following new features.

|Feature|Solution update required?|How to|
|--------------------------------------------------|-----------------------------------------------------|-------------------------------------------------|
|Support for low-bandwidth situations|No|- [HoloLens 2](hololens-low-bandwidth.md)<br><br>- [Mobile app](./mobile-app/low-bandwidth-mode.md)|
|Improvement to the Microsoft Dataverse Environment selection|Yes|- [Calls Dashboard](calls-dashboard.md)<br><br>- [One-time-calls](one-time-call.md)<br><br>- [Asset capture](asset-capture-overview.md)|
|Instinctual interaction improvements on HoloLens 2|No||
|Long Term Servicing for Dynamics 365 Remote Assist on HoloLens 1|No||

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

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2|303.2103.29002|
|iOS mobile app|2021.4.1|
|Android mobile app|2021.4.1|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|





## February 2021

|Feature|Solution update required?|How to|
|--------------------------------------------------|-----------------------------------------------------|-------------------------------------------------|
|XXX|XXX|XXX|
|XXX|XXX|XXX|
|XXX|XXX|XXX|

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

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|302.2102.2003|
|iOS mobile app|2021.2.10|
|Android mobile app|2021.2.10|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|





## January 2021

|Feature|Solution update required?|How to|
|--------------------------------------------------|-----------------------------------------------------|-------------------------------------------------|
|XXX|XXX|XXX|
|XXX|XXX|XXX|
|XXX|XXX|XXX|

### Bug fixes

#### HoloLens 1 and 2

- Important bug fixes and stability improvements.

#### iOS and Android mobile app

- Important bug fixes and stability improvements.

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|301.2101.6001|
|iOS mobile app|2021.1.8|
|Android mobile app|2021.01.05|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|





## December 2020

| Feature                                                                                                                                                                                                                                                                                 | Solution update required? |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| [Contact search keyboard improvements for HoloLens](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/contact-search-keyboard-improvements-hololens)                                                                                        | No                        |
| [Improvement in position accuracy for spatial annotations seen by remote collaborators on Teams](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/improvement-position-accuracy-spatial-annotations-seen-remote-collaborators-teams)       | No                        |
| [Join meetings in the Dynamics 365 Remote Assist mobile app](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/join-meetings-dynamics-365-remote-assist-mobile-app)                                                                         | No                        |
| [Lobby support enabled on HoloLens](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/lobby-support-enabled-hololens)                                                                                                                       | No                        |
| [Support Intune mobile application protection policies SDK for Dynamics 365 Remote Assist mobile app](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/support-intune-mobile-application-protection-policies-sdk-remote-assist-mobile-app) | No                        |
| [Teams live events supported on HoloLens](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/teams-live-events-supported-hololens)                                                                                                           | No                        |
| [Enable customer or vendor to join one-time call](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/enable-customer-or-vendor-join-one-time-call)                                                                                           | No                        |

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

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|301.2012.9002|
|iOS mobile app|2020.12.09|
|Android mobile app|2020.12.09|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|


 
 

## October 2020

| Feature                                                                                                                                                                                                                                                     | Solution update required? |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| [Dynamics 365 Remote Assist calls dashboard](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/remote-assist-calls-dashboard)                                                                                 | No                        |
| [Spatial tracking experience improvements](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/spatial-tracking-experience-improvements)                                                                        | No                        |
| [Updates to the annotation placement algorithm](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/updates-annotation-placement-algorithm)                                                                     | No                        |
| [Use Dynamics 365 Remote Assist on mobile devices without augmented reality support](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/use-remote-assist-mobile-devices-without-augmented-reality-ar-support) | No                        |
| [Automate asset-related processes with Power Automate](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/automate-asset-related-processes-power-automate)                                                     | No                        |
| [Capture and visualize asset information with spatial markup](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/capture-visualize-asset-information-spatial-markup)                                           | No                        |
| [Create and manage organizational asset records](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/create-manage-organizational-asset-records)                                                                | No                        |
| [Prepare your workspace with service-related documentation](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/prepare-workspace-service-related-documentation)                                                | No                        |
| [Enabling calls between Dynamics 365 Remote Assist mobile users](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/enabling-calls-between-remote-assist-mobile-users)                                         | No                        |
| [Improved annotation placement experience](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/improved-annotation-placement-experience)                                                                        | No                        |
| [Make group calls on Dynamics 365 Remote Assist mobile](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/make-group-calls-remote-assist-mobile)                                                              | No                        |

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

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|300.2010.1002|
|iOS mobile app|2020.10.1|
|Android mobile app|2020.10.03|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|



## September 2020

| Feature                                                                                                                                                                                                                                     | Solution update required? |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| | |
| | |
| | |

### Bug fixes

#### HoloLens 2

- Fixed issue with protocol activation when including contact parameter.

- Fixed issue with call recording in GCC High.

- Improved app reliability and stability.

#### iOS and Android mobile app

- Improvements for showing the tracking lost detection and messaging less frequently.

- Adjustments for annotations size being too large on certain device screens.

- Improvements for placing annotations at the correct angle as a remote collaborator in a call between two Dynamics 365 Remote Assist mobile users.

- Fix for application freeze after sign-in.

- Improvements to snapshot UI for when it’s uploading during a call.

- Improvements on ringtone audio for adhering to silent and vibrate modes on Android devices.

- Adjustments for landscape screen orientation when in a call between two Dynamics 365 Remote Assist mobile users.

- Fix for NullReferenceException showing up sometimes during inking and tutorial mode.

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|211.2009.7002.0|
|iOS mobile app|2020.9.1|
|Android mobile app|2020.09.04|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|



## August 2020

| Feature                                                                                                                                                                                                                                     | Solution update required? |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| | |
| | |
| | |

### Bug fixes

#### HoloLens 2

- Fix for the files shared from Microsoft Teams not downloading on HoloLens. 

- Fix for the "Snap" voice command not taking a photo in some cases.

- Fix for when the user answers a call from the shell and it takes them to the contacts screen rather than joining the call. 

- Fix for the Dynamics 365 Remote Assist video card appearing too close after the call has ended. 

- Improved application reliability. 

#### iOS and Android mobile app

- LIST OF MOBILE APP BUGS GOES HERE

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|211.2007.30002|
|iOS mobile app|XXX|
|Android mobile app|XXX|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|




## July 30, 2020

| Feature                                                                                                                                                                                                                                     | Solution update required? |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| | |
| | |
| | |

### Bug fixes

#### iOS and Android mobile app

- Fix for not displaying the Dynamics 365 Remote Assist mobile user's video feed on the Microsoft Teams desktop or mobile user's screen.

- Fix for placing the arrow annotation at the incorrect angle for Microsoft Teams desktop or mobile users.

- Optimized frequency of error messages guiding user to track their environment better.

- Incoming calls improvements. 

- Fix for authentication taking a long time.

- Fix for annotations inaccuracy in calls between two Dynamics 365 Remote Assists clients.

- Fix for Undo and Delete buttons in the incorrect state.

- Fix for memory issues caused by screen rotation.

- Improved application memory usage.

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|210.2007.1003.0|
|iOS mobile app|XXX|
|Android mobile app|XXX|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|





## July 2020

| Feature                                                                                                                                                                                                                                     | Solution update required? |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| | |
| | |
| | |

### Bug fixes

#### HoloLens 2

- A Dynamics 365 Remote Assist HoloLens user using GCC High can successfully join a meeting

-	Fixed bug in group calls on HoloLens 1 where remote collaborators are unable to annotate from Microsoft Teams client 
  
-	Fixed issue with video sharing when a Dynamics 365 Remote Assist HoloLens user rejoins a meeting

-	Improved experience for using near-field and far-field interactions to manage (for example, resize, move) holographic windows (for example, video card, undocked chat window)

-	Fixed issue regarding CDS instance selection for the Dynamics 365 Remote Assist solution from HoloLens

-	Addressed an issue where file shared through Teams text chat would sometimes not show up on HoloLens

-	Fixed positioning of Holographic pop ups (for example, teaching card, prompt to save snapshot to Field Service booking) to appear in front of Dynamics 365 Remote Assist main menu and video card

-	Voice command fixes to select the snapshot tool and take a snapshot

-	Fixed issue with the call recording button not toggling as expected in the HoloLens app

-	Fixed issue around saving and uploading of asset images while viewing asset list

-	Fixed issue causing incorrect states of the previous/next buttons when navigating between pages on Asset list

-	Additional miscellaneous bug fixes 

#### iOS and Android mobile app

- Improved incoming call experience for Dynamics 365 Remote Assist mobile users who do not have the app open when a call comes in from Microsoft Teams desktop or mobile clients.

-	Fix for app crashing on mobile devices without augmented reality (AR) support, especially iPhone 5 and iPhone 6 devices.

-	Dynamics 365 Field Service customers can now view the service account names on the bookings screen. 

-	Updated the User Guide and Dynamics 365 Integration links in the app.

-	Update for authentication library on iOS.

-	Fix for “Just a moment” message blocking users after sign-in.

-	Fix for ArgumentNullException showing up when user doesn't have any recent contacts and search query returns empty list.

-	Fix for Graphics.CopyTexture exception showing after annotating on the snapshot.

-	Fixes for application localization (for example “Retry sign-in” button, “Don’t show again” button and tracking error state messages).

-	Performance improvements for the application memory usage.

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|210.2007.1003.0|
|iOS mobile app|2020.7.1|
|Android mobile app|2020.06.27|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|



## June 2020

| Feature                                                                                                                                                                                                                                     | Solution update required? |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| | |
| | |
| | |

### Bug fixes

#### HoloLens 2

- Fixed bug in group calls where remote collaborators are unable to annotate from Microsoft Teams client

- Improvements to the Join Meeting feature to select between overlapping meetings

- Fixed bug with the snapshot tool causing photos taken with the snapshot tool to not be sent through Teams chat

- Fixed bug with the snapshot tool where the camera cursor would appear in the resulting photo

- Various near-field / far-field interaction fixes

- Fixed bug where the outgoing video feed may not work when answering a call from the HoloLens shell

- Various fixes to enable users in Egypt to use Dynamics 365 Remote Assist

- Incoming calls are now supported for GCC High and DOD

#### iOS and Android mobile app

- LIST OF MOBILE APP BUGS GOES HERE

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2|209.2006.11003.0|
|iOS mobile app|XXX|
|Android mobile app|XXX|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|





## May 28 2020

| Feature                                                                                                                                                                                                                                     | Solution update required? |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| | |
| | |
| | |

### Bug fixes

#### iOS and Android mobile app

- Fix for network error “HTTP 401 TeamsChatService.GetMessagesAsync”.

-	Fix for application not being responsive during launch.

-	Improvement for the recent contacts list.

-	Fix for not being able to find contacts in some countries, such as Egypt.

-	Improvement for the voicemail card.

-	Localization improvements.

-	Accessibility improvements and fixes.

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2|209.2006.11003.0|
|iOS mobile app|2020.5.28|
|Android mobile app|2020.05.22|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|




## May 4 2020

| Feature                                                                                                                                                                                                                                     | Solution update required? |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| | |
| | |
| | |

### Bug fixes

#### iOS and Android mobile app

- Improved flighting implementation and enabling per company app customizations.

- Fix for sign-in problem for users on mobile networks.

- Improved user feedback questionnaire experience.

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.5.7|
|Android mobile app|2020.05.04|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|




## April 2020

| Feature                                                                                                                                                                                                                                     | Solution update required? |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| [Capture asset condition through spatial markup](https://docs.microsoft.com/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-remote-assist/capture-asset-condition-through-spatial-markup)                                      | No                        |
| [Capture session history through call recordings](https://docs.microsoft.com/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-remote-assist/capture-session-history-through-call-recordings)                                    | No                        |
| [Share files between technicians and experts to improve collaboration](https://docs.microsoft.com/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-remote-assist/share-files-between-technicians-experts-improve-collaboration) | No                        |

### Bug fixes

#### HoloLens 1 and 2

- Fixed various speech command bugs

- Improvements to tool tips

- Improvements to annotation stability

- Fixed several application stability-related bugs

- Various bug fixes for joining Teams meetings

- Fixes to keyboard interaction and usability

- Various video quality fixes including support for SimulCast, bandwidth history, & network probing to improve overall video quality

- Fixed text chat bug that was causing text chats not to show on HoloLens

- Various near-field / far-field interaction fixes

#### iOS and Android mobile app

- Fix for yellow tracking dots. Yellow tracking dots will not show up on the mobile device screen.

- Improved quality of annotations placement in the near field of 1 meter (three feet).

- Improved loading for cached recent contacts when users are in poor network condition. 

- Improved authentication handling and messaging. Better support for offline scenario and better error description.

- Fixed incorrect annotations position on tablet devices. Annotations were shifted on the sides of the screen.

- Enabled saving a snapshot if a call ends unexpectedly.

- Fixed incoming video feed position on the screen.

- Improved messaging and handling when group call is detected.

- Fixed NullReferenceException showing up during app termination and in the contacts search page.

- Fix for ArgumentOutOfRange exception showing up when typing text in the text chat.

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|208.2004.1002.0|
|iOS mobile app|2020.4.1|
|Android mobile app|2002.03.18|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|





## Feburary 27,  2020

| Feature                                                                                                                                                                                                                                     | Solution update required? |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| | |
| | |
| | |

### Bug fixes

#### iOS and Android mobile app

- In low-bandwidth environments with a satellite network of 1000/256 kbps for bandwidth, 600/600ms for latency, and 10% of packet loss, users will not receive an 'Update Check Failed' pop-up and can continue to share their environment.  

- Users trying the 90-day license-free Dynamics 365 Remote Assist Mobile trial who don't have a Microsoft Teams license (free or paid) will be prompted to sign up for one. After they sign up, the app will recognize their Microsoft Teams account and they can sign in.  

- With Dynamics 365 Remote Assist mobile app downloaded on your device, users can launch the app from Safari web browser via ```ramobile:/``` deep linking. 
 
- Users can view their snapshots with annotations on it in both landscape and portrait orientations. These snapshots will save to users’ mobile device’s Photo Gallery.  

- In the text chat, the keyboard remains open after sending a message. 

- The ‘Lost Tracking' pop-up is localized in our supported languages. 

- The correct year is shown when users’ mobile device is set to the future in Thai. 

- Error message improvements.  

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.02.27|
|Android mobile app|2020.02.20|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|





# December 12, 2020

| Feature                                                                                                                                                                                                                                     | Solution update required? |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| | |
| | |
| | |

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

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.12.12|
|Android mobile app|2019.12.09|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|



# October 31, 2020

| Feature                                                                                                                                                                                                                                     | Solution update required? |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| | |
| | |
| | |

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

### Version info

|Device or software|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.10.31|
|Android mobile app|2019.10.22|
|Microsoft Dataverse solution|XXX|
|Teams|XXX|



## Locate your version number

### HoloLens

To find which version of Dynamics 365 Remote Assist HoloLens you have, go to **Settings**, and then find the version number in the **About** section.

### Mobile app

To find which version of Dynamics 365 Remote Assist mobile you have, go to the menu and select the **Information** option. You'll see the **App Version** there. See the following screenshot for reference.

> [!div class="mx-imgBorder"]
> ![Screenshot of Dynamics 365 Remote Assist on a mobile device, showing the information option and the app version listed.](./media/ram-version-history-locate.png)

