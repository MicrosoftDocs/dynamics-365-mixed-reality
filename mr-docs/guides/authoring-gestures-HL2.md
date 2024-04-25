---
author: davepinch
description: Learn how to use HoloLens 2 touch, hand rays, and gaze to navigate and manipulate holograms in Microsoft Dynamics 365 Guides.
ms.author: davepinch
ms.date: 04/24/2024
ms.topic: conceptual
title: HoloLens 2 gestures for authoring and navigating in Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# HoloLens 2 gestures for authoring and navigating in Dynamics 365 Guides

Hand-tracking in Microsoft HoloLens 2 provides instinctual interactions for authors. You can select and position holograms by using direct touch, like they're real objects. You can also use hand rays to interact with holograms that are out of reach.

## Basic actions and gestures to know

To author or navigate in HoloLens 2 and Dynamics 365 Guides, use these actions and gestures:

- **Touch**. Reach out and touch or grab holograms. This approach is the easiest and most intuitive way to author guides. When HoloLens sees your hand, a floating pointer (similar to a mouse pointer) appears near the tip of your index finger to help you target elements.

    ![Touch dwell animation.](media/touch-dwell-animation.gif "Touch dwell animation")

    > [!IMPORTANT]
    > Use touch interaction to work with parts that you've placed in the world. In Dynamics 365 Guides, keep instruction cards (Step cards) out of the way so that they are out of reach for touch interaction.

- **Hand ray**. Hold your hand in front of you, with your palm facing away. A laser pointer (hand ray) appears. After you target an item with your hand ray, you can act on that target in different ways.

    ![Hand ray example.](media/hand-rays-example.PNG "Hand ray example")

- **Gaze**. Select an item or target an object with the HoloLens. If the item has a selection box or circle (gaze/dwell button), select the item by gazing at it. The item is selected when the box or circle is filled. Gaze and air tap are used together often. When you gaze, turn your whole head, not just your eyes. The pointer follows.

    ![Animation of gaze gesture.](media/gaze-fill-2.gif "Animation of gaze gesture")

- **Air tap**. Hold your hand straight out in front of you in a loose fist, point your index finger straight up toward the ceiling, tap down your finger, and then quickly raise it back up again. Air tap is a gesture that's like a "click" with a mouse.

    ![Air tap animation.](media/air-tap-animation.gif "Air tap animation")

- **Air tap and hold**. Start by air tapping, but keep your finger down instead of raising it back up.

### Gesture frame

HoloLens 2 has sensors that can see a few feet to each side of you This area is the gesture frame. When you use gestures, keep them inside that frame. Otherwise, HoloLens doesn't see them. As you move around, the frame moves with you. When your hand is inside the frame, a hand ray appears from your palm. If HoloLens can't see your hands, and you're looking at a user interface (UI) element, the gaze pointer appears in the center of your display.

## Work with close-up UI elements and holograms by using touch

For close-up UI elements and holograms, reach out and touch or grab them with your hands. When your hand gets close enough to touch or grab a hologram, a visual appears around the control to let you know what that control does.

### Select a button

- Push the button with your index finger.

### Select a hologram

- Touch the hologram with your index finger. The controls appear.

    ![Touch dwell animation.](media/touch-dwell-animation.gif "Touch dwell animation")

### Move a hologram

- Grab the large white sphere in the center of the controls with your hands, and move it where you want. The sphere lights up based on where your index finger is in relation to it.

    ![Move a hologram by using touch.](media/touch-move.gif "Move a hologram by using touch")

### Rotate a hologram

- Pinch one of the blue spheres (rotation controls), and rotate it the way that you want. Arrows appear around the rotation controls to show which direction they can be rotated.

    **Left/right rotation**

    ![Rotate right by using touch.](media/touch-rotate-right.gif "Rotate right by using touch")

    **Up/down rotation**

    ![Rotate up and down by using touch.](media/touch-rotate-up-down.gif "Rotate up and down by using touch")

    **Free rotation**

    ![Free rotate by using touch.](media/touch-free-rotate.gif "Free rotate by using touch")

### Change the size of a hologram

- Pinch the blue dial (**Scale** control) on the right side of the part. A slider track appears above and below the **Scale** control to show scaling up or down.

    ![Change the size by using touch.](media/touch-scale-hologram.gif "Change the size by using touch")

### Edit a hologram

- Touch the **Edit hologram** button with your finger, and then touch the command that you want.

    ![Edit a hologram by using touch.](media/touch-edit-menu.gif "Edit a hologram by using touch")

## Work with far-away UI elements and holograms by using hand rays and gaze

Use hand rays to work with UI elements and holograms from a distance. Use gaze to work with the instruction card from a distance. You can't use gaze to manipulate holograms.

> [!TIP]
> When you author a guide, if your hand is visible, hand rays are enabled and gaze is disabled. To use gaze, place your hands at your sides, so that the HoloLens 2 device can't see them.

### Select a button or UI element with a hand ray

1. To target an object, point your hand ray at it.

1. Follow one of these steps:

    - Air tap to select the object.

    - If you see a selection box or circle, hold your hand ray on it until it's selected.

        ![Hand ray dwell on an instruction card animation.](media/hand-ray-dwell-instruction-card-animation.gif "Hand ray dwell on an instruction card animation")

### Manipulate a hologram by using a hand ray

1. To target an object, point your hand ray at it. Controls appear around the hologram.

    ![Hand ray dwell animation.](media/hand-ray-dwell-animation.gif "Hand ray dwell animation")

1. Follow one of these steps:

    - To move the hologram, air tap and hold the hand ray, move the hologram where you want it, and then release.

        ![Hand ray move animation.](media/hand-ray-move-animation.gif "Hand ray move animation")

    - To rotate the hologram, air tap and hold one of the blue spheres, rotate the hologram, and then release.

        **Left/right rotation**

        ![Hand ray rotate left or right animation.](media/hand-ray-rotate-left-right-animation.gif "Hand ray rotate left or right animation")

        **Free rotation**

        ![Hand ray free rotate animation.](media/hand-ray-free-rotate-animation.gif "Hand ray free rotate animation")

    - To change the size of a hologram, air tap and hold the **Scale** control. While you hold the control, move it up or down along the slider track.

        ![Hand ray scale animation.](media/hand-ray-scale-animation.gif "Hand ray scale animation")

    - To edit the hologram, air tap the **Edit** button, and then air tap the selections that you want.

        ![Hand ray edit a hologram animation.](media/hand-ray-edit-hologram-animation.gif "Hand ray edit a hologram animation")

### Select an item on the instruction card by using gaze

1. Put your hands at your sides, and gaze at the button or UI element.

1. Continue to gaze until the button is filled.

   ![Animation of gaze gesture.](media/gaze-fill-2.gif "Animation of gaze gesture")

## Open the Start menu

On HoloLens 2, use either one hand or two hands to open the **Start** menu. If you're ever unsure what to do, a good way to get reoriented is open the **Start** menu.

### Open the Start menu with one hand

1. Hold out one of your hands with the palm facing up, and look at your wrist. You should see a holographic Microsoft Windows logo.

1. With the hand that you're holding out, touch your index finger to your thumb in a pinching motion.

### Open the Start menu with two hands

1. Hold out one of your hands with the palm facing up, and look at your wrist. You should see a holographic Windows logo.

1. With the index finger of your other hand, touch the Windows logo.

    ![Video camera graphic.](media/video-camera.PNG) [Watch a video about opening the Start menu with two hands](https://www.microsoft.com/videoplayer/embed/RE3Wxng)

## Need a tutorial on gestures?

For a tutorial on some basic gestures, open the **Start** menu, and then select **Tips**. This action closes the Dynamics 365 Guides app.

## See also

- [HoloLens 2 gestures for operating (navigating) a guide](operator-gestures-HL2.md)
- [Calibrate your HoloLens 2 device](operator-calibrate-HL2.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
