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

## Staying on the account picker for more than 25 seconds during HoloLens sign-in will make it unresponsive

When you get to the screen where you can select between different saved accounts on [!include[pn-hololens](../includes/pn-hololens.md)], choose an option within 25 seconds. After 25 seconds, it becomes unresponsive, and you will need to restart the app. This issue has been fixed on RS5 but still exists on RS4 if you have that installed.

## When placing large assets on HoloLens, you might see minor loading delays
The [!include[pn-hololens](../includes/pn-hololens.md)] app currently loads the guide right after you open it, and in the background as you use the guide. If your guide contains large 3D models and media, you might experience loading delays of a few seconds.

## Circular code anchor method requires user's consent to use the camera

When the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] application on [!include[pn-hololens](../includes/pn-hololens.md)] is launched for the first time, the app will ask the user to provide consent to use the camera. If you plan to use circular code anchors in your guides, you will need to say **Yes** to this prompt. This is required for every device you use the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] application on. If this consent was not provided previously, you can go to the **Settings** menu on the [!include[pn-hololens](../includes/pn-hololens.md)] (operating system) and provide consent to the app. 

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

## How do I address hardware offset in HoloLens 1 devices to ensure accurate placement of holograms for circular code anchor alignment
 
The angle of each [!include[pn-hololens](../includes/pn-hololens.md)] 1 PV camera (the camera placed above the nose bridge) can be slightly different across devices due to manufacturing idiosyncrasies. Since the PV camera is used to scan the printed marker, this means holograms can appear slightly misaligned when using the same guide and same circular code anchor on multiple devices.
 
To fix this issue, the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] [!include[pn-hololens](../includes/pn-hololens.md)] app provides the ability to manually adjust for this offset and save the settings to the device so that each user does not need to set the offset each time. We recommend that IT staff go through the following steps before provisioning devices to [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] authors or operators. This is a one-time setup and does not need to be repeated unless the app is uninstalled or a new operating system is installed.
 
### Step 1 – Set up circular code anchor

#### On the PC

- Open the PC app, and then create a guide [using the circular code anchor method](anchor.md) (or you can use an existing guide that already uses the circular code anchoring method).

#### On HoloLens

- Run the [!include[pn-hololens](../includes/pn-hololens.md)] Calibration app to ensure proper fit and IPD.
 
### Step 2 – Open the guide and align it on HoloLens

1.	Open the HoloLens app, select **Operator** or **Author** mode, and then open the guide used in step 1.

2.	Select **Scan** to begin the alignment process. Accept the permissions prompts that appear. 

3. Look for your circular code anchor, allow the device to find the anchor, and wait for the blue outline animation. The blue outline shows where the circular code anchor is located, as calculated by [!include[pn-hololens](../includes/pn-hololens.md)].

### Step 3 – Adjust the offset

The blue outline is the same size as the anchor. You can move it up or down along the rails positioned at its corners. Look at the anchor from above. Is the blue outline too far to the left or right of the anchor? If so, try adjusting [!include[pn-hololens](../includes/pn-hololens.md)] to make sure it fits correctly on your head.

Tap and hold the blue outline and move it up or down until it overlaps with the anchor exactly. Make sure that the outline is exactly aligned by looking at the anchor from the side. 
 
The media panel shows the following image to visually indicate what you need to do.

![Adjust printed marker offset](media/adjust-marker-offset.png "Adjust printed marker offset")  

After you have verified that the blue outline and the anchor are lined up, select **Confirm** to complete the process. 

The next time this device is used to load a guide, the operator/author can just scan the anchor; they won't have to adjust the blue outline again.

If, at any point, you need to readjust this setting, you can trigger the offset adjustment process again by selecting the **Adjust Offset** setting. When you turn this setting on, it triggers the normal alignment process, beginning with the scanning of the printed marker.

## See also

[Known issues with Dynamics 365 Guides generally](known-issues.md)<br>
[Known issues with the PC app](known-issues-pc-app.md)<br>
[Dynamics 365 Guides FAQ](faq.md)
