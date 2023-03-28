---
author: davepinch
description: Learn how to add a website, email, guide, custom app or Power Apps link to a step in Microsoft Dynamics 365 Guides to create a seamless workflow for operators.
ms.author: davepinch
ms.date: 03/28/2023
ms.topic: article
title: Add a website, email, or an app link to a step
ms.reviewer: v-wendysmith
---

# Add a website, email, guide, or an app link to a step

You can add a website link, email, guide, custom app, or a Power Apps link to a Step card in Dynamics 365 Guides creating a seamless workflow for operators. Configure an action link with a Uniform Resource Identifier (URI) scheme so when an operator activates the link, the HoloLens opens the corresponding app or page.  For example, connect a sequence of guides, launch a website, launch a page of the Settings app, or launch a custom app that has been installed on the device.

- **Link.** Add a link to a step so that operators can see and interact with information outside the particular guide.

- **Power Apps link.** [Power Apps](https://products.office.com/business/microsoft-powerapps) enables teams to create custom applications with low-code tools to solve unique business workflows. By combining Guides and Power Apps, you can extend Guides capabilities to create a more seamless end-to-end solution that fits the needs of your operators. For example, you can add a link to an interactive quiz app, a parts re-ordering app, or an app that provides the latest status on IoT sensors.  

   > [!NOTE]
   > To run Power Apps from Guides, operators need a [Power Apps license](https://powerapps.microsoft.com/pricing/). They must also have [permission](/powerapps/maker/canvas-apps/share-app#share-an-app) to view the app that is created in Power Apps.

## Add a link to a step

To add a link to a step, you add an action. You can add one action per step. If a step already includes an action, any new action that you add overwrites the existing action.

1. On the right side of the page, select the **Action** tab.

    ![Action tab.](media/powerapps-action-tab.PNG "Action tab")

1. Drag the **Link** circle to the **Action** circle in the lower-right corner of the **Step Editor** pane.

    ![Dragging the Link circle to the Action circle.](media/website-link-drag-action.PNG "Dragging the Link circle to the Action circle")

1. In the **Link** dialog box that appears, enter the corresponding information based on the selected action:

   - Link to a custom app: Enter the [registered URI](/windows/uwp/launch-resume/handle-uri-activation) in the format expected by the app.
   - Link to an email: Enter **mailto:** and the email address.
   - Link to a guide or step: [Create and copy a link to a guide or step](pc-app-copy-link-guide-step.md).
   - Link to a web page: Enter the web address starting with **http:** or **https:**.
   - Open a HoloLens settings page: Enter **ms-settings:{[URI](/hololens/settings-uri-list#settings-uris)}**, for example **ms-settings:bluetooth** to open the Bluetooth settings.

1. Select **Save**.

1. To view, edit, or delete the link, right-click the **Link** button in the **Step Editor** pane, and then select the appropriate command.

    ![Website link button.](media/powerapps-menu.PNG "Website link button")

## Add a Power Apps link to a step

Adding a PowerApps link requires two steps:

1. Copy the Power Apps link.

2. Add the link to a step in the PC app.

### Copy the Power Apps link

You can link to a published app created in Power Apps if you have edit permissions for that app. 

1.	Go to <https://make.powerapps.com>.

2.	Select the **More Commands** button (**…**)  next to the appropriate app, and then select **Edit**.

     ![Edit button.](media/powerapps-home.PNG "Edit button")
 
3.	In the left pane, select **File**, and then select **Share**.      
 
4.	Under **Guides Power Apps example**, select **Share**.

     ![Share button.](media/powerapps-share-button.PNG "Share button")

5.	In the **Share Guides Power Apps example** dialog box, select **Cancel**.

     ![Cancel button.](media/powerapps-cancel-button.PNG "Cancel button")

6.	In the **Web link** field, copy the URL. 

     ![Power Apps web link.](media/powerapps-url.PNG "Power Apps web link")

### Add a Power Apps link to a step 

To add a Power Apps link to a step, you add an action. You can add one action per step. If the step already includes an action, any new action that you add (regardless of whether it's a website link or a Power Apps link) overwrites the existing action.

1.	In the PC Authoring app, go to the appropriate step, and then select the **Action** tab.

     ![Action tab.](media/powerapps-action-tab.PNG "Action tab")

2.	Drag the **Power Apps** circle to the **Action** circle in the lower-right corner of the **Step Editor** pane.

     ![Drag Power Apps.](media/powerapps-drag-action.PNG "Drag Power Apps")
     
3.	In the **Power Apps** dialog box that appears, paste the URL for the Power Apps link, and then select **Save**.

     ![Power Apps web link pasted.](media/powerapps-paste-url.PNG "Power Apps web link pasted")

4.	To view, edit, or delete the Power Apps link, right-click the **Power Apps** button in the **Step Editor** pane, and then select the appropriate command.

     ![Power Apps menu.](media/powerapps-menu.PNG "Power Apps menu")
     
## What's next?

- [Step Editor overview](pc-app-step-editor-overview.md)
- [Add a 3D model from the 3D toolkit](pc-app-add-3D-model.md)
- [Add a 3D part](pc-app-add-3D-part.md)
- [Add an image or video file](pc-app-add-media.md)
- [How to make a great mixed-reality guide](great-guide.md) 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
