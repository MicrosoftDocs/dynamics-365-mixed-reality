---
title: Use annotations with Dynamics 365 Guides
author: Mamaylya
description: Learn how to add annotations to a Dynamics 365 Guides HoloLens user's screen
ms.author: mamaylya
ms.date: 04/03/2023
ms.topic: how-to
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Use annotations with Dynamics 365 Guides

If you're using Dynamics 365 Guides on HoloLens, and you're on a call with a remote collaborator using Microsoft Teams (PC, Mac, or mobile) or Dynamics 365 Remote Assist mobile, you and your remote collaborators can annotate in your environment. Annotations are useful for pointing out different parts of your space, including parts that may be difficult or dangerous to reach. All call participants can see each others’ additions, and can make their own annotations. Once an annotation is placed, it remains anchored in your space until the person who placed the annotation deletes it or leaves the call. Call participants can also annotate [shared files or screens](calling-screen-sharing.md).

Any user on Teams (PC or Mac) or Dynamics 365 Remote Assist mobile can annotate the environment of the Dynamics 365 Guides user on HoloLens in a one-to-one or group call. Teams mobile users can also annotate, but only for one-to-one calls. Annotations are not supported for users on Teams Web.

## Prerequisites

- [Enable the annotation permission in Dynamics 365 Guides](hololens-permissions.md).

## Use Guides HoloLens to annotate in your environment

> [!NOTE]
> A HoloLens user can draw in their environment but can't place arrows. The remote collaborator on Teams or Dynamics 365 Remote Assist mobile can draw **and** place arrows in the Dynamics 365 Guides user's environment.
>
> Annotations don't work well on black or reflective surfaces.

### Draw in your space

1. When you're on a call, select the **Direct ink** button on the **Annotate** toolbar.

   :::image type="content" source="media/calling-annotations-direct-ink.png" alt-text="Screenshot of Meeting window and Annotate toolbar with focus on Direct ink tool.":::

1. Pinch your index finger and thumb to place ink at the tip of your fingers.

1. Lift your index finger from your thumb to stop placing ink.

### Draw far away

1. When you're on a call, select the **Far-field ink** button on the **Annotate** toolbar.

   :::image type="content" source="media/calling-annotations-far-field.png" alt-text="Screenshot of Annotate toolbar with focus on Far field ink tool.":::

1. Use your hand rays to place the cursor where you want to start drawing.

1. Air tap, keep your index finger and thumb together, and then start drawing in your space. Release the air tap to stop drawing.

### Change ink color

- Select the **Color** button on the **Annotate** toolbar, and then when the **Annotate** toolbar flips over, select the color you want. That color will be used the next time that you draw with the **Direct ink** or **Far-field ink** button.

   :::image type="content" source="media/calling-annotations-drawing-example.png" alt-text="Screenshot showing color ink choices.":::

### Erase your annotations

Use the following buttons to erase your annotations

|Button|Description|
|---------|----------------------------------------------------|
|![Screenshot of Erase all button.](media/calling-annotations-teams-erase-all-button.JPG)|Erase all drawings.|
|![Screenshot of Undo button.](media/calling-annotations-teams-undo-button.JPG)|Undo your most recent action, including the Erase all action.

## Use Teams (PC or Mac) to annotate the Guides user's environment

When you join a call in Microsoft Teams, you'll see your Dynamics 365 Guides collaborator’s space, including holograms, and can use the **Mixed Reality** toolbar in Teams to add annotations.

![Screenshot of the Teams mixed reality toolbar.](media/calling-annotations-teams-desktop-mr-toolbar.JPG)

> [!NOTE]
> - The toolbar appears only when the video feed for the Dynamics 365 Guides user is active.
> - The toolbar is disabled if the Dynamics 365 Guides user is not ready to receive annotations and files (for example, the  user's outgoing video feed is disabled, the user temporarily loses tracking, or Guides is not in the foreground because the user did the Bloom gesture).
> - The toolbar appears if the same Guides user is connected from Teams and Dynamics Guides at the same time, regardless of the device used.
> - The toolbar doesn't appear if you have not turned on the [new Microsoft Teams meeting experience](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/new-meeting-and-calling-experience-in-microsoft-teams/ba-p/1537581).

### Start annotations

1. Do one of the following to pause the video stream and enter edit mode:

   - Select anywhere in the call window.

   - Select one of the items on the **Mixed Reality** toolbar.

   - Select **Start editing**.

   In edit mode, you'll see a live stream of the call in the corner of the app window, including the annotations that other call participants add.

1. Use the **Mixed Reality** toolbar to place arrows, draw, or add files in the HoloLens user's space. Each call participant can only remove the annotations that they add. Specific drawings or arrows can’t be removed.

   |Button|Description|
   |---------|----------------------------------------------------|
   |![Graphic showing the Arrow button.](media/calling-annotations-teams-arrow-button.JPG)|Add an arrow.|
   |![Graphic showing the Ink button.](media/calling-annotations-teams-ink-button.JPG)|Add ink (draw).|
   |![Graphic showing the Insert file button.](media/calling-annotations-teams-insert-file-button.JPG)|Insert a file in the HoloLens user's space. You can select an image or .pdf file from OneDrive or from your device. [Learn more about sharing a file](calling-chat-file-sharing.md)|
   |![Graphic showing the Color button.](media/calling-annotations-teams-color-button.JPG)|Change the arrow or ink color.|
   |![Graphic showing the Undo button.](media/calling-annotations-teams-undo-button.JPG)|In edit mode, undo the last action.|
   |![Graphic showing the Erase button, which looks like a trashcan.](media/calling-annotations-teams-erase-all-button.JPG)|If you're in edit mode, erase all of the annotations made during that editing session. In you're in live mode, erase all of the annotations made during that call.

1. When you're done annotating, select **Stop editing** or select the live video feed in the corner of your screen.

1. To minimize the **Mixed Reality** toolbar and focus on the video stream from the HoloLens user, select the **Mixed Reality Toolbar** button. The toolbar remains minimized if you switch to a different Dynamics 365 Guides user's video feed. To restore the toolbar, select the **Mixed Reality Toolbar** button again.

   ![Screenshot of MR Toolbar (HoloLens) button.](media/calling-annotations-teams-desktop-minimize-toolbar.JPG)

## Use Teams mobile to annotate the Guides user's environment

You can only annotate in one-to-one calls with Teams mobile. Use the **Mixed Reality** toolbar in Teams to add annotations.

1. Select the **Ink button**. The Guides user's video feed freezes.

   ![Screenshot of the Mixed Reality toolbar, with the Ink button selected.](media/calling-annotations-teams-mobile-mr-toolbar.JPG)

1. Use the **Mixed Reality** toolbar to place arrows, draw, or add files in the HoloLens user's space.

   |Button|Description|
   |---------|----------------------------------------------------|
   |![Graphic of the Place arrow icon in the mixed reality toolbar.](media/calling-annotations-teams-arrow-button.JPG)| Add an arrow. To add an arrow, tap where you want to place the arrow. To control the direction of the arrow, tap, hold, and draw a circle with your finger until it's facing the desired direction. Release to lock the arrow in place.|
   |![Graphic of the Ink button, as represented by a pencil.](media/calling-annotations-teams-ink-button.JPG)|Add ink (draw).|
   |![Graphic of the Color button.](media/calling-annotations-teams-color-button.JPG)|Change the arrow or ink color.|
   |![Graphic showing the Undo button.](media/calling-annotations-teams-undo-button.JPG)|Undo your last action in edit mode or undo the most recent annotation you added.|
   |![Graphic showing the erase icon, which looks like a trash can.](media/calling-annotations-teams-erase-all-button.JPG)|To delete all annotations that you added, select this button, and then select **Delete All Notes**. To delete only the annotations you added recently, select this button, and then select **Clear Current Notes**. This does not clear the annotations your collaborator added.

   > [!NOTE]
   > Each call participant can only undo and delete their own annotations.

1. When you’re done annotating, select the **Checkmark** button on the **Mixed Reality** toolbar to resume the live video feed. All annotations persist even after you stop editing.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
