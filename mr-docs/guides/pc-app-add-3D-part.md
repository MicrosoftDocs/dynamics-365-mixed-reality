---
author: annitachow
ms.author: anchow
description: Learn how to add a custom 3D part to a step in the Microsoft Dynamics 365 Guides PC app. 
ms.date: 07/19/2023
ms.topic: how-to
title: Add a custom 3D part to a step in the Dynamics 365 Guides PC app
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Add a custom 3D part to a step in the Dynamics 365 Guides PC app

You can add 3D parts (models specific to your company) in Microsoft Dynamics 365 Guides by importing them. A 3D part hologram helps operators find a 3D part in the real world. You can use a combination of third-party tools to prepare your 3D computer-aided design (CAD) models. For more information, see [Overview of preparing 3D models](./3d-content-guidelines/overview.md).

1. On the right side of the page, select the **My files** tab.

   :::image type="content" source="media/library-panel.png" alt-text="Screenshot of the right-side pane with the My files tab highlighted.":::

   [!INCLUDE [pc-app-filter-sort](../includes/pc-app-filter-sort.md)]

1. Drag the 3D part that you want to one of the **3D parts** boxes.

    ![Dragging a 3D part to a 3D parts box.](media/drag-3D-part.PNG "Dragging a 3D part to a 3D parts box")

## Import a custom 3D model to use as a 3D part

You can import your own custom 3D models and add them to the **3D parts** library. To import files, you can drag them from a local file folder or use the **Import** command.

> [!TIP]
> You can set animation options (playback speed, direction, and looping) in the HoloLens app.

### Import a file by using a drag-and-drop operation

1. Open Windows File Explorer, and go to the folder that contains the 3D models, images, or videos that you want to import.

1. In the PC app on the right side of the page, select the **My files** tab.

1. Open the folder where you want to import the item.

1. Drag the files to **My files**.

    ![Drag-and-drop animation.](media/drag-drop.gif "Drag-and-drop animation")

### Import a file by using the Import command

1. In the PC app on the right side of the page, select the **My files** tab.

1. Open the folder where you want to import the item.

1. Select **Import** in the lower-right corner of the page.

    ![Import button.](media/import-command.PNG "Import button")

1. Find the files that you want to import, and then select **Open**.

    ![Importing a custom 3D part.](media/import-object.PNG "Importing a custom 3D part")

> [!NOTE]
> If you have trouble importing a custom 3D part, image, or video, [enable Guides to work in the background](known-issues-pc-app.md#cant-upload-3d-content-or-other-assets).

## Next steps

- [Step Editor overview](pc-app-step-editor-overview.md)
- [Add a 3D model from the 3D toolkit](pc-app-add-3D-model.md)
- [Add an image or video file](pc-app-add-media.md)
- [Add a website or Power Apps link](pc-app-website-powerapps-link.md)
- [How to make a great mixed-reality guide](great-guide.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
