---
author: Mamaylya
description: Learn how to place and manipulate holograms in the Dynamics 365 Guides HoloLens app
ms.author: mamaylya
ms.date: 11/08/2021
ms.topic: article
title: Place and manipulate holograms in the Dynamics 365 Guides HoloLens app
ms.reviewer: v-wendysmith
---

# Place and manipulate holograms in the Dynamics 365 Guides HoloLens app

After [creating a guide with the PC app](create-guide.md) in Microsoft Dynamics 365 Guides, the next step in the authoring process is to place the holograms in your real-world 
environment. During this stage of the process, you'll walk through each step in your guide and place any assets that you associated with that step when you authored 
it in the PC app. For example, if you added a 3D part to help operators with a step, you'll place that part over its physical counterpart in the real world. If you 
added a 3D object from the toolkit (for example, an arrow or a number), you'll place that object in an appropriate place where it can draw the 
user's attention. You can place the same 3D part or 3D object as many times as you want.

> [!NOTE]
> You don't have to do anything to place an image or video that you added in the PC app. Images and videos automatically appear when the operator goes to the step.

## Place a 3D part

1. In the bin, air tap the 3D part that you want to place.

2. Use gaze and gestures to place the 3D part hologram over its counterpart in the real world. [Learn how to manipulate holograms](#manipulate-holograms).

## Place a 3D model from the toolkit

If you added a 3D model to the bin in the PC app, you can place the 3D model in the same way that you place a 3D part. You can also add a 3D model directly from the [!include[pn-hololens](../includes/pn-hololens.md)] app (you don't have to add it in the PC app first).

1. Air tap one of the **Add** boxes in the bin.

2. Air tap a category (for example, **Arrows** or **Hands**), and then air tap the specific 3D model that you want to add.

    ![Categories.](media/step-card-arrow.jpg "Categories")

    The item is added to your bin. You can then place it in the same way that you place any 3D part.
    
> [!TIP]
> Learn about tips for [pointing at small, closely spaced objects in the real world](). 

## Memory constraints when adding 3D models

When you author each guide step, you'll see a warning if the step complexity will likely result in a poor experience for the operator of the guide. 

![Screenshot of warning message.](media/step-content-warning.jpg "Screenshot of warning message")

If you see the "Warning! High step memory usage" message, the 3D models that you place for the step will be displayed but the operator may have a degraded experience (the guide may have low frame rates or there may be noticeable loading times when moving between steps). 

If you continue to add 3D models and HoloLens reaches its memory limit, you'll see the "Step content failed to load" message.

![Screenshot of Step content failed to load message.](media/step-content-failed-load.jpg "Screenshot of Step content failed to load message")

You can't place any additional 3D models at this point. If a model was previously placed in the world, it will be represented as an exclamation point icon to authors and operators. 

![Screenshot of exclamation point icon.](media/exclamation-point-icon.jpg "Screenshot of exclamation point icon")

The exclamation point will also appear next to the model on the parts shelf to let you know that it failed to load and can't be placed.

![Screenshot of exclamation point next to model.](media/exclamation-point-model.jpg "Screenshot of exclamation point next to model")

For information on reducing step complexity, see [Optimize your 3D models to use with Dynamics 365 Guides and Power Apps](/dynamics365/mixed-reality/guides/3d-content-guidelines/optimize-models).

## Best practices for working with 3D content

- Make sure that the 3D content isn't in the way of the operator who is doing the task.

- Keep the field of vision in mind when you place your holograms. If you put a hologram behind someone, it will be very hard to find.

- Use 3D content sparingly and for a clear purpose. Too much content can clutter the instructions and make them harder to follow.

- Remember that you can attach a dotted line to 3D content to make it more discoverable.

## Manipulate holograms 

To place a 3D model from one of your bins, follow these steps.

1. Air tap a 3D model to add it to the real world. It will appear in front of the Step card in your world.

2. Raise your hand in the ready gesture and gaze at the model to preview it. To place a model, you must look at the model **and** put your hand up into the ready position. You'll know that the model is in a preview state when the 3D controls appear around it.

    > [!TIP]
    > If you put your hand down, the 3D controls disappear. This is a good way to view the holograms by themselves without the controls getting in the way. 

3. While the 3D controls are visible:

    1. Air tap and hold anywhere on the move control. 

    2. Move the model where you want it to go, and then release to place it.

    When you tap a 3D model to move it, you select it at the same time. After a 3D model is selected, if you put your hand down, the 3D controls will remain until you preview or select another part, or until you air tap somewhere in empty space.

> [!TIP]
> On [!include[pn-hololens](../includes/pn-hololens.md)] 2, you can manipulate holograms directly with your hands. To select a hologram, place your hand on it to show the 3D controls. Then grab the hologram, move it, and release to place it. When you've finished, air tap anywhere in an empty space. For more information about how to manipulate holograms in HoloLens 2, see [Authoring and navigating gestures for HoloLens 2](authoring-gestures-HL2.md).

### Rotate a hologram

It's unlikely that an asset will be correctly oriented when you first place or move it. You can use the rotation controls to rotate it the way that you want.

To rotate a hologram:

- Air tap and hold a rotation control, and then follow one of these steps:

    - Use the up/down sphere to rotate vertically.

    - Use the left/right sphere to rotate horizontally.

    - Use the free-hand sphere to rotate in any direction.

    > [!TIP]
    > You can gaze at any sphere to determine rotation direction.

    When you're using a rotation control, it's helpful to imagine that you're physically grabbing the sphere and rotating around the object, like a wheel.

The following illustrations show how to use the different rotation controls.

**Free rotation**

![Free rotation.](media/free-rotation.PNG "Free rotation")

**Left/right rotation**

![Left/right rotation.](media/left-right-rotation.PNG "Left/right rotation")

**Up/down rotation**

![Up/down rotation.](media/up-down-rotation.PNG "Up/down rotation")

> [!TIP]
> On [!include[pn-hololens](../includes/pn-hololens.md)] 2, you can operate the rotation controls with your hands. Pinch one of the available rotation controls with your hand, and then rotate the hologram the way that you want. For more information on manipulating holograms in HoloLens 2, see [Authoring and navigating gestures for HoloLens 2](authoring-gestures-HL2.md).

## Change the size of a hologram after you place it

- Air tap and hold the **Scale Hologram** control, and then move your hand up or down.

    ![Scale Hologram control.](media/scale-hologram.png "Scale Hologram control")

    > [!TIP]
    > On [!include[pn-hololens](../includes/pn-hololens.md)] 2, you can pinch the **Scale Hologram** control with your hand, and then move it up or down to change the size of the hologram.

## What's next?

- [Get oriented with the HoloLens app](hololens-app-orientation.md)
- [Add a dotted line for a focus area](hololens-app-dotted-line.md)
- [Use a style to add emphasis](hololens-app-styles.md)
- [Duplicate a 3D model](hololens-app-duplicate-model.md)
- [Copy a 3D model's position](hololens-app-copy-3D-model-position.md)
- [Change animation options](hololens-app-animations.md)
- [Create a trigger for step navigation](hololens-app-trigger.md)
    
[!INCLUDE[footer-include](../includes/footer-banner.md)]
