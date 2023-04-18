---
author: RobertButterworthMS
description: Learn how to use a style to add emphasis (caution, outline, obscure) to a hologram in the Dynamics 365 Guides HoloLens app
ms.author: robutter
ms.date: 04/28/2023
ms.topic: how-to
title: Use a style to add emphasis to a hologram in the Guides HoloLens app
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Use a style to add emphasis to a hologram in the Guides HoloLens app

You can add styles in the Dynamics 365 Guides HoloLens app to provide visual cues for your holograms. For example, add the **Warning** style to indicate caution or the **Red** style to make sure that an operator doesn't do something that could cause harm. As your operators get used to the visual language that styles provide, their learning process speeds up.

## Add a style

1. Select a hologram that you've already placed in the real world.

1. Select the **Edit Hologram** (pencil) button.

   :::image type="content" source="media/edit-hologram.png" alt-text="Screenshot of Edit Hologram button.":::

1. Select **Styles**.

    > [!TIP]
    > On HoloLens 2, you can select the **Styles** command and subsequent menu items directly with your finger. For more information about manipulating holograms in HoloLens 2, see [Authoring and navigating gestures for HoloLens 2](authoring-gestures-HL2.md).

1. Select the style that you want to use.

   :::image type="content" source="media/styles.png" alt-text="Screenshot of List of styles.":::

The styles available in Guides and when to use them include:

| Style | Potential use | How it appears to the operator |
|---|---|---|
| Original | Restore the original appearance. | Default appearance |
| Red | Show areas or things to avoid. | Red flashing |
| Green | Show areas or things to approach. | Green flashing |
| Caution | Warn about a safety or quality concern. | Yellow and black stripes |
| X-ray | Show things that occur inside something. | A pulse that appears through it |
| Outline | Tell the operator to pick something up. | Outline |
| Dashed outline | Show the operator where to place something. | Dotted line |
| Obscure | Cover sensitive objects to block the operator's view. | 90% bright white |
| Pass-through | Cut through holograms to see the real world behind them. | 100% transparent, including objects behind it |
| Metallic | Provide a realistic metal finish for an object. | Metallic |
| 50% transparent | Show something without obscuring the operator's view. | 50% transparent |
| 75% transparent | Layer one thing on top of another so that the operator can see through two layers. | 75% transparent |

The styles from the operator's perspective:

![All styles.](media/all-styles.PNG "All styles")

### Best practices for styles

- Use styles to reinforce actions.

- Be consistent in your styles usage. After operators learn the visual language of styles, they'll know that a particular style means a specific thing, which speeds up their learning process.

## Obscure or highlight items in your space

Use **Obscure** and **Pass-through** styles together to manage what is shared by your HoloLens camera during a call, when recording a video, or taking pictures to share. **Obscure** applies a 90% bright white style to a 3D object, effectively obscuring the real world on the shared view both in front and behind the 3D object. **Pass-through** makes a 3D object transparent for all holograms behind it, passing through holograms and showing the real world to the call participants. Together, these styles can help remote collaborators focus on specific real-world elements and protect other real-world elements.

For example, as an author, you want to obscure a diagram with sensitive information but you want the airplane pylon that's in front of the diagram to always be visible during a call.

:::image type="content" source="media/original-scene.jpg" alt-text="Original image before Obscure and Passthrough applied from an author's view.":::

1. [Create a guide](create-guide.md) with your image.

1. [Place a 3D cube](pc-app-add-3D-model.md) from the 3D toolkit in front of the diagram.

1. Add the **Obscure** style on the 3D object. Anything in front of the diagram will also be obscured.

1. To have the airplane pylon always be visible, place a 3D model of the pylon over the pylon image. Add the **Pass-through** style.

The author view:

   :::image type="content" source="media/obscure-passthrough.png" alt-text="Image with Obscure and Passthrough applied from an author's view.":::

The operator view:

   :::image type="content" source="media/obscure-passthrough-operator.png" alt-text="Image with Obscure and Passthrough applied from an author's view.":::

The guide author has full control over what they obscure from view when on a Teams call or making mixed reality videos, and can assemble a collection of 3D cubes to hide additional environment elements.  In the following example, more 3D cubes were placed to obscure the large whiteboard, the computer, and toolbox as well as the diagram.

## Next steps

- [Get oriented with the HoloLens app](hololens-app-orientation.md)
- [Place and manipulate holograms](hololens-app-place-holograms.md)
- [Add a dotted line for a focus area](hololens-app-dotted-line.md)
- [Change animation options](hololens-app-animations.md)
