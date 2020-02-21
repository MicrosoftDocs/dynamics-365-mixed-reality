---
author: Mamaylya
description: Learn how to add a website or Power Apps link to a step in Dynamics 365 Guides to create a seamless workflow for operators
ms.author: mamaylya
ms.date: 02/25/2020
ms.service: crm-online
ms.topic: article
title: Add a website or Power Apps link to a step in Dynamics 365 Guides
ms.reviewer: v-brycho
---

# XAdd a website or Power Apps link to a step in Dynamics 365 Guides

You can use add a website link or a [!include[pn-powerapps](../includes/pn-powerapps.md)] link to a Step card in [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)].

- **Website link.** Add a website link to a step so that operators can see and interact with information outside of [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. For example, you might want to provide a link to a parts diagram, parts inventory system, analytics dashboard, or information about Internet of Things (IoT) sensors. Website links let authors create a seamless workflow for operators.

- **[!include[pn-powerapps](../includes/pn-powerapps.md)] link.** [Power Apps](https://products.office.com/en-us/business/microsoft-powerapps) enables teams to create custom applications with low-code tools to solve unique business workflows. By combining [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] and [!include[pn-powerapps](../includes/pn-powerapps.md)], you can extend [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] capabilities to create a more seamless end-to-end solution that fits the needs of your operators. For example, you can add a link to an interactive quiz app, a parts re-ordering app, or an app that provides the latest status on IoT sensors.  

   >[!NOTE]
   >Operators need a [Power Apps license](https://powerapps.microsoft.com/en-us/pricing/) to run [!include[pn-powerapps](../includes/pn-powerapps.md)] from [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. Operators must also have [permission](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/share-app#share-an-app) to view the app created in [!include[pn-powerapps](../includes/pn-powerapps.md)].

## Add a website link to a step

To add a website link to a step, you add an action. You can add one action per step. If the step already includes an action, adding a new action (whether it's a website link or [!include[pn-powerapps](../includes/pn-powerapps.md)] link) overwrites the existing action. 

1. On the right side of the page, select the **Action** tab.

    ![Action tab](media/powerapps-action-tab.PNG "Action tab")
 
2. Drag the **Website link** circle to the **Action** circle in the lower-right corner of the **Step Editor**.

    ![Dragging the Website link symbol to the Action circle](media/website-link-drag-action.PNG "Dragging the Website link symbol to the Action circle")

3. In the **Website link** dialog box, enter a valid URL that begins with **http://** or **https://**, and then select **Save**.

    ![Website link dialog box](media/website-dialog.PNG "Website link dialog box")

4. To view, edit, or delete the link, right-click the **Website link** button in the **Step Editor**, and then select the appropriate command.

    ![Website link button](media/powerapps-menu.PNG "Website link button")

## Add a Power Apps link to a step

Adding a PowerApps link requires two steps:

- Copy the [!include[pn-powerapps](../includes/pn-powerapps.md)] link

- Add the link to a step in the PC app

### Copy the Power Apps link

You can link to a published app created in [!include[pn-powerapps](../includes/pn-powerapps.md)] if you have edit permissions for that app. 

1.	Go to https://make.powerapps.com.

2.	Select **More Commands (…)** next to the appropriate app, and then select **Edit**.

     ![Edit button](media/powerapps-home.PNG "Edit button")
 
3.	In the left pane, select **File**, and then select **Share**.      
 
4.	Under **Guides [!include[pn-powerapps](../includes/pn-powerapps.md)] example**, select the **Share** button.

     ![Share button](media/powerapps-share-button.PNG "Share button")

5.	In the **Share Guides [!include[pn-powerapps](../includes/pn-powerapps.md)] example** screen, select **Cancel** in the lower-right corner.

     ![Cancel button](media/powerapps-cancel-button.PNG "Cancel button")

6.	In the **Web link** field, copy the URL. 

     ![Power Apps web link](media/powerapps-url.PNG "Power Apps web link")

### Add a Power Apps link to a step 

To add a [!include[pn-powerapps](../includes/pn-powerapps.md)] link to a step, you add an action. You can add one action per step. If the step already includes an action, adding a new action (whether it's a website link or [!include[pn-powerapps](../includes/pn-powerapps.md)] link) overwrites the existing action. 

1.	Open the PC Authoring app, go to the appropriate step, and then select the **Action** tab.

     ![Action tab](media/powerapps-action-tab.PNG "Action tab")

2.	Drag the **[!include[pn-powerapps](../includes/pn-powerapps.md)]** circle to the **Action** circle in the lower-right corner of the **Step Editor**.

     ![Drag Power Apps](media/powerapps-drag-action.PNG "Drag Power Apps")
     
3.	In the **[!include[pn-powerapps](../includes/pn-powerapps.md)]** dialog box that appears, paste the [!include[pn-powerapps](../includes/pn-powerapps.md)] link, and then select **Save**.

     ![Power Apps web link pasted](media/powerapps-paste-url.PNG "Power Apps web link pasted")

4.	To view, edit, or delete the [!include[pn-powerapps](../includes/pn-powerapps.md)] link, right-click the **[!include[pn-powerapps](../includes/pn-powerapps.md)]** button in the **Step Editor**, and then select the appropriate command.

     ![Power Apps menu](media/powerapps-menu.PNG "Power Apps menu")
     
## See also?

[Open a website from the Step card (for operators)](operator-orientation#access-a-website-that-is-linked-from-the-step-card)<br>
[Launch an app created in Power Apps from the Step card (for operators)](operator-orientation#launch-an-app-created-in-power-apps-from-the-step-card)

 
