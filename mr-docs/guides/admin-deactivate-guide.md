---
author: davepinch
description: As a Guides admin, learn how to activate, deactivate, or delete a guide, packaged guide, or guide content (video, image, or 3D part).
ms.author: davepinch
ms.date: 02/23/2024
ms.topic: how-to
title: Activate, deactivate, or delete a guide in Dynamics 365 Guides (admins)
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Activate, deactivate, or delete a guide in Dynamics 365 Guides

If a [guide has been deactivated](pc-app-deactivate-guide.md) in Guides, you can reactivate it. When you reactivate a guide, it immediately becomes available for authors to open or edit in the PC app. You can deactivate a guide or permanently delete it if you're sure that you no longer need it.

If a [packaged guide has been deactivated](package-a-guide.md#manage-a-packaged-guide-in-the-pc-app) in Guides, you can reactivate it. When you reactivate a packaged guide, it immediately becomes available for HoloLens users to view or for [authors to download it](package-a-guide.md#download-a-packaged-guide-in-the-model-driven-app). It can't be opened or edited in the PC app.

You can also activate, deactivate, or delete specific guide content (video, image, or 3D part). Only admins can delete guides and guide content.

## Prerequisites

- Guides Admin or Author role. Only admins can delete guides and guide content.

## Activate, deactivate, or delete a guide

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. To activate a guide, select **Inactive Guides** in the drop-down list above the grid to view all the guides that are currently inactive.

   To deactivate or delete a guide, select **Active Guides**.

   :::image type="content" source="media/inactive-guides-list.PNG" alt-text="Screenshot that shows selecting Inactive Guides in the Guides model-driven app.":::

    > [!TIP]
    > If there are many guides, use the search box in the upper-right corner of the page, or the letter filters at the bottom of the page, to find the correct guide.

1. Select the check box next to the appropriate guide, and then select **Activate**, **Deactivate**, or **Delete** at the top of the page.

    > [!WARNING]
    > You can't recover a guide if you permanently delete it.

   :::image type="content" source="media/activate-deactivate-delete.PNG" alt-text="Screenshot that shows Activate, Deactivate, and Delete buttons in the Guides model-driven app.":::

1. Confirm your action.

## Activate, deactivate, or delete a packaged guide

A [packaged guide](package-a-guide.md) can't be opened in the model-driven app. Deleting a packaged guide only deletes the *.guide* file. The original guide isn't impacted.

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. Select **Packaged Guides** on the left side of the screen. 

1. To activate a packaged guide, select **Inactive Packaged Guides**.

   To deactivate or delete a packaged guide, select **Active Packaged Guides**.

1. Select the check box next to the appropriate guide, and then select **Activate**, **Deactivate**, or **Delete** at the top of the page.

1. Confirm your action.

## Activate, deactivate or delete specific guide content (video, image, or 3D part)

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. To activate content, select **Inactive 3D Objects**, **Inactive Images**, or **Inactive Videos**.

   To deactivate or delete specific content, select **Images**, **Videos**, or **3D**.

   :::image type="content" source="media/deactivate-active-3D-objects.PNG" alt-text="Screenshot that shows Inactive 3D objects in the Guides model-driven app.":::

1. Select the check box next to the appropriate object, and then select **Activate**, **Deactivate**, or **Delete** at the top of the page.

   :::image type="content" source="media/deactivate-select-objects.PNG" alt-text="Screenshot that shows Activate, Deactivate, and Delete buttons for selected objects in the Guides model-driven app.":::

1. Confirm your action.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
