---
title: What's new in Dynamics 365 Remote Assist
author: amaraanigbo
description: Overview of what's new in Dynamics 365 Remote Assist
ms.author: soanigbo
ms.date: 01/27/2022
ms.service: crm-online
ms.topic: article
ms.reviewer: v-bholmes
---

# What's new in Dynamics 365 Remote Assist

This article describes details about the **current wave of features (October 2021 through March 2022)** for Dynamics 365 Remote Assist, organized by release date. To see a comprehensive list of released and upcoming features, see [Dynamics 365 and Power Platform release plans](https://docs.microsoft.com/dynamics365/release-plans/). You can also see a complete list of [features organized by previous waves](version-history.md).

## January 27, 2022

### Features

|Feature|How to|
|-----------------------------------------------|----------------------------------------------------|
|[New Restricted mode prevents users from making private calls, and accessing files and assets](https://docs.microsoft.com/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/planned-features)|[Protect company information by restricting capabilities in Dynamics 365 Remote Assist](restricted-mode-overview.md)|

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
|[Support for spotlight and pinning for video feed on Microsoft Teams desktop](https://docs.microsoft.com/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/support-spotlight-pinning-remote-assist-video-feed-teams-desktop)|None|

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
|[One-time-call users can open files shared with them from the mobile app](https://docs.microsoft.com/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/one-time-call-users-open-files-shared-them)|[Invite a user to join a one-time call](one-time-call.md)|
|[Support for a subset of Microsoft Teams policies](https://docs.microsoft.com/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/support-subset-teams-policies)|[Teams policies supported by Dynamics 365 Remote Assist](teams-policies.md)|
|[Accuracy improvements for mixed-reality annotations on mobile](https://docs.microsoft.com/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/accuracy-improvements-mixed-reality-annotations-mobile)|None|
|[Support for spotlight and pinning for video feed on Microsoft Teams desktop](https://docs.microsoft.com/dynamics365-release-plan/2021wave2/remote-assist/dynamics365-remote-assist/support-spotlight-pinning-remote-assist-video-feed-teams-desktop)|None|

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
