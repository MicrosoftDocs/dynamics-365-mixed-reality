---
author: annitachow
ms.author: anchow
description: Learn how to add a custom 3D part to a step in the Microsoft Dynamics 365 Guides PC app. 
ms.date: 02/01/2024
ms.topic: how-to
title: Add a custom 3D part to a step in the Dynamics 365 Guides PC app
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Add a custom 3D part to a step in the Dynamics 365 Guides PC app

You can add 3D parts (models specific to your company) in Microsoft Dynamics 365 Guides by importing them. A 3D part hologram helps operators find a 3D part in the real world. You can use a combination of third-party tools to prepare your 3D computer-aided design (CAD) models. For more information, see [Overview of preparing 3D models](./3d-content-guidelines/overview.md).

1. On the right side of the page, select the **My files** tab.

    ![Screenshot of the right-side pane with the My files tab highlighted.](media/library-panel.png "Screenshot of the right-side pane with the My files tab highlighted")

   [!INCLUDE [pc-app-filter-sort](../includes/pc-app-filter-sort.md)]

1. Drag the 3D part that you want to one of the **3D parts** boxes.

    ![Dragging a 3D part to a 3D parts box.](media/drag-3D-part.PNG "Dragging a 3D part to a 3D parts box")

## Import a custom 3D model to use as a 3D part

You can import your own custom 3D models and add them to **My files** or a folder in **My files**. To import files, you can drag them from a local file folder or use the **Import** command.

> [!TIP]
> You can set animation options (playback speed, direction, and looping) in the HoloLens app.

[!INCLUDE [import-include](../includes/pc-app-import.md)]

## View 3D model complexity statistics

On the step, select the 3D model and then select the **Properties** tab. The following statistics appear:

- **Parts**:
- **Triangles**:
- **Vertices**: A vertex is the smallest component of a polygon model. It's a point in a three-dimensional space. You can create a polygon by connecting multiple vertices with edges. These points can be manipulated to create the desired shape.
- **Materials**:
- **Textures**: Textures are two-dimensional image files that are mapped onto the model's 3D surface. Textures can range in complexity from a simple, flat color texture to photorealistic surface detail.
- **Texture size**: Size is measured in megapixel (MP).

If the 3D model exceeds the recommended limits for optimal performance on the HoloLens, a warning appears on the step. Make the necessary changes to the model. Learn more: [Optimize your 3D models](/3d-content-guidelines/optimize-models.md).

## Next steps

- [Step Editor overview](pc-app-step-editor-overview.md)
- [Add a 3D model from the toolkit](pc-app-add-3D-model.md)
- [Add an image or video file](pc-app-add-media.md)
- [Add a website or Power Apps link](pc-app-website-powerapps-link.md)
- [How to make a great mixed-reality guide](great-guide.md)

[!INCLUDE [footer-include](../includes/footer-banner.md)]
