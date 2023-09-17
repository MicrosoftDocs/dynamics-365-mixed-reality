---
author: annitachow
ms.author: anchow
description: Learn how to package a guide and its content and share it with others in Dynamics 365 Guides. 
ms.date: 09/07/2023
ms.topic: how-to
title: Package a guide in Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Package a guide in Dynamics 365 Guides

Packaging a guide allows authors to create a self-contained, real-only file that contains a copy of all contents in a guide. Use a packaged guide to archive versions of a guide, easily migrate guides between environments, or quickly share content with others regardless of permission levels. The packaged guide can't be edited and can only be viewed with a HoloLens device in operator mode.

> [!IMPORTANT]
> Verify permissions on guide content before packaging a guide. Be aware of any sensitive information that might be shared and manage the packaged guide according to your organization's privacy policies.

## Limitations

- Maximum of 2 GB for a packaged guide
- Maximum of 100 MB 3D models and other assets
- Maximum of 500 MB to upload to the model-driven app
- Animated anchors aren't supported
- Offline mode isn't supported

## Package a guide in the PC app

1. In the PC app, open the guide you want to package and select **Package guide**.

   :::image type="content" source="media/package-guide.png" alt-text="Screenshot that shows the Package guide option.":::

1. Keep the default name or enter a unique name for the package guide. For example, provide the guide name and version number or guide name and status.

1. Select **Package**. The guide and all its contents is downloaded, archived into a *.guide* file, and uploaded to the Guides model-driven app. The packaged guide is listed with other guides on the **Home** page. The packaged guide is available to HoloLens users in operator mode.

## Manage a packaged guide in the PC app

A packaged guide can't be opened in the PC app. You can rename, deactivate, or share it.

1. In the PC app, select **Home** to view a list of guides.

1. Right-click the packaged guide you want to manage and choose one of the following options:

   - **Rename**: Change the name of the packaged guide.

   - **Deactivate**: Deactivate the packaged guide so it no longer appears in the library. To permanently delete it, contact an admin.

   - **Copy link to this guide**: Copy the link to the packaged guide to share it with someone in the same environment.

## Share a packaged guide with someone in a different environment

1. Have the author of the guide [create a packaged guide](#package-a-guide-in-the-pc-app).

1. Have the author [download the packaged guide](#download-a-packaged-guide-in-the-model-driven-app) and send you the *.guide* file.

1. Access your environment and [upload the packaged guide](#upload-a-packaged-guide-in-the-model-driven-app).

## Download a packaged guide in the model-driven app

Download a packaged guide to share it with others.

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. Under **Content**, on the left side of the screen, select **Packaged Guides**.

1. Navigate to the packaged guide file and select it. The record for the packaged guide opens.

   > [!TIP]
   > You can rename the packaged guide.

1. Select the packaged guide link. A zip file automatically downloads to your downloads folder that you can share with others.

   :::image type="content" source="media/mda-packaged-guide-link.png" alt-text="Screenshot that shows the link of the packaged guide file to download.":::

> [!IMPORTANT]
> Packaged content is no longer protected by permissions that might be set by your organization. If a guide contains sensitive information, take precautions according to your organization's privacy policies before sharing it.

## Upload a packaged guide in the model-driven app

If you have received a packaged guide and you want to make it available for viewing in a HoloLens, upload the packaged guide. If you work in multiple environments, select the environment in which you want the packaged guide available for viewing.

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. Under **Content**, on the left side of the screen, select **Packaged Guides**.

1. Select **New**.

1. On the **New Packaged Guide** screen, enter the name of the packaged guide, and then select **Save**.

   :::image type="content" source="media/mda-new-packaged-guide.png" alt-text="Screenshot of the New Packaged Guide screen in the model-driven app.":::

1. Select **Choose file** and browse to the .guide file and select it.

   > [!TIP]
   > You can only upload a .guide file.

1. Select **Save**.
