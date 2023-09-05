---
author: davepinch
description: Frequently asked questions about Dynamics 365 Guides
ms.author: davepinch
ms.date: 04/28/2023
ms.topic: article
title: FAQ about Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# Frequently asked questions about Microsoft Dynamics 365 Guides

[See also Dynamics 365 Guides 8.0 FAQ](faq-version-8.md)

## How do I contact Support if I don't find an answer in this FAQ?

If you're not able to use Microsoft Dynamics 365 Guides, or if you have an issue that isn't answered in this FAQ or in the documentation, please contact Customer Support by using the following steps:

1. Go to [https://dynamics.microsoft.com/support/](https://dynamics.microsoft.com/support/).

2. Under **Customer Engagement help + support**, select **GET SUPPORT**.

3. Find a phone number or submit a support request through the admin center. 

## Which Microsoft platforms is Dynamics 365 Guides dependent on?
 
Dynamics 365 Guides is dependent on three Microsoft platforms:
 
- Microsoft Dataverse
- Microsoft Dynamics 365 Core Service
- Microsoft Teams
 
In rare cases, changes to these underlying platforms can cause issues in Dynamics 365 Guides. Likewise, a change to one of these platforms can resolve a Dynamics 365 Guides issue. To learn about the schedule for changes to these platforms, see the following articles:

- [Released versions of Microsoft Dataverse](/dynamics365/released-versions/microsoft-dataverse)
- [Released versions of Dynamics 365 Core Service Scheduling](/dynamics365/released-versions/dynamics365-css)
- [Update history for Microsoft Teams app version (Public Cloud and GCC)](/officeupdates/teams-app-versioning)

## How do I stream my HoloLens view to a PC using Miracast?

The Connect app for wireless projection using Miracast is no longer installed by default on the PC, but is available as an optional feature. To install the app on the PC, select **Settings** > **Apps** > **Optional features** > **Add a feature**, and then install the Wireless Display app. 

The Connect app is automatically installed by default on the HoloLens. To initiate sharing from the HoloLens:

From the OS start menu, select **Cast screen** :::image type="icon" source="media/hololens-cast-screen.png":::.

## I don't see my Dynamics 365 Guides environment even though I have a valid Dynamics 365 Guides license. What should I do? 

You might have installed Dynamics 365 Guides on a trial environment that has expired. Trial environments have their own life cycle, independent of the Dynamics 365 Guides license. You can go to [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), select your trial environment, and switch it to a production environment.

## Can I add more than eight 3D models to a step?

There are only eight **3D parts** boxes in the bin, which limits the variety of 3D models you can add to a single step. When placing holograms on the HoloLens, you can, however, place an unlimited number from the bin. For example, you can add up to eight different 3D models (arrows, boxes, nuts, drills, and so on) to the bin, but you can place as many arrows, boxes, nuts, and drills from each **3D Parts** box that you want when in HoloLens. To do this, either tap the asset bins to spawn 3D models or go to a 3D model's **Edit** menu and select **Duplicate**.

## I see a triangle-shaped hazard sign when I load a step. What does that mean?

The hazard sign is a placeholder for 3D models, videos, or images that can't be successfully loaded in the HoloLens app. Possible reasons for this:

- This might occur due to intermittent connectivity issues or because the file is too large. If you see this, please relaunch the HoloLens app. If this doesn't fix the problem, launch the PC app, find the file in question, and open it in preview mode. If the preview loads, reinstall the HoloLens app and try launching the guide again. 

- If you can't find the file in the PC app library, the reference (entity) to the 3D model/video/image is broken. Please upload the file again and re-author the guide.

- If the file exists in the library but the preview doesn't load, there's a problem with the file information in Guides. Please upload the file again, and then edit the guide to refer to this new asset wherever applicable.

## Why does the HoloLens app require permissions to launch?

The HoloLens app includes advanced features that rely on eye-tracking, voice, camera, and movement to function properly. For example, you need eye tracking to access the Main menu. [Learn more about the permissions required to use the HoloLens app](hololens-permissions.md)  

## See also

[Known Issues in Dynamics 365 Guides](known-issues.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
