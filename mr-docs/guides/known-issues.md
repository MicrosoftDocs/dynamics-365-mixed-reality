---
author: BryceHo
description: Known Issues with Dynamics 365 Guides
ms.author: makamat
ms.date: 02/25/2020
ms.service: crm-online
ms.topic: article
title: Known Issues with Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Known issues with Microsoft Dynamics 365 Guides

## I can't sign in

To sign in, you must use the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365](../includes/pn-dyn-365.md)] sign-in credentials for your organization. It will resemble: johndoe@contoso.onmicrosoft.com. You can't use a [!include[cc-microsoft](../includes/cc-microsoft.md)] account (used for Outlook.com, [!include[cc-microsoft](../includes/cc-microsoft.md)] Store, and so on) or your corporate credentials to sign in. 

If you see any of the following errors, contact your IT admin, or see the self-service documentation at <https://aka.ms/guidesdocs>:

- [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] isn't set up correctly, or you might not have permission to access it. Contact your admin, or see the [self-service documentation](https://aka.ms/guidesdocs).

- Your client app version doesn't support your [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution version. Update your client app, contact your admin, or see the [self-service documentation](https://aka.ms/guidesdocs).

- You don't have a license to use [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. Contact your admin.

## Improvements for 3D model positioning in the October 1 release might shift models in guides that were created before October 1, 2019

The October 1 release includes refactoring of code for hologram positions to enhance overall performance and enable future improvements. You may notice that the position of some imported models, which have had scale applied to them, might be shifted. You will need to re-position those 3D models. This does not impact the position of models from the 3D toolkit.

## "Create account" link when signing in with a new account doesn't work
When signing in with a brand new account on the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps, there is a link to create a new account:

![Sign-in screen](media/sign-in-screen.PNG "Sign-in screen")  
 
Please do not use this link to create an account–it doesn't work.

## I can't see guides that I created or guides created by my teammates

If you don't see any guides, either your internet connection is unstable, or you might have signed in to an instance that doesn't have any guides. First, check your internet connection. If you're connected, try signing in again, but this time make sure you sign into the instance that has the guides you were looking for. If you still don't see any guides, contact your administrator.


## Text wrapping on PC and HoloLens might differ in rare cases

In rare cases, you might notice that text is wrapped on the step card view in [!include[pn-hololens](../includes/pn-hololens.md)] but not on the PC. This is because [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] renders fonts at different sizes for readability between PC and [!include[pn-hololens](../includes/pn-hololens.md)], and different widths of characters might cause them to go to the next line. To ensure this does not affect operator experience, validate the text on all steps on the [!include[pn-hololens](../includes/pn-hololens.md)] app before sharing your guides with operators.

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

[Known issues with the PC app](known-issues-pc-app.md)<br>
[Known issues with the HoloLens app](known-issues-hololens-app.md)<br>
[Dynamics 365 Guides FAQ](faq.md)

