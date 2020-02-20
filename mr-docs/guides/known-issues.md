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

## Improvements for 3D model positioning in the October 1 release might shift models in guides that were created before October 1, 2019

The October 1 release includes refactoring of code for hologram positions to enhance overall performance and enable future improvements. You may notice that the position of some imported models, which have had scale applied to them, might be shifted. You will need to re-position those 3D models. This does not impact the position of models from the 3D toolkit.
 
## Keep file names for 3D models and media short

Before you upload custom 3D models or media files in the PC app, please make sure the file names are not more than 60 characters, and do not contain special characters (&, @, and so on). 

Large 3D models are stored in [!include[pn-hololens](../includes/pn-hololens.md)] memory while in use; therefore, the experience is significantly slower if there are too many models in a guide. **For reasonable performance, we recommend that you don't exceed 450 MB of 3D models in a single guide.** 

## Text wrapping on PC and HoloLens might differ in rare cases

In rare cases, you might notice that text is wrapped on the step card view in [!include[pn-hololens](../includes/pn-hololens.md)] but not on the PC. This is because [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] renders fonts at different sizes for readability between PC and [!include[pn-hololens](../includes/pn-hololens.md)], and different widths of characters might cause them to go to the next line. To ensure this does not affect operator experience, validate the text on all steps on the [!include[pn-hololens](../includes/pn-hololens.md)] app before sharing your guides with operators.

## When placing large assets on HoloLens, you might see minor loading delays
The [!include[pn-hololens](../includes/pn-hololens.md)] app currently loads the guide right after you open it, and in the background as you use the guide. If your guide contains large 3D models and media, you might experience loading delays of a few seconds.

## You can create guides with the same name without overwriting old guides

You can create multiple guides with the same name. While this prevents unintentional overwrites of old files, it's confusing when you choose a guide from a list. When you create a new guide, make sure to use a unique name.

## 3D content and media cannot be renamed or deleted from the PC app after uploading

At this time, we do not support renaming or deleting 3D content and media once they have been uploaded to the server. While it's possible to rename them in [!include[pn-dyn-365](../includes/pn-dyn-365.md)], doing so can have unintended consequences on any guides that use this content.

## 3D content and media will be overwritten if you upload new content with the same name

We do not support multiple files with the same name in the current release. When uploading new 3D models or media, check to make sure a file with the same name does not exist in the library. You can, however, have different types of files with the same name—for example, a bolt.png image and a bolt.glb 3D model.

## Can't use the same name for 3D parts that you upload, even if they have different extensions

The app currently looks up media by file names. So, for example, if you have a picture.jpg file and a picture.png, the app doesn't know which file to show for the step. So it's best to always use unique file names for media files you upload.

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

