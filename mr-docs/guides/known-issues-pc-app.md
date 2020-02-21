---
author: BryceHo
description: Known Issues with the Dynamics 365 Guides PC app
ms.author: makamat
ms.date: 02/25/2020
ms.service: crm-online
ms.topic: article
title: Known Issues with the Dynamics 365 Guides PC app
ms.reviewer: v-brycho
---

# Known issues with the Dynamics 365 Guides PC app

## I can't sign in

To sign in, you must use the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365](../includes/pn-dyn-365.md)] sign-in credentials for your organization. It will resemble: johndoe@contoso.onmicrosoft.com. You can't use a [!include[cc-microsoft](../includes/cc-microsoft.md)] account (used for Outlook.com, [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Store, and so on) or your corporate credentials to sign in. 

If you see any of the following errors, contact your IT admin, or see the self-service documentation at <https://aka.ms/guidesdocs>:

- [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] isn't set up correctly, or you might not have permission to access it. Contact your admin, or see the [self-service documentation](https://aka.ms/guidesdocs).

- Your client app version doesn't support your [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution version. Update your client app, contact your admin, or see the [self-service documentation](https://aka.ms/guidesdocs).

- You don't have a license to use [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. Contact your admin, or [sign up for a free trial subscription]().

## Keep file names for 3D models and media short

Before you upload custom 3D models or media files in the PC app, please make sure the file names are not more than 60 characters, and do not contain special characters (&, @, and so on). 

Large 3D models are stored in [!include[pn-hololens](../includes/pn-hololens.md)] memory while in use; therefore, the experience is significantly slower if there are too many models in a guide. **For reasonable performance, we recommend that you don't exceed 450 MB of 3D models in a single guide.** 

## You can create guides with the same name without overwriting old guides

You can create multiple guides with the same name. While this prevents unintentional overwrites of old files, it's confusing when you choose a guide from a list. When you create a new guide, make sure to use a unique name.

## 3D content and media cannot be renamed or deleted from the PC app after uploading

At this time, we do not support renaming or deleting 3D content and media once they have been uploaded to the server. While it's possible to rename them in [!include[pn-dyn-365](../includes/pn-dyn-365.md)], doing so can have unintended consequences on any guides that use this content.

## 3D content and media will be overwritten if you upload new content with the same name

We do not support multiple files with the same name in the current release. When uploading new 3D models or media, check to make sure a file with the same name does not exist in the library. You can, however, have different types of files with the same name—for example, a bolt.png image and a bolt.glb 3D model.

## Can't use the same name for 3D parts that you upload, even if they have different extensions

The app currently looks up media by file names. So, for example, if you have a picture.jpg file and a picture.png, the app doesn't know which file to show for the step. So it's best to always use unique file names for media files you upload.

## I don't see media or 3D content that I uploaded to the app

When you upload content, at this time, the app doesn't automatically scroll to the place in the library where the content is uploaded. To find the content, go to the library (right side of the screen), and then select the appropriate tab (**3D parts**, **Pictures**, **Videos**, or **3D toolkit**).

The PC app shows notifications (in the top title bar) if there are any errors during uploading. Check to make sure your content is in the right file format. [Learn about supported file formats for Dynamics 365 Guides](create-steps-assign-media.md#what-file-formats-are-supported-for-3d-models-images-and-videos). 

If you still can't find your content, contact your administrator.

## I have an issue that isn't listed in these troubleshooting steps

Please contact customer service: [https://docs.microsoft.com/dynamics365/get-started/support/](https://docs.microsoft.com/dynamics365/get-started/support/). This page can also be found by signing in to your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] account and selecting the **Support** link.

## See also

[Known issues with Dynamics 365 Guides generally](known-issues.md)<br>
[Known issues with the HoloLens app](known-issues-hololens-app.md)<br>
[Dynamics 365 Guides FAQ](faq.md)

