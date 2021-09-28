---
author: Mamaylya
description: Learn about known issues with the Microsoft Dynamics 365 Guides PC app.
ms.author: mamaylya
ms.date: 04/01/2020
ms.topic: article
title: Known issues with the Dynamics 365 Guides PC app
ms.reviewer: v-brycho
---

# Known issues with the Dynamics 365 Guides PC app

## I can't open a non-English Example guide

Some customers might have installed the Example guide that is included with Microsoft Dynamics 365 Guides in an existing instance. As of the April 28, 2020, release, the Example guide is obsolete and will no longer be installed in new instances. 

As part of this change, you won't be able to open an existing non-English (localized) Example guide. If you try, you will be redirected to the **Guides** list.

## I can't find the guide that I created

In the list of guides, look for newly created guides on the **All** tab. The **Recents** list shows only those guides that have previously been opened on the device. It doesn't include guides that were recently created in the PC authoring app. 

## Keep file names short for 3D models and media

Before you upload custom 3D models or media files in the PC app, make sure that the file names are no longer than 60 characters. Also make sure that they don't contain special characters such as ampersands (&) and at signs (@). 

Large 3D models are stored in [!include[pn-hololens](../includes/pn-hololens.md)] memory while they are used. Therefore, the experience is significantly slower if there are too many models in a guide. **For reasonable performance, we recommend that the total size of 3D models in a single guide not exceed 450 megabytes (MB).** 

## You can create guides that have the same name without overwriting old guides

You can create multiple guides that have the same name. Although this capability helps prevent unintentional overwrites of old files, it can cause confusion when you select a guide in a list. Therefore, when you create a new guide, be sure to use a unique name.

## 3D content and media can't be renamed or deleted from the PC app after they are uploaded

Currently, you can't rename or delete 3D content and media after they have been uploaded to the server. Although you can rename the 3D content and media in [!include[pn-dyn-365](../includes/pn-dyn-365.md)], name changes can have unintended consequences for any guides that use that content.

## 3D content and media are overwritten if you upload new content that has the same name

The current release doesn't support multiple files that have the same name. Therefore, when you upload new 3D models or media, make sure that the library doesn't already include files that have the same names. However, files of different types can have the same name. For example, you can have an image that is named bolt.png image and a 3D model that is named bolt.glb.

## You can't use the same name for 3D parts that you upload, even if they have different extensions

The app currently looks up media by file name. For example, if you have one file that is named picture.jpg and another that is named picture.png, the app can't determine which file should be shown for a step. Therefore, as a best practice, you should always use unique file names for media files that you upload.

## You don't see media or 3D content that you uploaded to the app

Currently, when you upload content, the app doesn't automatically scroll to the place in the library where the content is uploaded. To find the content, go to the library on the right side of the page, and select the appropriate tab (**3D parts**, **Images**, **Actions**, **Videos**, or **3D toolkit**).

If any errors occurred during upload, the PC app shows notifications in the title bar. Make sure that content that you upload is in the correct file format. For information about supported file formats, see [What file formats are supported for 3D models, images, and videos?](create-steps-assign-media.md#what-file-formats-are-supported-for-3d-models-images-and-videos). 

If you still can't find your content, contact your admin.

## Deleting an asset from a step (from the bin) in the PC app removes all previously placed instances on HoloLens

You might have an existing guide where an asset was placed in the bin in the PC app, and then instances of that asset were placed in the world on [!include[pn-hololens](../includes/pn-hololens.md)]. If you delete the asset from the bin while you're editing this guide, all instances that have been placed in the world are removed. Those placed instances won't be restored if you add the asset again. To restore them, select the **Undo** button in the PC app.

## Uploading glTF files that have dependencies across different folders might cause upload errors

Some glTF files might have dependencies in other folders. During upload, if the app doesn't have permissions to those folders, errors can occur, or 3D models in the gallery might be broken. When you upload glTF models, make sure that you have permissions to all dependencies, or that all dependencies are in the same folder.

## See also

[Known issues with Dynamics 365 Guides generally](known-issues.md)<br>
[Known issues with the HoloLens app](known-issues-hololens-app.md)<br>
[Dynamics 365 Guides FAQ](faq.md)



[!INCLUDE[footer-include](../includes/footer-banner.md)]