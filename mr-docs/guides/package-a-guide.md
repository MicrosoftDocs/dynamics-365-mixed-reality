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

Packaging a guide creates a copy of all content in a guide that you can share with a user regardless of permission levels. Packaging a guide allows authors to create a self-contained, real-only file that can be shared with others.

<!--- Add benefits --->

The packaged guide can only be viewed by an operator with a HoloLens device.

> [!IMPORTANT]
> Verify permissions on guide content before packaging a guide. Be aware of any sensitive information that might be shared and manage the packaged guide according to your organization's privacy policies.

## Limitations

- Maximum of 2 GB for a packaged guide
- Maximum of 100 MB 3D modesl and other assets, except animated anchors which are not supported
- Maximum of 500 MB to upload to the model-driven app
- Offline mode is not supported

## Package a guide in the PC app

1. In the PC app, open the guide you want to package and select **Package guide**.

   :::image type="content" source="media/package-guide.png" alt-text="Screenshot that shows the Package guide option.":::

1. Name the package guide. For example, provide the guide name and version number or guide name and status.

1. Select **Package**. The guide and all its contents is downloaded and archived into a .guide file

1. Upload the .guide file to the Guides model-driven app. Or is that done automatically?

## Download a packaged guide to share it?

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. Under**Content**, on the left side of the screen, select **Packaged Guides**.

1. Navigate to the packaged guide file and select it. A zip file is downloaded to your downloads folder that you can share with others.

## Manage a packaged guide

A packaged guide can't be opened or managed in the PC app. You can rename, deactivate, or share it from the Guides model-driven app.

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. Select **Packaged Guides**.

1. Right-click the guide you want to manage.
