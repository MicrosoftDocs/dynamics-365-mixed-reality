---
author: annitachow
ms.author: anchow
description: Learn how to add an image or video to a step in the Microsoft Dynamics 365 Guides PC app to help operators with a complex step.
ms.date: 02/22/2024
ms.topic: how-to
title: Add an image or video to a step in the Dynamics 365 Guides PC app
ms.reviewer: mhart
ms.custom: bap-template
---

# Add an image or video to a step in the Dynamics 365 Guides PC app

As an author, add an image or video in the Dynamics 365 Guides PC app to help an operator with a complex step. For example, add a diagram or a short video to explain a difficult process.

> [!NOTE]
> The PC app converts and resizes videos when they're uploaded to ensure optimal performance on HoloLens. This transcoding process depends on the codecs installed on the PC and errors can occur if codecs are removed from the PC.

1. In the PC app, on the right side of the page, select the **My files** tab.

1. Find and select your image or video.

   [!INCLUDE [pc-app-filter-sort](../includes/pc-app-filter-sort.md)]

1. Drag the image or video to the **Media panel** box.

    ![Screenshot of dragging a file from My files tab to the Media box.](media/select-image-video.png "Screenshot of dragging a file from My files tab to the Media box")

> [!TIP]
> You can preview the image or video on the right side of the screen by selecting it (click or double-click) in the **My files** tab.

## Import an image or video

You can import your own images and videos and add them to **My files** or a folder in **My files**. To import files, you can drag them from a local file folder or use the **Import** command.

[!INCLUDE [import-include](../includes/pc-app-import.md)]

## Change a video thumbnail

When you add a video to a step, the thumbnail for the video is automatically created. If you want to change the thumbnail to an image of your choice, you can use the Guides model-driven app.

1. [Open the Guides model-driven app](open-model-driven-app.md).

1. Open the video that has the thumbnail you want to replace.

1. At the top left of the screen, select the video circle.

   :::image type="content" source="media/model-driven-app-video-change-thumbnail.PNG" alt-text="Screenshot of video in model-driven-app with circle icon highlighted.":::

1. In the **Choose Image** dialog box, select **Upload Image**, and then find the image you want to upload.

    > [!NOTE]
    > The image will automatically update in the model-driven app. To refresh the image in the PC app **Step Editor** page, open the **Outline** page, and then go back to the **Step Editor** page.

## Next steps

- [Step Editor overview](pc-app-step-editor-overview.md)
- [Add a 3D object from the toolkit](pc-app-add-3D-model.md)
- [Add a 3D part](pc-app-add-3D-part.md)
- [Add a website or Power Apps link](pc-app-website-powerapps-link.md)
- [How to make a great mixed-reality guide](great-guide.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
