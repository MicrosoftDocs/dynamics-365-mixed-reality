---
author: annitachow
ms.author: anchow
description: Learn how to add a 3D object (for example, an arrow or a hand) to a step in the Dynamics 365 Guides PC app. 
ms.date: 07/26/2023
ms.topic: how-to
title: Add a 3D object from the toolkit to a step in the Dynamics 365 Guides PC app
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Add a 3D object from the toolkit to a step in the Dynamics 365 Guides PC app

Microsoft Dynamics 365 Guides includes a library of predefined 3D objects that are optimized to work perfectly with HoloLens. The toolkit includes markers, arrows, hands, numbers, symbols, zones, and generic tools. The following illustration shows an example where holographic numbers, arrows, and zones are used to help operators complete a step.

![Example of holographic numbers, arrows, and zones.](media/3d-toolkit-example.PNG "Example of holographic numbers, arrows, and zones")

You can mix and match different types of 3D objects. You can also use the same object (instance) as many times as you want in a step.

> [!NOTE]
> Some toolkit items have built-in animations that you can turn on or off. [Learn more about animation options.](hololens-app-animations.md)

To add a model from the toolkit, follow these steps.

1. On the right side of the page, select the **Toolkit** tab. Then, select the category for the type of item that you want to add.

1. Drag the 3D object from the **Toolkit** tab to one of the **3D parts** boxes.

    ![Screenshot of the Toolkit tab highlighted dragging an arrow.](media/select-3D-toolkit.png "Screenshot of the Toolkit tab highlighted dragging an arrow")

1. To preview the model, select (click or double-click) the model.

    ![Screenshot of the Properties tab.](media/properties-tab.png "Screenshot of the Properties tab")

> [!NOTE]
> You can also add 3D objects from the toolkit directly in the HoloLens app.

## Follow best practices for the toolkit

- Use pointers to communicate simple spatial information, such as position, direction, and translation. You can adjust the size of the pointer, but you should never reduce it below 1 cm. Otherwise, errors can occur.

- Use the arrow when you want the operator to insert a part into something stationary. For example, to hand-tighten a bolt into a tapped hole.

- Use one of the hand poses when you want the operator to use their hand in a specific way to influence or manipulate something. There are various poses for specific interactions, such as Pull, Push, Pinch, and Grab. Combine these standard poses with arrows and/or icons to add more meaning.

- Preview the image or video on the right side of the screen by selecting it (click or double-click) in the **Toolkit** tab.

For more information about ways to use objects from the toolkit, see [Create a great guide](great-guide.md).

## Next steps

- [Step Editor overview](pc-app-step-editor-overview.md)
- [Add a 3D part](pc-app-add-3D-part.md)
- [Add an image or video file](pc-app-add-media.md)
- [Add a website or Power Apps link](pc-app-website-powerapps-link.md)
- [How to make a great mixed-reality guide](great-guide.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
