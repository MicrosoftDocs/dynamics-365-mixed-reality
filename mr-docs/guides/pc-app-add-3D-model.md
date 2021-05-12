---
author: Mamaylya
ms.author: mamaylya
description: Learn how to add a 3D model (for example, an arrow or a hand) to a step in the Dynamics 365 Guides PC app. 
ms.date: 05/04/2021
ms.service: crm-online
ms.topic: article
title: Add a 3D model (arrow or hand, for example) to a step in the Dynamics 365 Guides PC app
ms.reviewer: v-bholmes
---

# Add a 3D model from the 3D toolkit to a step in the Dynamics 365 Guides PC app

Microsoft [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] includes a library of predefined 3D objects that are optimized to work perfectly with [!include[pn-hololens](../includes/pn-hololens.md)]. The 3D toolkit includes markers, arrows, hands, numbers, symbols, zones, and generic tools. The following illustration shows an example where holographic numbers, arrows, and zones are used to help operators complete a step.

![Example of holographic numbers, arrows, and zones](media/3d-toolkit-example.PNG "Example of holographic numbers, arrows, and zones")

You can mix and match different types of 3D models. You can also use the same object (instance) as many times as you want in a step.

To add a model from the 3D toolkit, follow these steps.

1. On the right side of the page, select the **3D toolkit** tab, and then select the category for the type of item that you want to add.

    ![3D toolkit tab](media/select-3D-toolkit.PNG "3D toolkit tab")

2. Drag the 3D model that you want to one of the **3D parts** boxes.

    ![Dragging a 3D model to a 3D parts box](media/select-arrow.PNG "Dragging a 3D model to a 3D parts box")
    
3. To preview the model, select (click or double-click) the model in the **Library**.

    ![Properties tab for previewing image, video, or 3D model](media/properties-tab.PNG "Properties tab for previewing image, video, or 3D model")
    
    The image and its properties are displayed on the right side of the screen.   

> [!NOTE]
> You can also add 3D models from the 3D toolkit directly in the [!include[pn-hololens](../includes/pn-hololens.md)] app.

## Best practices for the 3D toolkit

- Use pointers to communicate simple spatial information, such as position, direction, and translation. You can adjust the size of the pointer, but you should never reduce it below 1 cm. Otherwise, errors can occur.

- Use the arrow when you want the operator to insert a part into something stationary (for example, to hand-tighten a bolt into a tapped hole).

- Use one of the hand poses when you want the operator to use his or her hand in a specific way to influence or manipulate something. There are various poses for specific interactions, such as Pull, Push, Pinch, and Grab. Combine these standard poses with arrows and/or icons to add additional meaning.

- You can preview the image or video on the right side of the screen by selecting it (click or double-click) in the **Library**.

For more information about ways to use objects from the 3D toolkit, see [Create a great guide](great-guide.md).

## What's next?

[Step Editor overview](pc-app-step-editor-overview.md)<br>
[Add a 3D part](pc-app-add-3D-part.md)<br>
[Add an image or video file](pc-app-add-media.md)<br>
[Add a website or Power Apps link](pc-app-website-powerapps-link.md)<br>
[How to make a great mixed-reality guide](great-guide.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
