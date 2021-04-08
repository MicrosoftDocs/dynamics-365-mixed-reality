

# Version history for Dynamics 365 Remote Assist

This article provides a version history for Microsoft Dynamics 365 Remote Assist features. For the most recent features, see [What's new in Dynamics 365 Remote Assist](whats-new.md). To see a comprehensive list of released and upcoming features, see [Dynamics 365 and Power Platform release plans](https://docs.microsoft.com/dynamics365/release-plans/), which summarize early access features, preview features, monthly general availability enhancements, and bug fixes.

## September 2020

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|211.2009.7002.0|
|iOS mobile app|2020.9.1|
|Android mobile app|2020.09.04|

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





## August 2020

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|211.2007.30002|

### Bug fixes

#### HoloLens 2

- Fix for the files shared from Microsoft Teams not downloading on HoloLens. 
- Fix for the "Snap" voice command not taking a photo in some cases.
- Fix for when the user answers a call from the shell and it takes them to the contacts screen rather than joining the call. 
- Fix for the Dynamics 365 Remote Assist video card appearing too close after the call has ended. 
- Improved application reliability. 




## July 30, 2020

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.7.30|
|Android mobile app|2020.07.23|

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





## July 2020

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|210.2007.1003.0|
|iOS mobile app|2020.7.1|
|Android mobile app|2020.06.27|

### Bug fixes

#### HoloLens 2

- A Dynamics 365 Remote Assist HoloLens user using GCC High can successfully join a meeting. 
-	Fixed bug in group calls on HoloLens 1 where remote collaborators are unable to annotate from Microsoft Teams client.   
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





## June 2020

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 2|209.2006.11003.0|

### Bug fixes

#### HoloLens 2

- Fixed bug in group calls where remote collaborators are unable to annotate from Microsoft Teams client.
- Improvements to the Join Meeting feature to select between overlapping meetings.
- Fixed bug with the snapshot tool causing photos taken with the snapshot tool to not be sent through Teams chat.
- Fixed bug with the snapshot tool where the camera cursor would appear in the resulting photo.
- Various near-field / far-field interaction fixes.
- Fixed bug where the outgoing video feed may not work when answering a call from the HoloLens shell.
- Various fixes to enable users in Egypt to use Dynamics 365 Remote Assist.
- Incoming calls are now supported for GCC High and DOD.





## May 28 2020

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.5.28|
|Android mobile app|2020.05.22|

### Bug fixes

#### iOS and Android mobile app

- Fix for network error “HTTP 401 TeamsChatService.GetMessagesAsync”.
-	Fix for application not being responsive during launch.
-	Improvement for the recent contacts list.
-	Fix for not being able to find contacts in some countries, such as Egypt.
-	Improvement for the voicemail card.
-	Localization improvements.
-	Accessibility improvements and fixes.





## May 4 2020

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.5.7|
|Android mobile app|2020.05.04|

### Bug fixes

#### iOS and Android mobile app

- Improved flighting implementation and enabling per company app customizations.
- Fix for sign-in problem for users on mobile networks.
- Improved user feedback questionnaire experience.





## April 2020

### Version info

|Device|Version|
|------------------------------------------|---------------------------------------------|
|HoloLens 1 and 2|208.2004.1002.0|
|iOS mobile app|2020.4.1|
|Android mobile app|2002.03.18|

### Bug fixes

#### HoloLens 1 and 2

- Fixed various speech command bugs.
- Improvements to tool tips.
- Improvements to annotation stability.
- Fixed several application stability-related bugs.
- Various bug fixes for joining Teams meetings.
- Fixes to keyboard interaction and usability.
- Various video quality fixes including support for SimulCast, bandwidth history, & network probing to improve overall video quality.
- Fixed text chat bug that was causing text chats not to show on HoloLens.
- Various near-field / far-field interaction fixes.

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




## Feburary 27,  2020

### Version info

|Device |Version|
|------------------------------------------|---------------------------------------------|
|iOS mobile app|2020.02.27|
|Android mobile app|2020.02.20|

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
