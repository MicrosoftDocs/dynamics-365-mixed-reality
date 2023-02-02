---
author: Mamaylya
description: Learn how to copy a 3D model's position (orientation and scale) in the Dynamics 365 Guides HoloLens app
ms.author: mamaylya
ms.date: 11/08/2021
ms.topic: article
title: Copy a 3D model's position in the Dynamics 365 Guides HoloLens app
ms.reviewer: v-wendysmith
---

# Copy a 3D model's position in the Dynamics 365 Guides HoloLens app

When working with the Microsoft Dynamics 365 Guides HoloLens app, sometimes you might want to duplicate a 3D model and keep the same position, orientation, and scale for 
different steps of a guide. This is especailly useful for fully digital guides where instructions are placed on top of the holographic versions of a machine that must be 
present and identical for several steps.

## Replicate the 3D position properties (position, orientation, and scale) of a 3D model

1. Select the hologram that has the position, orientation, and scale that you want to copy.

2. Select the **Edit Hologram** (pencil) button.

    ![Edit Hologram button.](media/edit-hologram.png "Edit Hologram button")
 
3. Select **Copy 3D position**. 
 
    ![Copy 3D position command.](media/copy-3D-position.PNG "Copy 3D position command")

    > [!TIP]
    > The 3D position parameters are copied to the Clipboard so you can paste them as many times as you want in the same or a different step or guide. The Clipboard is cleared when you close the HoloLens app.

4. Select the target hologram.

5. Select the **Edit Hologram** button again, and then select **Paste 3D position**.

    ![Paste 3D position command.](media/paste-3D-position.PNG "Paste 3D position command")
 
> [!TIP]
> You can also use voice commands (say **copy 3D position** and **paste 3D position**) to copy a 3D model's position. [See a full list of voice commands that you can use in the HoloLens app](voice-commands.md).

### Using Copy 3D position to reconstruct CAD assemblies

The reference point used by **Copy 3D position** is the pivot point of the object, which might be different from the center of the transparent white-bounding sphere shown for selection and movement purposes. This enables you to rapidly reconstruct Computer-aided Design (CAD) assemblies that you import into Dynamics 365 Guides as separate models and that share the same pivot point. After importing, position, orient, and scale one of the assembly models, and then copy/paste the 3D position onto the other assembly models to reconstruct the whole CAD assembly very quickly. 

## What's next?

- [Get oriented with the HoloLens app](hololens-app-orientation.md)
- [Place and manipulate holograms](hololens-app-place-holograms.md)
- [Add a dotted line for a focus area](hololens-app-dotted-line.md)
- [Use styles for emphasis](hololens-app-styles.md)
- [Duplicate a 3D model](hololens-app-duplicate-model.md)
- [Change animation options](hololens-app-animations.md)
- [Create a trigger for step navigation](hololens-app-trigger.md)
