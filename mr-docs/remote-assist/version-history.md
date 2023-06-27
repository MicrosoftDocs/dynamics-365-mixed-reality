---
title: Version history for Microsoft Dynamics 365 Remote Assist
author: amaraanigbo
description: Find version history for earlier versions of Microsoft Dynamics Remote Assist, including a list of fixed bugs for each version.
ms.author: soanigbo
ms.date: 10/20/2022
ms.topic: article
ms.reviewer: v-wendysmith
---

# Version history for Dynamics 365 Remote Assist

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

This article provides a version history for Microsoft Dynamics 365 Remote Assist features. For the **most recent wave of features**, see [What's new in Dynamics 365 Remote Assist](whats-new.md). To see a comprehensive list of released and upcoming features, see [Dynamics 365 and Power Platform release plans](/dynamics365/release-plans/), which summarize early access features, preview features, monthly general availability enhancements, and bug fixes.

## 2022 Release Wave 1

## September 21, 2022

### Bugs fixed 

The September 21 release includes the following mobile app bug fixes. 

#### Mobile

- Fixed issue causing call recording video to be cropped when the mobile app is in portrait orientation.
- Fixed crash happening intermittently during authentication failures (iOS only).

The following app versions include the above bug fixes.

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2022.9.21|
|Android mobile app|2022.9.21|

## June 29, 2022

### Features

|Feature|How to|
|-----------------------------------------------|----------------------------------------------------|
|Minimize the Mixed Reality toolbar in Microsoft Teams to focus on the HoloLens video feed|[Collaborate with a Dynamics 365 Remote Assist user through Microsoft Teams desktop for PC or Mac](teams-pc-all.md)|

> [!NOTE]
> You don't need to update the Dynamics 365 Remote Assist HoloLens app or mobile app to be able to minimize the Mixed Reality toolbar from Microsoft Teams.

### Bugs fixed 

The June 29 release also includes the following bug fixes. 

#### HoloLens 2

- Improved the behavior of inking in user interface panels.
- Increased reliability of contact search when searching by full email address.
- Fixed an issue where the **Sign out** button was unexpectedly available when running in Kiosk mode configured for multiple applications on HoloLens 2.
- Addressed a rare issue where the keyboard would disappear when interacting with user interface panels.
- Addressed a rare issue that would cause some chat messages to not be displayed.
- Fixed localized text in several languages to better suit specific scenarios. 

#### Mobile

- Fix for microphone volume being too low during calls on certain Samsung devices.

The following app versions include the above bug fixes.

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|310.2206.15002|
|iOS mobile app|2022.6.29|
|Android mobile app|2022.6.29|

## May 11, 2022

### Features

|Feature|How to|
|-----------------------------------------------|----------------------------------------------------|
|[Support for Microsoft Teams desktop for Mac](/dynamics365-release-plan/2022wave1/remote-assist/dynamics365-remote-assist/support-teams-desktop-mac)|[Collaborate with a Dynamics 365 Remote Assist user through Microsoft Teams desktop for PC or Mac](teams-pc-all.md)|

> [!NOTE]
> You don't need to update the Dynamics 365 Remote Assist HoloLens app or mobile app to take advantage of Microsoft Teams desktop support for Mac.

## April 13, 2022

### Features

|Feature|How to|
|-----------------------------------------------|---------------------------------------------------|
|[Support for screen sharing in the mobile app](/dynamics365-release-plan/2022wave1/remote-assist/dynamics365-remote-assist/support-teams-desktop-mac)|[Share your screen in the mobile app](mobile-app/share-screen.md)|
|[Restrict users from signing out of the HoloLens app](/dynamics365-release-plan/2022wave1/remote-assist/dynamics365-remote-assist/restrict-users-signing-out-hololens-app)|[Restrict users from signing out of the HoloLens app](restricted-mode-signout.md)|
|[Adjust outgoing video quality to reduce HoloLens temperature](/dynamics365-release-plan/2022wave1/remote-assist/dynamics365-remote-assist/adjust-outgoing-video-quality-reduce-hololens-temperature)|[How Dynamics 365 Remote Assist adjusts HoloLens device temperature](hololens-thermal-adjusting.md)|
|[New voice commands for navigating app settings and managing windows](/dynamics365-release-plan/2022wave1/remote-assist/dynamics365-remote-assist/new-voice-commands-navigating-app-settings-window-management)|[Voice commands for Dynamics 365 Remote Assist on HoloLens](voice-commands-hololens.md)|
|[Disable file sharing by using a Microsoft Teams policy](/dynamics365-release-plan/2022wave1/remote-assist/dynamics365-remote-assist/disable-file-sharing-using-teams-policy)|[Microsoft Teams policies supported by Dynamics 365 Remote Assist](teams-policies.md#file-sharing-policies)|
|[Improvement to incoming call notifications on Android](/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/improvement-incoming-call-notifications-android)|[Make calls between Dynamics 365 Remote Assist mobile and Microsoft Teams](mobile-app/remote-assist-mobile-to-teams-calls.md#what-happens-when-dynamics-365-remote-assist-mobile-and-teams-mobile-are-installed-on-the-same-device)|

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|309.2204.06001|
|iOS mobile app|2022.4.6|
|Android mobile app|2022.4.6|

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

## 2021 Release Wave 2

## January 27, 2022

### Features

|Feature|How to|
|-----------------------------------------------|----------------------------------------------------|
|[New restriction capabilities prevent users from making private calls, and accessing files and assets](/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/planned-features)|[Protect company information by restricting capabilities in Dynamics 365 Remote Assist](restricted-mode-overview.md)|

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|308.2201.19002|
|iOS mobile app|2022.2.2|
|Android mobile app|2022.2.2|

### Bugs fixed 

#### HoloLens 2

- Added notification for users having difficulty joining a scheduled meeting. 
- Fixed visual glitches for annotations on certain panels. 
- Fixed issue that prevented text chat and file sharing from working. 
- Improved behavior of pinned panels (they no longer move after the call ends). 

#### Mobile

- Fixed unexpected error when posting to a work order.
- Fixed the "Oops something went wrong" pop-up that was incorrectly triggered when the app launched.
- Fixed blank screen issues that appeared when the app was launched.
- Fixed issue with Intune App Protection scenarios breaking due to missing Mobile Threat Defense (MTD).

## December 14, 2021

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|307.2112.10002|

### Bug fixed

Fixed problem with precision of remote annotations placed close to the HoloLens user. 

## December 10, 2021

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|307.2111.30002|
|iOS mobile app|2021.12.8|
|Android mobile app|2021.12.8|

### Features

|Feature|How to|
|-----------------------------------------------|----------------------------------------------------|
|[Support for spotlight and pinning for video feed on Microsoft Teams desktop](/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/support-spotlight-pinning-remote-assist-video-feed-teams-desktop)|None|

### Bug fixes and improvements

#### HoloLens 2

- Fixed an issue where voice commands would sometimes stop working after connecting to a call.
- Increased reliability and completeness of data logged for Calls Dashboard.
- Call recordings initiated from Dynamics 365 Remote Assist are now saved to SharePoint/OneDrive for 
Business instead of Microsoft Stream for permission management flexibility.
- Addressed cases with text not fitting in UI elements in some languages.
- Improved performance of the UI when launching the app, and ensured clear visual state of the app 
when permission dialogs are presented on the first launch.
- Improved application stability, by addressing various rare crashes.
- Optimizations and fixes for memory leaks.

#### Mobile

- Call recordings initiated from Dynamics 365 Remote Assist are now saved to SharePoint/OneDrive for 
Business instead of Microsoft Stream for permission management flexibility.
- Fix for black screen on some iOS devices.
- Fix for Android app crash when Company Portal is installed.
- Improvements for recent contact presence status.
- Improvements for call notification reliability.
- Increased reliability and completeness of data logged for Calls Dashboard.
- Fix for ‘Unexpected ConfirmButtonPressed’ and ‘Oops something went wrong’ popups showing up 
incorrectly.
- Stability improvements

## October 6, 2021

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|306.2109.24003|
|iOS mobile app|2021.10.6|
|Android mobile app|2021.10.6|

### Features

|Feature|How to|
|-----------------------------------------------|----------------------------------------------------|
|[One-time-call users can open files shared with them from the mobile app](/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/one-time-call-users-open-files-shared-them)|[Invite a user to join a one-time call](one-time-call.md)|
|[Support for a subset of Microsoft Teams policies](/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/support-subset-teams-policies)|[Teams policies supported by Dynamics 365 Remote Assist](teams-policies.md)|
|[Accuracy improvements for mixed-reality annotations on mobile](/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/accuracy-improvements-mixed-reality-annotations-mobile)|None|
|[Support for spotlight and pinning for video feed on Microsoft Teams desktop](/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/support-spotlight-pinning-remote-assist-video-feed-teams-desktop)|None|

### Bugs fixed

#### HoloLens 2

- Fixed issue with holograms disappearing for other participants in the call when holograms are less than 30 cm from the HoloLens user. Collaborators now see what the Dynamics 365 Remote Assist user sees.  

- Improvements to rendering for imported media objects that include transparency. 

- Increased number of contact search results shown to the user. 

- Improvements to audio sounds played on certain actions. 

- Fixed an issue where **Recent** contacts may not appear in rare instances. 

- Addressed incorrect visual state for **Mute** button in rare instances. 

- Fixed notification for incoming chat message that wasn’t visible at times. 

- Fixed sign-in issue for Dynamics 365 Field Service environment (Dynamics 365 Field Service integration).  

#### Mobile 

- Fixed issue with missing recording link in chat.  

- Improved annotations accuracy in snapshot. 

- Fixed video scaling issue in landscape mode. 

- Fixed issue for calls between Dynamics 365 Remote Assist mobile and Dynamics 365 Remote Assist HoloLens devices where users weren’t able to annotate. 

- Fixed issue for video recording on devices that don’t support augmented reality. 

- Fixed issue with unnecessary **Switch view** dialog box on calls between Dynamics 365 Remote Assist clients. 

- Fixed an issue where **Recent** contacts may not appear in rare instances.  

- Intune and authentication SDK updates. 

- Accessibility improvements. 

- Improvement for annotations occlusions on devices supporting LiDAR. 

## 2021 Release Wave 1

### August 9, 2021

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|305.2108.2003.0|
|iOS mobile app|2021.8.4|
|Android mobile app|2021.8.4|

#### Features

|Feature|How to|
|-----------------------------------------------|----------------------------------------------------|
|[Turn hand rays off or on](/dynamics365-release-plan/2021wave1/service/dynamics365-remote-assist/turn-hand-rays-off-or)|[Turn hand rays off or on](hololens-hand-rays.md)|

#### Bugs fixed

##### HoloLens 2

- Fixed an issue causing some of the contacts in the **Recent Contacts** list to disappear upon refresh
- Fixed an issue that sometimes prevented media files from opening on OneDrive
- Improved precision of short ink lines drawn by a Microsoft Teams user in the HoloLens user space
- Improved reliability of text chat (sending and receiving messages) and file sharing
- Improved handling of changes to the call state to increase reliability of calling experiences
- Addressed an issue where transferring the call would sometimes lead to an unexpected visual state
- Addressed rare case where the first photo capture could lead to a crash
- Addressed case where duplicate entries were logged in Calls Dashboard
- Visually polished various panels and improved in-app messaging

##### Mobile

- Fix for last frame being active on the screen in the new call
- Fix for snapshot state after a call was put on hold
- Improvements for saving data in the Calls Dashboard 
- Fix for saving files in the work order in a group call
- Fix for incorrect “Learn more” destination link
- Imrpoved messaging when enabling Dynamics 365 Field Service integration
- General stability improvements
- Fix for missing currently signed-in user’s status in the **Settings** tab
- Fix for not being able to launch the app in some regions
- Fix for accessibility issues

### June 24, 2021

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|304.2106.23002|

#### Bugs fixed

Fix for video freezing in the HoloLens app 

### June 2, 2021

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2 app|304.2105.24005.0|
|iOS mobile app|2021.6.1|
|Android mobile app|2021.6.1|

#### Bug fixes

##### HoloLens 2

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

##### Mobile

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

### May 7, 2021

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2|303.2105.4005|

#### Bug fixes

-	Fix for Calls dashboard to improve logging reliability

### April 29, 2021

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2021.4.3|
|Android mobile app|2021.4.3|

#### Bug fixes

-	Fix for one-time-call sessions – for users who weren't able to take and annotate snapshots during sessions.
-	Fix for Bluetooth headset – Dynamics 365 Remote Assist will now properly use the headset microphone. 


### April 1, 2021

> [!IMPORTANT]
> Dynamics 365 Remote Assist on HoloLens (1st gen) has entered Long Term Servicing state. Future updates for HoloLens (1st gen) will focus on issues and security fixes, while maintaining feature parity with the February 2021 release (version 302.2102.2003).

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2|303.2103.29002|
|iOS mobile app|2021.4.1|
|Android mobile app|2021.4.1|

#### Features

|Feature|How to|
|-----------------------------------------------|----------------------------------------------------|
|Support for low-bandwidth situations|- [HoloLens 2](hololens-low-bandwidth.md)<br><br>- [Mobile app](./mobile-app/low-bandwidth-mode.md)|
|Support for meeting recordings on HoloLens|[Record calls in Dynamics 365 Remote Assist on HoloLens](record-calls-hololens.md)|
|Improvement to the Microsoft Dataverse Environment selection||
|Instinctual interaction improvements on HoloLens 2|[HoloLens voice commands and gestures](voice-commands-hololens.md#gestures)|
|Long Term Servicing for Dynamics 365 Remote Assist on HoloLens (1st gen)||

#### Bug fixes

##### HoloLens 2

- Fixed date format for Calls Dashboard. 
- Addressed an issue where contact presence wasn't displayed in some instances.
- Fixed a problem with setting permissions for a photo shared from HoloLens in a call chat with guest participants.

##### Mobile

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

## 2020 Release Wave 2

### February 2021

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens (1st gen) and 2|302.2102.2003|
|iOS mobile app|2021.2.10|
|Android mobile app|2021.2.10|

#### Bug fixes

##### HoloLens (1st gen) and 2

- Fixed bugs related to file sharing with Teams users.
- Fixed bugs related to voice commands.
- Fixed bugs related to contact searching.
- Improved error handling when selecting Dynamics 365 environment.

##### iOS and Android mobile app

- Fix for video issues on devices with limited GPU support for texture copy, like Samsung Galaxy J4+.
- Fix for removed Dynamics 365 environment selection after app relaunch.
- Fix for missing meetings on user today’s list.
- Fix for annotations being removed when technician navigates to text chat or participants list.
- Fix for annotations toolbar state when a Teams desktop user joins the meeting.
- Improvements for role switching in the one-time call scenario.
- Fix for users not being able to place annotations on iOS after a few minutes in the call.
- Support for contact search with names written in non-Latin scripts, like Arabic, Hebrew, and more.
- Stability improvements.

### January 2021

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens (1st gen) and 2|301.2101.6001|
|iOS mobile app|2021.1.8|
|Android mobile app|2021.01.05|

#### Bug fixes

##### HoloLens (1st gen) and 2

- Important bug fixes and stability improvements.

##### iOS and Android mobile app

- Important bug fixes and stability improvements.

### December 12, 2020

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.12.12|
|Android mobile app|2019.12.09|

#### Bug fixes

##### iOS and Android mobile app

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

### December 2020

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens (1st gen) and 2|301.2012.9002|
|iOS mobile app|2020.12.09|
|Android mobile app|2020.12.09|                                                                                       

#### Bug fixes

##### HoloLens (1st gen) and 2

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

##### iOS and Android mobile app

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

### October 31, 2020

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.10.31|
|Android mobile app|2019.10.22|

#### Bug fixes

##### iOS and Android mobile app

- The Screenshot button is removed from the toolbar. You can edit a screenshot by selecting the Snapshot and annotate button instead.
- If there's a network disconnection, you’re automatically rejoined to the call when the network is restored. If there’s no network connection, the call is ended.
- If you’re using a screen reader and access the tutorial page accessed from the Learn the Tools or Try It button, you can access the Arrow tool.
- If you tap the Try It button on the Sign-in page, and then select the back button on your device, you return to the Sign-in page.
- The end-user license agreement (EULA) link on the Sign-in page goes to the appropriate page (Android or iOS) based on your device.
- On the tutorial page, the buttons now read: Restart Tutorial and Exit Practice.
- If you’re using Dynamics 365 Field Service with Dynamics 365 Remote Assist, the Post to Dynamics 365 pop-up will disappear when you receive or accept a call, but will reappear after the call has ended.
- The “NullReferenceException: Object reference not set to an instance of an object” error message does not appear when starting a call, whether system-generated logs are enabled or not.

### October 2020

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens (1st gen) and 2|300.2010.1002|
|iOS mobile app|2020.10.1|
|Android mobile app|2020.10.03|

#### Bug fixes

##### HoloLens 2

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

##### iOS and Android mobile app

- Improvements to the UI for group calling participants list.
- Improved the view space switching logic for when only one participant is sharing their space in a group call.
- Fix for annotations not being removed after participants leave a group call.
- Fix for call participants in a group call unable to post call content to a Dynamics 365 Field Service work order.
- Fix for getting stuck on loading screen after sign-in.
- Fix for disappearing annotations after saving a snapshot in the call.
- Incoming call notification sound is not present when the device is on silent mode.
- Improved support for Bluetooth headset on iPads and tablets.
- Improved annotations toolbar visibility in Teams clients when in calls with mobile devices without augmented reality (AR) support.

## 2020 Release Wave 1

### September 2020

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens (1st gen) and 2|211.2009.7002.0|
|iOS mobile app|2020.9.1|
|Android mobile app|2020.09.04|

#### Bug fixes

##### HoloLens 2

- Fixed issue with protocol activation when including contact parameter.
- Fixed issue with call recording in GCC High.
- Improved app reliability and stability.

##### iOS and Android mobile app

- Improvements for showing the tracking lost detection and messaging less frequently.
- Adjustments for annotations size being too large on certain device screens.
- Improvements for placing annotations at the correct angle as a remote collaborator in a call between two Dynamics 365 Remote Assist mobile users.
- Fix for application freeze after sign-in.
- Improvements to snapshot UI for when it’s uploading during a call.
- Improvements on ringtone audio for adhering to silent and vibrate modes on Android devices.
- Adjustments for landscape screen orientation when in a call between two Dynamics 365 Remote Assist mobile users.
- Fix for NullReferenceException showing up sometimes during inking and tutorial mode.

### August 2020

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens (1st gen) and 2|211.2007.30002|

#### Bug fixes

##### HoloLens 2

- Fix for the files shared from Microsoft Teams not downloading on HoloLens. 
- Fix for the "Snap" voice command not taking a photo in some cases.
- Fix for when the user answers a call from the shell and it takes them to the contacts screen rather than joining the call. 
- Fix for the Dynamics 365 Remote Assist video card appearing too close after the call has ended. 
- Improved application reliability. 

### July 30, 2020

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.7.30|
|Android mobile app|2020.07.23|

#### Bug fixes

##### iOS and Android mobile app

- Fix for not displaying the Dynamics 365 Remote Assist mobile user's video feed on the Microsoft Teams desktop or mobile user's screen.
- Fix for placing the arrow annotation at the incorrect angle for Microsoft Teams desktop or mobile users.
- Optimized frequency of error messages guiding user to track their environment better.
- Incoming calls improvements. 
- Fix for authentication taking a long time.
- Fix for annotations inaccuracy in calls between two Dynamics 365 Remote Assists clients.
- Fix for Undo and Delete buttons in the incorrect state.
- Fix for memory issues caused by screen rotation.
- Improved application memory usage.

### July 2020

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens (1st gen) and 2|210.2007.1003.0|
|iOS mobile app|2020.7.1|
|Android mobile app|2020.06.27|

#### Bug fixes

##### HoloLens 2

- A Dynamics 365 Remote Assist HoloLens user using GCC High can successfully join a meeting. 
-	Fixed bug in group calls on HoloLens (1st gen) where remote collaborators are unable to annotate from Microsoft Teams client.   
-	Fixed issue with video sharing when a Dynamics 365 Remote Assist HoloLens user rejoins a meeting.
-	Improved experience for using near-field and far-field interactions to manage (for example, resize, move) holographic windows (for example, video card, undocked chat window).
-	Fixed issue regarding CDS instance selection for the Dynamics 365 Remote Assist solution from HoloLens.
-	Addressed an issue where file shared through Teams text chat would sometimes not show up on HoloLens.
-	Fixed positioning of Holographic pop ups (for example, teaching card, prompt to save snapshot to Field Service booking) to appear in front of Dynamics 365 Remote Assist main menu and video card.
-	Voice command fixes to select the snapshot tool and take a snapshot.
-	Fixed issue with the call recording button not toggling as expected in the HoloLens app.
-	Fixed issue around saving and uploading of asset images while viewing asset list.
-	Fixed issue causing incorrect states of the previous/next buttons when navigating between pages on Asset list.
-	Additional miscellaneous bug fixes. 

##### iOS and Android mobile app

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

### June 2020

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2|209.2006.11003.0|

#### Bug fixes

##### HoloLens 2

- Fixed bug in group calls where remote collaborators are unable to annotate from Microsoft Teams client.
- Improvements to the Join Meeting feature to select between overlapping meetings.
- Fixed bug with the snapshot tool causing photos taken with the snapshot tool to not be sent through Teams chat.
- Fixed bug with the snapshot tool where the camera cursor would appear in the resulting photo.
- Various near-field / far-field interaction fixes.
- Fixed bug where the outgoing video feed may not work when answering a call from the HoloLens shell.
- Various fixes to enable users in Egypt to use Dynamics 365 Remote Assist.
- Incoming calls are now supported for GCC High and DOD.

### May 28 2020

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.5.28|
|Android mobile app|2020.05.22|

#### Bug fixes

##### iOS and Android mobile app

- Fix for network error “HTTP 401 TeamsChatService.GetMessagesAsync”.
-	Fix for application not being responsive during launch.
-	Improvement for the recent contacts list.
-	Fix for not being able to find contacts in some countries/regions, such as Egypt.
-	Improvement for the voicemail card.
-	Localization improvements.
-	Accessibility improvements and fixes.

### May 4 2020

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.5.7|
|Android mobile app|2020.05.04|

#### Bug fixes

##### iOS and Android mobile app

- Improved flighting implementation and enabling per company app customizations.
- Fix for sign-in problem for users on mobile networks.
- Improved user feedback questionnaire experience.

### April 2020

#### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens (1st gen) and 2|208.2004.1002.0|
|iOS mobile app|2020.4.1|
|Android mobile app|2002.03.18|

#### Bug fixes

##### HoloLens (1st gen) and 2

- Fixed various speech command bugs.
- Improvements to tool tips.
- Improvements to annotation stability.
- Fixed several application stability-related bugs.
- Various bug fixes for joining Teams meetings.
- Fixes to keyboard interaction and usability.
- Various video quality fixes including support for SimulCast, bandwidth history, & network probing to improve overall video quality.
- Fixed text chat bug that was causing text chats not to show on HoloLens.
- Various near-field / far-field interaction fixes.

##### iOS and Android mobile app

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

### 2019 Release Wave 2

### Feburary 27,  2020

#### Version info

|Device |Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.02.27|
|Android mobile app|2020.02.20|

#### Bug fixes

##### iOS and Android mobile app

- In low-bandwidth environments with a satellite network of 1000/256 kbps for bandwidth, 600/600ms for latency, and 10% of packet loss, users will not receive an 'Update Check Failed' pop-up and can continue to share their environment.  
- Users trying the 90-day license-free Dynamics 365 Remote Assist Mobile trial who don't have a Microsoft Teams license (free or paid) will be prompted to sign up for one. After they sign up, the app will recognize their Microsoft Teams account and they can sign in. 
- With Dynamics 365 Remote Assist mobile app downloaded on your device, users can launch the app from Safari web browser via ```ramobile:/``` deep linking.  
- Users can view their snapshots with annotations on it in both landscape and portrait orientations. These snapshots will save to users’ mobile device’s Photo Gallery.  
- In the text chat, the keyboard remains open after sending a message. 
- The ‘Lost Tracking' pop-up is localized in our supported languages. 
- The correct year is shown when users’ mobile device is set to the future in Thai. 
- Error message improvements.  

## Locate your version number

### HoloLens

To find which version of Dynamics 365 Remote Assist HoloLens you have, go to **Settings**, and then find the version number in the **About** section.

### Mobile app

To find which version of Dynamics 365 Remote Assist mobile you have, go to the menu and select the **Information** option. You'll see the **App Version** there. See the following screenshot for reference.

> [!div class="mx-imgBorder"]
> ![Screenshot of Dynamics 365 Remote Assist on a mobile device, showing the information option and the app version listed.](./media/ram-version-history-locate.png)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
