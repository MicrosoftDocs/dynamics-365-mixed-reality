---
title: Overview of Dynamics 365 Remote Assist on HoloLens 2
author: davepinch
description: Overview of Dynamics 365 Remote Assist features and links to HoloLens 2 gestures.
ms.author: davepinch
ms.date: 04/22/2024
ms.topic: overview
ms.reviewer: v-wendysmith
---

# Overview of Dynamics 365 Remote Assist on HoloLens 2

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

When you use Microsoft Dynamics 365 Remote Assist on HoloLens 2, you can collaborate with one or more Microsoft Teams desktop users or one Teams mobile user. 

## Requirements

To use Dynamics 365 Remote Assist with HoloLens 2, you need:

- A subscription to Dynamics 365 Remote Assist and Microsoft Teams. The Teams license is included with Dynamics 365 Remote Assist. 
- A HoloLens 2 running the [Windows 10 April 2018 update](requirements.md) or later.
- A remote collaborator using the Teams desktop application or the Teams mobile app.  
- An internet connection. At least [1.5 mpbs of bandwidth is recommended](/microsoftteams/upgrade-prepare-environment-prepare-network#bandwidth-planning).
- Your credentials for signing into the HoloLens and Dynamics 365 Remote Assist.
- Dynamics 365 Remote Assist installed on your HoloLens 2.
- (Optional) If you're a Dynamics 365 Field Service customer, a [Dynamics 365 Remote Assist Attach license](buy-remote-assist.md) to connect to Dynamics 365 Field Service from Dynamics 365 Remote Assist.

## Overview of core features

When you launch Dynamics 365 Remote Assist, the **Call** tab is selected by default. This tab shows your recent contacts. You can use the tools in the top-right corner to access Dynamics 365 Field Service bookings, move the window, or pin the window to a particular place in your world.  

![Screenshot of the HoloLens field of view, showing the Call tab screen.](media/02.00-contacts.png)

Select the **Files** tab at any time (before, during, or after a call) to access service-related documents from OneDrive.

![Screenshot of the HoloLens field of view, showing the Files tab screen.](media/06.00-files.png "Files")

Select the **Settings** tab to:

- Configure various settings
- Provide feedback
- Watch a brief tutorial (the same tutorial that appears the first time you use Dynamics 365 Remote Assist)
- Find other tutorials 
- Switch your Dynamics 365 instance

![Screenshot of the HoloLens field of view, showing the Settings tab screen.](media/08.00-settings.png "Settings")

When you join a call or meeting, a video card appears. When you're in a call, the tools appear at the top and bottom of the video card. The participant tray displays the avatars for all call participants.  

![Screenshot of Dynamics 365 Remote Assist on HoloLens showing an active call showing the recording button.](media/03.00-call.png)

## Annotation and other tools

Anyone on the call can use the following tools:

|Button|Description|
|------|-----------------------------------------------------------------------------------|
|![Graphic showing the annotate with arrows button.](media/RAHL_Arrow.png "Arrow")|Annotate with arrows.|
|![Graphic showing the pencil or ink button.](media/RAHL_Ink.png "Ink")|Annotate with drawings.|
|![Graphic showing the colors button.](media/RAHL_Color.png "Colors")|Change annotation colors.|
|![Graphic showing the undo button.](media/RAHL_Undo.png "Undo")|Undo an action.|
|![Graphic showing the delete button.](media/RAHL_Trash.png "Delete")|Delete all annotations.|
|![Graphic showing the camera button.](media/RAHL_Camera.png "Camera")|Take a photo of what you see.|
|![Graphic showing the pin button.](media/RAHL_Pin.png "Pin")|Pin the call window wherever you want. Use the same button to unpin the call window.|

Anyone on the call can also send files, which appear in the space of the people they're collaborating with.  

## Types of calls supported

- A Dynamics 365 Remote Assist HoloLens user can join a one-to-one call, group call, or meeting with a Teams desktop user.

- A Dynamics 365 Remote Assist HoloLens user can join a one-to-one call with a Teams mobile user.

- Remote collaborators can join the call using the Microsoft Teams desktop application or the Teams mobile app.  

In a call, remote collaborators can see everything the HoloLens user sees (including holograms and the real world behind the holograms) and can add annotations, insert files, and more.

## HoloLens 2 gestures in Dynamics 365 Remote Assist

For basic navigation, see [HoloLens 2 gestures](/hololens/hololens2-basic-usage).

- Open the **Start** menu by tapping your wrist.

- Select holograms with gaze, air tap, voice, and touch.

- Move, resize, and rotate apps.

- If the object is out of your reach, extend your arm, aim your hand ray, and then air tap.

- If the object is within your reach, touch it directly.

## Voice

A good way to learn Dynamics 365 Remote Assist features and voice commands is to say "Remote Assist." When you're in a call, the app shows what it believes you said by showing a check mark and "Remote Assist." Then the app shows the name of each button. After a few seconds, the labels automatically disappear.

To see the labels again after they disappear, hover your finger over the button. If the Dynamics 365 Remote Assist user interface is out of reach, extend your arm and hover the hand ray over the button.

## Supported languages

[Check the FAQ to see if your language is supported](faq-hololens.md).

## Benefit of integrating with Dynamics 365 Field Service

If your organization uses Dynamics 365 Field Service to manage work orders, the technician using HoloLens 2 can view Dynamics 365 Field Service bookings from Dynamics 365 Remote Assist and do heads-up, hands-free calling in the context of a Field Service booking. For example, the technician can:

- View booking details

- Quickly call the assigned collaborator  

- Save snapshots to a booking

- Save call artifacts to the work order that the booking is associated with, including the call log and files shared during the call.

[Learn more about integrating Dynamics 365 Field Service](troubleshoot-field-service.md).

[!INCLUDE[footer-include](../includes/footer-banner.md)]
