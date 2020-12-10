---
title: "Dynamics 365 Remote Assist mobile version history | MicrosoftDocs"
description: Version history for Dynamics 365 Remote Assist mobile
ms.custom: 
  - dyn365-mixed-reality-remote-assist
ms.date: 12/10/2020
ms.reviewer: krbjoran
ms.topic: article
ms.service: crm-online
applies_to: 
  - "Dynamics 365 (online)"
  - "Dynamics 365 Version 9.x"
author: FieldServiceDave
ms.author: daclar
manager: shellyha
search.app: 
  - MRRA
  - MRRA
---

# Dynamics 365 Remote Assist mobile version history

## iOS - 2020.12.09 + Android - 2020.12.00

Date: December, 2020

### Bug fixes

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

## iOS - 2020.10.1 + Android - 2020.10.03

Date: October 1, 2020

### Bug fixes

- Improvements to the UI for group calling participants list.
- Improved the view space switching logic for when only one participant is sharing their space in a group call.
- Fix for annotations not being removed after participants leave a group call.
- Fix for call participants in a group call unable to post call content to a Dynamics 365 Field Service work order.
- Fix for getting stuck on loading screen after sign-in.
- Fix for disappearing annotations after saving a snapshot in the call.
- Incoming call notification sound is not present when the device is on silent mode.
- Improved support for Bluetooth headset on iPads and tablets.
- Improved annotations toolbar visibility in Teams clients when in calls with mobile devices without augmented reality (AR) support.

## iOS - 2020.9.1 + Android - 2020.09.04

Date: September 1, 2020

### Bug fixes

- Improvements for showing the tracking lost detection and messaging less frequently.
- Adjustments for annotations size being too large on certain device screens.
- Improvements for placing annotations at the correct angle as a remote collaborator in a call between two Dynamics 365 Remote Assist mobile users.
- Fix for application freeze after sign-in.
- Improvements to snapshot UI for when it’s uploading during a call.
- Improvements on ringtone audio for adhering to silent and vibrate modes on Android devices.
- Adjustments for landscape screen orientation when in a call between two Dynamics 365 Remote Assist mobile users.
- Fix for NullReferenceException showing up sometimes during inking and tutorial mode.

## iOS - 2020.7.30 + Android - 2020.07.23

Date: July 30, 2020

### Bug fixes

- Fix for not displaying the Dynamics 365 Remote Assist mobile user's video feed on the Microsoft Teams desktop or mobile user's screen.
- Fix for placing the arrow annotation at the incorrect angle for Microsoft Teams desktop or mobile users.
- Optimized frequency of error messages guiding user to track their environment better.
- Incoming calls improvements. 
- Fix for authentication taking a long time.
- Fix for annotations inaccuracy in calls between two Dynamics 365 Remote Assists clients.
- Fix for Undo and Delete buttons in the incorrect state.
- Fix for memory issues caused by screen rotation.
- Improved application memory usage.

## iOS - 2020.7.1 + Android - 2020.06.27

Date: July 1, 2020

### Bug fixes

-	Improved incoming call experience for Dynamics 365 Remote Assist mobile users who do not have the app open when a call comes in from Microsoft Teams desktop or mobile clients.
-	Fix for app crashing on mobile devices without augmented reality (AR) support, especially iPhone 5 and iPhone 6 devices.
-	Dynamics 365 Field Service customers can now view the service account names on the bookings screen. 
-	Updated the User Guide and Dynamics 365 Integration links in the app.
-	Update for authentication library on iOS.
-	Fix for “Just a moment” message blocking users after sign-in.
-	Fix for ArgumentNullException showing up when user doesn't have any recent contacts and search query returns empty list.
-	Fix for Graphics.CopyTexture exception showing after annotating on the snapshot.
-	Fixes for application localization (for example “Retry sign-in” button, “Don’t show again” button and tracking error state messages).
-	Performance improvements for the application memory usage.

## iOS - 2020.5.28 + Android - 2020.05.22

Date: May 28, 2020

### Bug fixes 

-	Fix for network error “HTTP 401 TeamsChatService.GetMessagesAsync”.
-	Fix for application not being responsive during launch.
-	Improvement for the recent contacts list.
-	Fix for not being able to find contacts in some countries, such as Egypt.
-	Improvement for the voicemail card.
-	Localization improvements.
-	Accessibility improvements and fixes.

## iOS – 2020.5.7 + Android - 2020.05.04

Date: May 4, 2020

### Bug fixes

- Improved flighting implementation and enabling per company app customizations.
- Fix for sign-in problem for users on mobile networks.
- Improved user feedback questionnaire experience.

## iOS – 2020.4.1 + Android - 2002.03.18

Date: April 1, 2020

### Bug fixes

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

## iOS – 2020.02.27 + Android - 2020.02.20

Date: February 27, 2020

### Bug fixes

- In low-bandwidth environments with a satellite network of 1000/256 kbps for bandwidth, 600/600ms for latency, and 10% of packet loss, users will not receive an 'Update Check Failed' pop-up and can continue to share their environment.  
- Users trying the 90-day license-free Dynamics 365 Remote Assist Mobile trial who don't have a Microsoft Teams license (free or paid) will be prompted to sign up for one. After they sign up, the app will recognize their Microsoft Teams account and they can sign in.  
- With Dynamics 365 Remote Assist mobile app downloaded on your device, users can launch the app from Safari web browser via “ramobile:/” deep linking.  
- Users can view their snapshots with annotations on it in both landscape and portrait orientations. These snapshots will save to users’ mobile device’s Photo Gallery.  
- In the text chat, the keyboard remains open after sending a message. 
- The ‘Lost Tracking' pop-up is localized in our supported languages. 
- The correct year is shown when users’ mobile device is set to the future in Thai. 
- Error message improvements.  

## iOS – 2020.12.12 + Android - 2019.12.09

Date: December 12, 2020

### Bug fixes

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

## iOS – 2020.10.31 + Android - 2019.10.22

Date: October 31, 2020

### Bug fixes 

- The Screenshot button is removed from the toolbar. You can edit a screenshot by selecting the Snapshot and annotate button instead.
- If there's a network disconnection, you’re automatically rejoined to the call when the network is restored. If there’s no network connection, the call is ended.
- If you’re using a screen reader and access the tutorial page accessed from the Learn the Tools or Try It button, you can access the Arrow tool.
- If you tap the Try It button on the Sign-in page, and then select the back button on your device, you return to the Sign-in page.
- The end-user license agreement (EULA) link on the Sign-in page goes to the appropriate page (Android or iOS) based on your device.
- On the tutorial page, the buttons now read: Restart Tutorial and Exit Practice.
- If you’re using Dynamics 365 Field Service with Dynamics 365 Remote Assist, the Post to Dynamics 365 pop-up will disappear when you receive or accept a call, but will reappear after the call has ended.
- The “NullReferenceException: Object reference not set to an instance of an object” error message does not appear when starting a call, whether system-generated logs are enabled or not.

## Locate your version number

To find which version of Dynamics 365 Remote Assist mobile you have, go to the menu and select the **Information** option. You'll see the **App Version** there. See the following screenshot for reference.

> [!div class="mx-imgBorder"]
> ![Screenshot of Dynamics 365 Remote Assist on a mobile device, showing the information option and the app version listed.](./media/ram-version-history-locate.png)
