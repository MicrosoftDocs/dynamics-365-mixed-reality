---
author: davepinch
description: As a Guides admin, learn how to activate, deactivate, or delete a guide, packaged guide, or guide content (video, image, or 3D part).
ms.author: davepinch
ms.date: 09/15/2023
ms.topic: how-to
title: Activate, deactivate, or delete a guide in Dynamics 365 Guides (admins)
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Activate, deactivate, or delete a guide in Dynamics 365 Guides (for admins)

If a [guide has been deactivated](pc-app-deactivate-guide.md) in Guides, you can reactivate it. When you reactivate a guide, it immediately becomes available for authors to open or edit in the PC app. You can deactivate a guide or permanently delete it if you're sure that you no longer need it.

If a [packaged guide has been deactivated](package-a-guide.md#manage-a-packaged-guide-in-the-pc-app) in Guides, you can reactivate it. When you reactivate a packaged guide, it immediately becomes available for HoloLens users to view or for [authors to download it](package-a-guide.md#download-a-packaged-guide-in-the-model-driven-app).

You can also activate, deactivate, or delete specific guide content (video, image, or 3D part).

## Activate, deactivate, or delete a guide

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. In the drop-down list above the grid, select **Inactive Guides** to view all the guides that are currently inactive.

    ![Selecting Inactive Guides.](media/active-guides-list.PNG "Selecting Inactive Guides")

    > [!TIP]
    > If there are many guides, use the search box in the upper-right corner of the page, or the letter filters at the bottom of the page, to find the correct guide.

1. Select the check box next to the appropriate guide, and then select **Activate**, **Deactivate**, or **Delete** at the top of the page.

    > [!WARNING]
    > You can't recover a guide if you permanently delete it.

    ![Activate, Deactivate, and Delete buttons.](media/activate-deactivate-delete.PNG "Activate, Deactivate, and Delete buttons")

## Activate, deactivate, or delete a packaged guide

A [packaged guide](package-a-guide.md) can't be opened in the model-driven app. Deleting a packaged guide only deletes the *.guide* file. The original guide isn't impacted.

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. Select **Packaged Guides** on the left side of the screen. Then select **Inactive Guides**.

1. Navigate to the packaged guide file and select it. The record for the packaged guide opens.

1. Select **Activate**, **Deactivate**, or **Delete** at the top of the page.

1. Select **Save**.

## Activate, deactivate, or delete specific guide content (video, image, or 3D part)

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. Under **Content**, on the left side of the screen, select **Images**, **Videos**, or **3D**.

1. In the drop-down list above the grid, select **Inactive 3D Objects**, **Inactive Images**, or **Inactive Videos**, depending on the item you choose in step 2. For example, if you choose **3D** under **Content**, select **Inactive 3D Objects** to view all the objects that are currently inactive.

    ![Inactive 3D objects.](media/deactivate-active-3D-objects.PNG "Inactive 3D objects")

1. Select the check box next to the appropriate object, and then select **Activate**, **Deactivate**, or **Delete** at the top of the page.

    ![Selected objects.](media/deactivate-select-objects.PNG "Selected objects")

## Reactivate specific guide content

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. Under **Content**, on the left side of the screen, select **Images**, **Videos**, or **3D**.

1. Locate and select the deactivated content.

1. Select **Activate** at the top of the screen.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
