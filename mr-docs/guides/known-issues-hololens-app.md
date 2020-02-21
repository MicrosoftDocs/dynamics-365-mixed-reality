---
author: BryceHo
description: Known Issues with Dynamics 365 Guides HoloLens app
ms.author: makamat
ms.date: 02/25/2020
ms.service: crm-online
ms.topic: article
title: Known Issues with Dynamics 365 Guides HoloLens app
ms.reviewer: v-brycho
---

# Known Issues with the Dynamics 365 Guides HoloLens app

## I can't sign in

To sign in, you must use the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365](../includes/pn-dyn-365.md)] sign-in credentials for your organization. It will resemble: johndoe@contoso.onmicrosoft.com. You can't use a [!include[cc-microsoft](../includes/cc-microsoft.md)] account (used for Outlook.com, [!include[cc-microsoft](../includes/cc-microsoft.md)] Store, and so on) or your corporate credentials to sign in. 

If you see any of the following errors, contact your IT admin, or see the self-service documentation at <https://aka.ms/guidesdocs>:

- [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] isn't set up correctly, or you might not have permission to access it. Contact your admin, or see the [self-service documentation](https://aka.ms/guidesdocs).

- Your client app version doesn't support your [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution version. Update your client app, contact your admin, or see the [self-service documentation](https://aka.ms/guidesdocs).

- You don't have a license to use [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. Contact your admin.

## Staying on the account picker for more than 25 seconds during HoloLens sign-in will make it unresponsive

When you get to the screen where you can select between different saved accounts on [!include[pn-hololens](../includes/pn-hololens.md)], choose an option within 25 seconds. After 25 seconds, it becomes unresponsive, and you will need to restart the app. This issue has been fixed on RS5 but still exists on RS4 if you have that installed.

## When placing large assets on HoloLens, you might see minor loading delays
The [!include[pn-hololens](../includes/pn-hololens.md)] app currently loads the guide right after you open it, and in the background as you use the guide. If your guide contains large 3D models and media, you might experience loading delays of a few seconds.

## Circular code anchor method requires user's consent to use the camera

When the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] application on [!include[pn-hololens](../includes/pn-hololens.md)] is launched for the first time, the app will ask the user to provide consent to use the camera. If you plan to use circular code anchors in your guides, you will need to say **Yes** to this prompt. This is required for every device you use the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] application on. If this consent was not provided previously, you can go to the **Settings** menu on the [!include[pn-hololens](../includes/pn-hololens.md)] (operating system) and provide consent to the app. 

## I don't see any guides in the Guides list

If you don't see any guides, either your internet connection is unstable, or you might have signed into an instance that doesn't have any guides. First, check your internet connection. If you're connected, try signing in again, but this time make sure you sign into the instance that has the guides you were looking for. If you still don't see any guides, contact your administrator.

## The profile picture shown in the app is incorrect 

Make sure you're signed in. To do this, select the profile picture, and then sign out and sign back in with your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] credentials. Your profile picture should appear correctly.

Signing in with the right credentials ensures that your work progress is correctly tracked in [!include[pn-dyn-365](../includes/pn-dyn-365.md)].

## The video preview on a step is blurry

The [!include[pn-hololens](../includes/pn-hololens.md)] app converts and resizes videos when they're uploaded to ensure optimal performance on [!include[pn-hololens](../includes/pn-hololens.md)]. If your video was recorded at a very high resolution, or if it's extremely large, the transcoding process might have degraded its quality. Re-record and upload a new video, keeping length and resolution in mind.

As a best practice, video clips should not be too long (**maximum of 2 minutes**). This helps operators focus on one meaningful task at a time and keeps them from getting overwhelmed. 

## The see-through style, when applied to a 3D model might show gray areas instead of rendering textures properly

There are some problems with rendering the "see through" style on some 3D models. Some surfaces on these models will look gray. Please use another style if you see this problem, or contact customer service if this is a must-have and you need help with it.

## When moving a 3D model during authoring on HoloLens, the movement of the model may seem slow

To allow authors to place 3D models carefully and precisely, the default movement is set to be slow. To indicate this, the manipulation sphere around the model will be blue. You can move your hand faster, or wiggle the model a bit to switch it to move faster. 

## I have an issue that isn't listed in these troubleshooting steps
Please contact customer service: [https://docs.microsoft.com/dynamics365/get-started/support/](https://docs.microsoft.com/dynamics365/get-started/support/). This page can also be found by signing in to your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] account and selecting the **Support** link.

## See also

[Known issues with Dynamics 365 Guides generally](known-issues.md)<br>
[Known issues with the PC app](known-issues-pc-app.md)<br>
[Dynamics 365 Guides FAQ](faq.md)
