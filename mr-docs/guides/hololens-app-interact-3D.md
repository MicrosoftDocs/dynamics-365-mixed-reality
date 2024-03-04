---
author: RobertButterworthMS
description: Learn how to make a hologram interactive in the Dynamics 365 Guides HoloLens app.
ms.author: robutter
ms.date: 04/28/2023
ms.topic: how-to
title: Enable operators to interact with holograms in the Guides HoloLens app
ms.reviewer: v-wendysmith
---

# Enable operators to interact with holograms in the Guides HoloLens app

If you want operators to explore a 3D part, use the HoloLens app to place it in the real world, and then set it as interactable.

## Set a 3D part as interactable

1. [Place the 3D object in the real world](hololens-app-place-holograms.md).
1. Air tap the hologram to select it.
1. Air tap the **Edit Hologram** (pencil) button, and select **Interactable**.
1. Enable **Interactable**. A hand icon appears in the middle of the object.

    :::image type="content" source="media/hololens-interactable-select.png" alt-text="Screenshot of the hand icon that appears when the Interactable option is enabled.":::

1. (Optional) Enable **Interactable Ghost** to give the operator a persistent hint for putting the object back into the correct position.

    > [!NOTE]
    > The **Interactable Ghost** option increases the complexity of the step. To learn how you can reduce complexity, go to [Optimize your 3D objects to use with Guides and Power Apps](/dynamics365/mixed-reality/guides/3d-content-guidelines/optimize-models).

To learn how operators work with interactable objects, go to [Interact with holograms in the Guides HoloLens app](operator-holograms.md).

## Tip for using interactable objects

You can make multiple parts of an assembly interactable. In this way, operators learn about the parts by disassembling and reassembling them.

1. In author mode, place multiple parts from the same CAD file into a step, and make each part interactable. To accurately align the parts with each other, place one part where you want it, copy its position, and then paste it to all the other parts.

    :::image type="content" source="media/hololens-interactable-assembled.png" alt-text="Screenshot of assembled equipment, showing several interactable parts.":::

1. In the step card instructions, encourage the operator to pick up the parts and then return them to their original position.

    :::image type="content" source="media/hololens-interactable-author-disassembled.png" alt-text="Screenshot of disassembled equipment, showing several interactable parts.":::

## Next steps

- [Get oriented with the HoloLens app](hololens-app-orientation.md)
- [Place and manipulate holograms](hololens-app-place-holograms.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
