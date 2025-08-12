---
title: Restrict the ability to access OneDrive files in Dynamics 365 Remote Assist
author: prashantyvr
description: Learn how to restrict the ability to access OneDrive files in Microsoft Dynamics 365 Remote Assist
ms.author: prashan
ms.date: 06/07/2024
ms.topic: how-to
ms.reviewer: v-wendysmith
ms.custom: sfi-image-nochange
---

# Restrict the ability to access OneDrive files in Dynamics 365 Remote Assist

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

If you [have a scenario where you need to protect your company information](restricted-mode-overview.md), you can restrict the ability for Microsoft Dynamics 365 Remote Assist users from accessing OneDrive files. Restricting the ability to access OneDrive files is also helpful in a situation where a service account is shared between users and you want to prevent users from accessing each other's files. 

When you restrict the ability to access OneDrive files, HoloLens users will see the **Files** tab, but no files will be visible and they'll see this message: "We can't connect to OneDrive."

## Restrict access to OneDrive files

1. Sign in to the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?#/users) as an admin. 

2. In the left pane, select **Users** > **Active users**, and then select **Add a user**.

    ![Screenshot showing Active users and Add a user highlighted.](media/restricted-mode-files-add-user.jpg "Screenshot showing Active users and Add a user highlighted")
    
    > [!IMPORTANT]
    > It's critical to create a NEW ACCOUNT to make sure that the user will not have access to the licenses required to access OneDrive files. 

3. Fill out the user information, and then select **Next**.

    ![Screenshot of Set up the basics section.](media/restricted-mode-files-user-info.jpg "Screenshot of Set up the basics section")

4. Select the **Dynamics 365 Remote Assist** and **Microsoft Teams** license check boxes.

    ![Screenshot showing Dynamics 365 Remote Assist and Microsoft Teams check boxes selected.](media/restricted-mode-files-select-licenses.jpg "Screenshot showing Dynamics 365 Remote Assist and Microsoft Teams check boxes selected")

    > [!NOTE]
    > The name of the Teams license may vary based on the products you have installed. 

5. Clear the **Office for the Web** and **SharePoint** license check boxes, and then select **Next**.

    ![Screenshot showing SharePoint and Office for the Web check boxes cleared.](media/restricted-mode-files-clear-licenses.jpg "Screenshot showing SharePoint and Office for the Web check boxes cleared")

6. In the **Optional settings** section, leave the default value (no administration access), and then select **Next**.

    ![Screenshot of Optional settings section.](media/restricted-mode-files-optional-settings.jpg "Screenshot of Optional settings section")

7. In the **Review and finish** section, make sure the information is correct, and then select **Finish adding** when you're ready.

8. The system confirms if the user was added correctly. Select **Close**.

    
## See also

- [Overview of restricting capabilities in Dynamics 365 Remote Assist](restricted-mode-overview.md)
- [Restrict calling and the ability to search and access contacts](restricted-mode-calling.md)
- [Restrict the ability to access asset records](restricted-mode-assets.md)
- [Restrict the ability to sign out of the HoloLens app](restricted-mode-signout.md)

