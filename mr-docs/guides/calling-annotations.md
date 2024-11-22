---
title: Use annotations with Dynamics 365 Guides
description: Learn how to add annotations to a Dynamics 365 Guides HoloLens user's screen.
author: prashantyvr
ms.author: prashan
ms.date: 04/08/2024
ms.topic: how-to
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Use annotations with Dynamics 365 Guides

Annotations are useful for pointing out different parts of your space, including parts that might be difficult to reach. All call participants can see each other's additions, and can make their own annotations. Once an annotation is placed, it remains anchored in your space until the person who placed the annotation deletes it or leaves the call.

If you're using Dynamics 365 Guides and you're on a call with another person or group, you can annotate in your environment in different ways. The primary way to use annotations is through Microsoft Teams.

- If you're on a mobile device and have Microsoft Teams, [use Teams mobile to annotate the environment (preview)](#use-teams-mobile-to-annotate-in-a-users-environment-preview). Teams desktop users (PC or Mac) can annotate in a mobile user's space.
- If you're not on a mobile device but are using a HoloLens, [use your HoloLens to annotate the environment](#use-guides-hololens-to-annotate-in-your-environment).
- If you're using Teams desktop (PC or Mac) and not a HoloLens, [use Teams desktop to annotate the environment](#use-teams-pc-or-mac-to-annotate-the-guides-users-environment).

## Use Teams mobile to annotate in a user's environment (preview)

[!INCLUDE [public-preview-banner-include](../includes/public-preview-banner.md)]

[!INCLUDE [public-preview-banner-note](../includes/public-preview-note.md)]

You can annotate in calls with Microsoft Teams mobile users if you have a Dynamics 365 Guides, Remote Assist, or Field Service license. Microsoft Teams desktop users can annotate in a mobile user's space. Use the **Spatial Annotations** toolbar in Teams to add annotations.

[!INCLUDE [annotations-teams-mobile-include](../includes/annotations-teams-mobile.md)]

<!--- This topic in RA and Field Service. Field Service topic is annotations-teams-mobile.md --->

## Use Guides HoloLens to annotate in your environment

### Prerequisites

- [Enable the annotation permission in Dynamics 365 Guides](hololens-permissions.md)

### Use HoloLens to annotate

If you're using Dynamics 365 Guides on HoloLens, and you're on a call with a remote collaborator using Microsoft Teams (PC, Mac, or mobile) or Dynamics 365 Remote Assist mobile, you and your remote collaborators can annotate in your environment. Call participants can also annotate [shared files or screens](calling-screen-sharing.md).

> [!NOTE]
> A HoloLens user can draw in their environment but can't place arrows. The remote collaborator on Teams or Dynamics 365 Remote Assist mobile can draw **and** place arrows in the Dynamics 365 Guides user's environment.
>
> Annotations don't work well on black or reflective surfaces.

1. When you're on a call, use the **Annotate** toolbar to place arrows or draw in your space.

   :::image type="content" source="media/annotate.png" alt-text="Screenshot of Meeting window and Annotate toolbar.":::

1. Select from the following annotations.

   |Button|Description|
   |---------|----------------------------------------------------|
   |:::image type="icon" source="media/calling-annotations-direct-ink.png":::| Direct ink (draw). Pinch your index finger and thumb to place ink at the tip of your fingers. Lift your index finger from your thumb to stop placing ink.|
   |:::image type="icon" source="media/calling-annotations-far-field-ink.png":::|Draw far away. Use your hand rays to place the cursor where you want to start drawing. Air tap, keep your index finger and thumb together, and then start drawing. Release the air tap to stop drawing.|
   |:::image type="icon" source="media/calling-annotations-color.png":::|Change ink color. Select the **Color** button and then select the color you want. That color will be used the next time that you draw with the Direct ink or Draw far away button.|
   |:::image type="icon" source="media/calling-annotations-teams-undo-button.png":::|Undo the most recent action, including the Erase all action.|
   |:::image type="icon" source="media/calling-annotations-teams-erase-all-button.png":::|Erase all drawings.|

## Use Teams (PC or Mac) to annotate the Guides user's environment

When you join a call in Microsoft Teams (PC or Mac), the Dynamics 365 Guides collaborator’s space displays, including holograms, and you can use the **Mixed Reality** toolbar in Teams to add annotations.

![Screenshot of the Teams mixed reality toolbar.](media/calling-annotations-teams-desktop-mr-toolbar.JPG)

> [!NOTE]
>
> - The toolbar appears only when the video feed for the Dynamics 365 Guides user is active.
> - The toolbar is disabled if the Dynamics 365 Guides user is not ready to receive annotations and files (for example, the user's outgoing video feed is disabled, the user temporarily loses tracking, or Guides is not in the foreground).
> - The toolbar is disabled if the same Guides user is connected from Teams and Dynamics 365 Guides at the same time, regardless of the device used.

### Start annotations

1. To pause the video stream and enter edit mode, choose one of the following actions:

   - Select anywhere in the call window.
   - Select one of the items on the **Mixed Reality** toolbar.
   - Select **Start editing**.

   In edit mode, a live stream of the call displays in the corner of the app window, including the annotations that other call participants add.

1. Use the **Mixed Reality** toolbar to place arrows, draw, or add files in the HoloLens user's space. Each call participant can remove only the annotations that they add. Specific drawings or arrows can’t be removed.

   |Button|Description|
   |---------|----------------------------------------------------|
   |![Graphic showing the Arrow button.](media/calling-annotations-teams-desktop-arrow-button.JPG)|Add an arrow.|
   |![Graphic showing the Ink button.](media/calling-annotations-teams-desktop-ink-button.JPG)|Add ink (draw).|
   |![Graphic showing the Insert file button.](media/calling-annotations-teams-desktop-insert-file-button.JPG)|Insert a file in the HoloLens user's space. You can select an image or .pdf file from OneDrive or from your device. [Learn more about sharing a file.](calling-chat-file-sharing.md)|
   |![Graphic showing the Color button.](media/calling-annotations-teams-desktop-color-button.JPG)|Change the arrow or ink color.|
   |![Graphic showing the Undo button.](media/calling-annotations-teams-desktop-undo-button.JPG)|In edit mode, undo the last action.|
   |![Graphic showing the Erase button, which looks like a trashcan.](media/calling-annotations-teams-desktop-erase-all-button.JPG)|If you're in edit mode, erase all of the annotations made during that editing session. In you're in live mode, erase all of the annotations made during that call.

1. When you're done annotating, select **Stop editing** or select the live video feed in the corner of your screen.

1. To minimize the **Mixed Reality** toolbar and focus on the video stream from the HoloLens user, select the **Mixed Reality Toolbar** button. The toolbar remains minimized if you switch to a different Dynamics 365 Guides user's video feed. To restore the toolbar, select the **Mixed Reality Toolbar** button again.

   ![Screenshot of Mixed Reality Toolbar (HoloLens) button.](media/calling-annotations-teams-desktop-minimize-toolbar.JPG)

[!INCLUDE [footer-include](../includes/footer-banner.md)]
