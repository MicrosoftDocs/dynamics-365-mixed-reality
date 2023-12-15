---
author: davepinch
description: Learn about known issues with the Microsoft Dynamics 365 Guides PC app.
ms.author: davepinch
ms.date: 12/15/2023
ms.topic: faq
title: Known issues with the Dynamics 365 Guides PC app
ms.reviewer: mhart
---

# Known issues with the Dynamics 365 Guides PC app

## The Guides PC app stops responding if you use a non-English language and select the **All** or **Recent** tab

If you use the Guides PC app in a non-English language and select the **All** or **Recent** tab on the Guides list, the app stops responding.

## I can't find the guide that I created

In the list of guides, look for newly created guides on the **All** tab. The **Recent** list shows only those guides that have previously been opened on the device. It doesn't include guides that were recently created in the PC authoring app.

## You can create guides that have the same name without overwriting old guides

You can create multiple guides that have the same name. Although this capability helps prevent unintentional overwrites of old files, it can cause confusion when you select a guide in a list. Therefore, when you create a new guide, be sure to use a unique name.

## Keep file names short for 3D models and media

Before you upload custom 3D models or media files in the PC app, make sure that the file names are no longer than 60 characters. Also make sure that they don't contain special characters such as ampersands (&) and at signs (@).

## Can't upload 3D content or other assets

If you can't upload your custom 3D parts, images, or videos, enable Guides to work in the background.

- For Windows 10: Go to **Settings** > **Apps & features** > **Dynamics 365 Guides** and select **Advanced options**. Turn on **Background apps**.

- For Windows 11: Go to **Settings** > **Apps** > **Installed apps** > **Dynamics 365 Guides** and select **Advanced options**. For **Let this app run in background**, select **Power optimized (recommended)**. If you still can't import, select **Always**.

## 3D content and media are overwritten if you upload new content that has the same name

The current release doesn't support multiple files that have the same name. Therefore, when you upload new 3D models or media, make sure that the library doesn't already include files that have the same names. However, files of different types can have the same name. For example, you can have an image that is named bolt.png image and a 3D model that is named bolt.glb.

## You can't use the same name for 3D parts that you upload, even if they have different extensions

The app currently looks up media by file name. For example, if you have one file that is named picture.jpg and another that is named picture.png, the app can't determine which file should be shown for a step. Therefore, as a best practice, you should always use unique file names for media files that you upload.

## You don't see media or 3D content that you uploaded to the app

Currently, when you upload content, the app doesn't automatically scroll to the place in the library where the content is uploaded. To find the content, go to the library on the right side of the page, and select the appropriate tab (**3D parts**, **Images**, **Actions**, **Videos**, or **Toolkit**). You can sort content by newest or by alphabetical order. Alternatively, you can search for a specific file name. 

If any errors occurred during upload, the PC app shows notifications in the title bar. Make sure that content that you upload is in the correct file format. For information about supported file formats, see [What file formats are supported for 3D models, images, and videos?](pc-app-supported-file-formats.md)

If you still can't find your content, contact your admin. There might be a permissions issue.

## Deleting an asset from a step (from the bin) in the PC app removes all previously placed instances on HoloLens

You might have an existing guide where an asset was placed in the bin in the PC app, and then instances of that asset were placed in the world on HoloLens. If you delete the asset from the bin while you're editing this guide, all instances that have been placed in the world are removed. Those placed instances won't be restored if you add the asset again. To restore them, select the **Undo** button in the PC app.

## Guest users can't see environment in PC app

The Dynamics 365 Guides PC app doesn't support guest access. Guest users can access Guides content as an operator, not as an author. For more information, see [Invite a guest user to operate a guide](admin-add-guest-user.md).

## See also

- [Known issues with Dynamics 365 Guides generally](known-issues.md)
- [Known issues with the HoloLens app](known-issues-hololens-app.md)
- [Dynamics 365 Guides FAQ](faq.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
