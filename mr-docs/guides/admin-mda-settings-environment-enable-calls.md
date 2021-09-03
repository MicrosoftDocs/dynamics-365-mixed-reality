---
author: v-mhoag
description: Learn how to enable calling in a Dynamics 365 Guides environment 
ms.author: v-mhoag
ms.date: 08/07/2021
ms.topic: article
title: Enable calling for an environment in Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# Enable calling in a Dynamics 365 Guides environment 

When calling is enabled, a Microsoft Dynamics 365 Guides HoloLens user can make a one-to-one call to a remote collaborator. The remote collaborator can join the call using the Microsoft Teams desktop app or the mobile app. During the call, the remote collaborator can see everything seen by the Dynamics 365 Guides user, including holograms and the real world behind the holograms.

If you're an admin for Dynamics 365 Guides, you can enable or disable calling for all guides accessed by a user in a specific Dynamics 365 Guides environment. Enabling or disabling calling by environment is useful when operators or authors do not need to work with remote collaborators. Or if it is preferred that HoloLens users are not able to start a call and allow remote collaborators to see everything that they see while working in Dynamics 365 Guides.  

<!--In the second sentence in the above paragraph, how about "Enabling or disabling by environment is useful depending on whether operators or authors need to work with remote collaborators or not. Or you may want to restrict HoloLens users from calling a remote collaborator and sharing everything they see while working in Dynamics 365 Guides"?-->

<!--Is calling enabled by default?-->

## Settings

1. Sign in to the instance by using your admin or author credentials.

    > [!TIP]
    > To find the URL for the instance, select the **Analyze** tab in the PC app. The URL is shown in the **Instance URL** field at the bottom of the page. Copy this URL, and paste it into the address bar of your web browser.
    >
    > ![Instance URL field.](media/instance-url.PNG "Instance URL field")

2. In Power Apps, select the **Guides** app tile.

    ![Guides app tile.](media/guides-app-tile.PNG "Guides app tile")
    
3.	In the left pane, select **Settings** to view all settings for the instance.

    ![Settings highlighted in the left pane.](media/Admin-EnableCalling01__Background-GuidesMDA-AreaPicker-Settings.png "Settings highlighted in left pane")

4.	On the left side of the screen, select **Environment**, and then move the **Enable Call** slider as needed to enable or disable calling for the environment.

    ![New command highlighted at top of Power Apps screen.](media/Admin-EnableCalling02__Background-GuidesMDA-AreaSettings-Environment.png "New command highlighted at top of Power Apps screen") 

    If a user tries to start a call while working in an environment where calling is disabled, the user will see the following error message: 

    **Your admin may have disabled calling or you may not have a Microsoft Teams or Remote Assist license**

## See also

[Overview of calling in Dynamics 365 Guides ](create-guide.md)

[Calling licensing and product requirements](admin-export-import-folders.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
