---
author: prashantyvr
ms.author: prashan
description: Learn how to package a guide and its content and share it with others in Dynamics 365 Guides. 
ms.date: 03/04/2024
ms.topic: how-to
title: Package a guide in Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Package a guide in Dynamics 365 Guides

Packaging a guide allows authors to create a self-contained, read-only file that contains a copy of all contents in a guide. Use a packaged guide to archive versions of a guide, easily migrate guides between environments, or quickly share content with others regardless of permission levels. The packaged guide can't be edited and can only be viewed with a HoloLens device in operator mode.

> [!IMPORTANT]
> Verify permissions on guide content before packaging a guide. Packaging a guide creates a copy of all content in a guide and enables you to share everything within that guide regardless of permission levels within the Dynamics 365 environment. Be aware of any sensitive information that might be shared and manage the packaged guide according to your organization's privacy policies.

## Limitations

- Maximum of 2 GB for a packaged guide
- Maximum of 100 MB 3D objects and other assets
- Migrating a combination of packaged and non-packaged guides isn't supported
- Animated anchors aren't supported
- Offline mode isn't supported

## Support across versions

A packaged guide is supported in future versions of the client applications, without the need to repackage it again after updating the versions. For example, if a guide is packaged using version 9.0, users can still open the packaged guide in future client versions such as 9.1 or 10.0. However, if a guide is packaged using a PC app version higher than the HoloLens app version of the user trying to open it, that guide won't open. For example, if a guide is packaged using PC app version 9.2, that guide won't open on HoloLens app version 9.1. The user must update their version.

## Package a guide in the PC app

1. In the PC app, open the guide you want to package and select **Package guide**.

   :::image type="content" source="media/package-guide.png" alt-text="Screenshot that shows the Package guide option.":::

1. Keep the default name or enter a unique name for the package guide. For example, provide the guide name and version number or guide name and status.

1. Select **Package**. The guide and all its contents is downloaded, archived into a *.guide* file, and uploaded to the Guides model-driven app. The packaged guide is listed with other guides on the **Home** page. The packaged guide is available to HoloLens users in operator mode.

   > [!NOTE]
   > Don't exit the app during the packaging process or the packaging will be cancelled.

## Manage a packaged guide in the PC app

A packaged guide can't be opened in the PC app. You can rename, deactivate, or share it with someone in the same environment.

1. In the PC app, select **Home** to view a list of guides.

1. Right-click the packaged guide you want to manage and choose one of the following options:

   - **Rename**: Change the name of the packaged guide.

   - **Deactivate**: Deactivate the packaged guide so it no longer appears in the library. To [reactivate](admin-deactivate-guide.md#activate-deactivate-or-delete-a-packaged-guide) or [permanently delete it](admin-deactivate-guide.md#activate-deactivate-or-delete-a-packaged-guide), contact an admin.

   - **Copy link to this guide**: Copy the link to the packaged guide to share it with someone in the same environment.

## Share a packaged guide with another author in a different environment

If your organization works in multiple environments, the packaged guide must be in the same environment as the HoloLens user wanting to view it. Share the packaged guide with an author in that environment so it can be made available for viewing.

1. [Create a packaged guide](#package-a-guide-in-the-pc-app).

1. [Download the packaged guide](#download-a-packaged-guide-in-the-model-driven-app) and send the author the *.guide* file.

1. Have the author access their environment in the model-driven app and [upload the packaged guide](#upload-a-packaged-guide-in-the-model-driven-app). The packaged guide is available for viewing with a HoloLens in operator mode.

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

If you receive a packaged guide and want to make it available for viewing in a HoloLens, upload the packaged guide. If you work in multiple environments, select the environment in which you want the packaged guide available for viewing.

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. Under **Content**, on the left side of the screen, select **Packaged Guides**.

1. Select **New**.

1. On the **New Packaged Guide** screen, enter the name of the packaged guide, and then select **Save**.

   :::image type="content" source="media/mda-new-packaged-guide.png" alt-text="Screenshot of the New Packaged Guide screen in the model-driven app.":::

1. Select **Choose file** and browse to the *.guide* file and select it.

   > [!TIP]
   > You can only upload a *.guide* file.

1. Select **Save**.
