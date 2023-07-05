---
author: davepinch
description: Learn how to add a website, email, guide, custom app, or Power Apps link to a step in Microsoft Dynamics 365 Guides to create a seamless workflow for operators.
ms.author: davepinch
ms.date: 03/31/2023
ms.topic: how-to
title: Add a website, email, guide, or app link to a step
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Add a website, email, guide, or app link to a step

Create a seamless workflow for operators by adding a website, email, guide, custom app, or Power Apps link to a Step card in Dynamics 365 Guides. If you configure an action link with a Uniform Resource Identifier (URI) scheme, the HoloLens opens the corresponding app or page when an operator activates the link.

- [**Link**](#add-a-link-to-a-step): Add a link to a step so that operators can view and interact with information outside the guide. For example, connect a sequence of guides, open a website, open a page of the Settings app, or open a custom app that has been installed on the device.
- [**Power Apps link**](#add-a-power-apps-link-to-a-step): Add a Power Apps link to a step. [Power Apps](https://products.office.com/business/microsoft-powerapps) provides low-code tools that teams can use to create custom applications to solve unique business workflows. By combining Guides and Power Apps, you can extend Guides capabilities to create a more seamless end-to-end solution that fits the needs of your operators. For example, you can add a link to an interactive quiz app, an app for reordering parts, or an app that provides the latest status on Internet of Things (IoT) sensors.

    > [!NOTE]
    > To run Power Apps from Guides, operators need a [Power Apps license](https://powerapps.microsoft.com/pricing/). They must also have [permission](/powerapps/maker/canvas-apps/share-app#share-an-app) to view the app that is created in Power Apps.

## Add a link to a step

To add a link to a step, you add an action. You can add one action per step. If a step already includes an action, any new action that you add overwrites the existing action.

1. In the PC Authoring app, go to the appropriate step, and then select the **Action** tab on the right side of the page.
1. Drag the **Link** circle to the **Action** circle in the lower-right corner of the **Step Editor** pane.

    :::image type="content" source="media/website-link-drag-action.PNG" alt-text="Screenshot that shows the Link circle being dragged to the Action circle.":::

1. In the **Link** dialog box that appears, enter information based on the selected action:

    - **Email**: Enter *mailto:* and then the email address.
    - **Guide or step**: [Create and copy a link to a guide or step](pc-app-copy-link-guide-step.md).
    - **Web page**: Enter the web address, starting with *http:* or *https:*.
    - **A HoloLens settings page**: Enter *ms-settings:\<URI\>*, where \<*URI*\> is the [URI of the appropriate settings page for HoloLens](/hololens/settings-uri-list#settings-uris) in the Settings app. For example, enter *ms-settings:bluetooth* to open the Bluetooth settings.
    - **A custom app**: Enter the [registered URI](/windows/uwp/launch-resume/handle-uri-activation) in the format that the app expects.

        > [!NOTE]
        > If a custom app has been registered as the [default handler for a URI](/windows/uwp/launch-resume/handle-uri-activation), an author can open it by specifying a URI in the format that the app expects. Apps can be opened in [kiosk mode](/hololens/hololens-kiosk). Administrators can [use Windows Defender Application Control (WDAC) and Windows PowerShell to allow or block apps on HoloLens 2 devices with Microsoft Intune](/mem/intune/configuration/custom-profile-hololens).

1. Select **Save**.
1. To view, edit, or delete the link, select and hold (or right-click) the **Link** button in the **Step Editor** pane, and then select the appropriate command.

    :::image type="content" source="media/website-link-edit.png" alt-text="Screenshot of the shortcut menu for the Link button, showing the Edit, View, and Delete commands.":::

## Add a Power Apps link to a step

The process of adding a Power Apps link has two steps:

1. Copy the Power Apps link.
1. Add the link to a step in the PC app.

### Copy the Power Apps link

You can link to a published app that was created in Power Apps if you have edit permissions for that app.

1. Open the [Power Apps maker portal](https://make.powerapps.com/).
1. Select the **More Commands** button (**…**) next to the appropriate app, and then select **Edit**.

    ![Screenshot that shows Edit being selected on the More Commands menu.](media/powerapps-home.PNG "Screenshot that shows Edit being selected on the More Commands menu")

1. In the left pane, select **File**, and then select **Share**.
1. Under **Guides Power Apps example**, select **Share**.

    ![Screenshot of the Share button.](media/powerapps-share-button.PNG "Screenshot of the Share button")

1. In the **Share Guides Power Apps example** dialog box, select **Cancel**.

    ![Screenshot of the Cancel button in the Share Guides Power Apps example dialog box.](media/powerapps-cancel-button.PNG "Screenshot of the Cancel button in the Share Guides Power Apps example dialog box")

1. In the **Web link** field, copy the URL.

    ![Screenshot of the Web link field containing the URL for the Power Apps link.](media/powerapps-url.PNG "Screenshot of the Web link field containing the URL for the Power Apps link")

### Add the Power Apps link to a step

To add a Power Apps link to a step, you add an action. You can add one action per step. If a step already includes an action, any new action that you add overwrites the existing action.

1. In the PC Authoring app, go to the appropriate step, and then select the **Action** tab on the right side of the page.
1. Drag the **Power Apps** circle to the **Action** circle in the lower-right corner of the **Step Editor** pane.

    :::image type="content" source="media/powerapps-drag-action.PNG" alt-text="Screenshot that shows the Power Apps circle being dragged to the Action circle.":::

1. In the **Power Apps** dialog box that appears, paste the URL for the Power Apps link, and then select **Save**.
1. To view, edit, or delete the Power Apps link, select and hold (or right-click) the **Power Apps** button in the **Step Editor** pane, and then select the appropriate command.

    :::image type="content" source="media/website-link-edit.png" alt-text="Screenshot of the shortcut menu for the Power Apps button, showing the Edit, View, and Delete commands.":::

## Next steps

- [Step Editor overview](pc-app-step-editor-overview.md)
- [Add an image or video file](pc-app-add-media.md)
- [How to make a great mixed-reality guide](great-guide.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
