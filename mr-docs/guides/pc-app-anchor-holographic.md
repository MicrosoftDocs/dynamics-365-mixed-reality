---
author: davepinch
description: Learn how to anchor holograms in the Microsoft Dynamics 365 Guides PC app by using a holographic anchor
ms.author: davepinch
ms.date: 09/15/2023
ms.topic: how-to
title: Anchor your guide in Dynamics 365 Guides by using a holographic anchor
ms.reviewer: mhart
ms.custom: bap-template
---

# Anchor your guide in Dynamics 365 Guides by using a holographic anchor

Use a holographic anchor to anchor your guide to the real world in Guides. Review [best practices for holographic anchors.](pc-app-anchor-holographic-best-practices.md)

> [!NOTE]
> An object anchor created with [object anchors](pc-app-anchor-object.md) is preferred over a holographic anchor when:
> - The target object is [suitable for object detection](pc-app-anchor-object-best-practices.md)
> - Accuracy needs are high
> - The target object is available in the real world to scan with HoloLens
> - Holograms need to be consistently positioned at the same location

## Set up a holographic anchor

You can access the **Anchor** wizard from the **Outline** page in the PC app. The **Outline** page automatically appears after you create or open a guide.

1. On the **Outline** page, select **Set your anchor now**.

    ![Set your anchor now button.](media/outline-page-3.PNG "Set your anchor now button")

1. On the **Choose an anchor method** page, select **Select** for the **Holographic** anchor method.

1. In step 1 of the wizard, select **Create**, find your custom 3D model, and then select **Open** to import it. The model is added to the **My files** tab in the gallery.

    ![Import button.](media/holographic-anchor-import-button.PNG "Import button")

   > [!TIP]
   > The filter is automatically set to **Object anchors**.

1. Drag the 3D model from the **My files** tab to the **Assign holographic anchor** box. The 3D model is assigned as the holographic anchor for the guide. When you've finished, select **Next** to move to the next step.

    ![Assign holographic anchor box.](media/holographic-anchor-drag-model.PNG "Assign holographic anchor box")

1. Put on your HoloLens, open the guide, and then use air tap and hold to move the holographic anchor directly over a physical object in your work environment. If you must rotate the object, use air tap and hold to move the blue spheres.

    ![Blue spheres.](media/blue-spheres-digital-anchor.PNG "Blue spheres")

   > [!TIP]
   > On HoloLens 2, you can use your hand to directly select and place a holographic anchor when you author a guide. For more information, see [HoloLens 2 gestures for authoring and navigating](authoring-gestures-HL2.md).

1. Take a picture of the place where you put the holographic anchor, to help the operator find it.

1. Go back to the PC app, and then select **Next** in the wizard two times. (You can skip step 2 of the wizard if you took a photo of the location in the previous step.)

1. In step 4 of the wizard, select the **Import** button to import the photo that you took in step 6. Then drag it to the **Import photo of anchor location** box. When you've finished, select **Next** to move to the next step.

1. In step 5 of the wizard, if you want to change the default instructions for the operator, select **Edit Step card text**, and then enter your instructions. When you've finished, select **Next** to move to the next step, and then select **Confirm**.

    ![Edit Step card text button.](media/holographic-anchor-operator-instructions.PNG "Edit Step card text button")

## Next steps

- [Best practices for holographic anchors.](pc-app-anchor-holographic-best-practices.md)
- [Anchor a guide in the HoloLens app](hololens-app-anchor.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
