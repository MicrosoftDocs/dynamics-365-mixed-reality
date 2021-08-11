---
author: v-mhoag
description: Learn how to enable calling within a Dynamics 365 Guides environment 
ms.author: v-mhoag
ms.date: 08/07/2021
ms.topic: article
title: Enable calling for an environment in Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# Enable calling in a Dynamics 365 Guides Environment 

When enabled, a Dynamics 365 Guides HoloLens user can make a one-to-one call. Remote collaborators can join the call using Microsoft Teams desktop application or mobile application.  In a call, remote collaborators can see everything seen by the Hololens user – including holograms and the real world behind the holograms.

If you're an admin or an author for Microsoft Dynamics 365 Guides, you can enable or disable  calling for all guides accessed by a user within a Dynamics 365 Guides Environment.  Enabling or disabling calling by environment is useful to manage when operators or authors do not need to work with remote collaborators.  Or if it is preferred that HoloLens users are not able to start a call and allow remote collaborators to see everything that they see while working in Dynamics 365 Guides.  

## Settings

1. Sign in to the instance by using your admin or author credentials.

    > [!TIP]
    > To find the URL for the instance, select the **Analyze** tab in the PC app. The URL is shown in the **Instance URL** field at the bottom of the page. Copy this URL, and paste it into the address bar of your web browser.
    >
    > ![Instance URL field.](media/instance-url.PNG "Instance URL field")

2. In Power Apps, select the **Guides** app tile.

    ![Guides app tile.](media/guides-app-tile.PNG "Guides app tile")
    
3.	In the left pane, use the area picker to select **Settings** to view all setting for the instance.

    ![Area picker selector highlighted in the left pane.](media/Admin-EnableCalling01--BackGround-GuidesMDA-AreaPicker-Settings.PNG "Area picker selector  highlighted in left pane")

4.	At the top of the screen, select **New** to create a new folder.

    ![New command highlighted at top of Power Apps screen.](media/folders-new.PNG "New command highlighted at top of Power Apps screen") 

5.	Enter the name and owner of the folder. You can select an existing folder in the **Parent Folder** field, or leave the **Parent Folder** field blank to create a folder at the root level.

6.	At the top of the screen, select **Save & Close** to save the folder and return to the folder list. After saving, you can add guides and subfolders to the folder.

## Add a guide to a folder

1.	In the left pane, select **Guides**, and then locate the guide you want to add to the folder.    

2.	On the **General** tab, in the **Parent Folder** field, enter the parent folder name or search for it.

    ![General tab and Parent Folder field highlighted.](media/folders-general-tab.PNG "General tab and Parent Folder field highlighted")

3.	At the top of the screen, select **Save** or **Save & Close**.

> [!TIP]
> To move a guide back to the root folder, return to the guide details and delete the contents of the **Parent Folder** field.

## Change the owner of a folder

When you change the owner of a folder, any guides or subfolders within that folder will be assigned to that owner. This allows you to easily manage access for a group of related guides.

To change the owner of a folder:

1.	In the left pane, select **Folders** to view the list of folders in the instance.

2.	Go to the desired folder, and then at the top of the screen, select **Assign** to display the folder information.

    ![Assign command highlighted at top of screen.](media/folders-assign.PNG "Assign command highlighted at top of screen")

3.	In the **Assign Folder** dialog box, select the box to the right of the **Assign to** label to toggle between **Me** and **User or team**. If **Me** is selected, the folder is assigned to you. If **User or team** is selected, you can enter the owner in the **User or team** field or search for an owner.

    ![Assign Folder dialog box.](media/folders-assign-to.PNG "Assign Folder dialog box")



4.	Select **Assign** to save the new owner. 

## See also

[Create or find a guide](create-guide.md)

[Move your folder structure from one environment to another](admin-export-import-folders.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
