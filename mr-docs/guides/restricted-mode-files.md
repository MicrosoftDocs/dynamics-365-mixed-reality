---
title: Restrict the ability to access OneDrive files in Dynamics 365 Guides
author: m-hartmann
description: Learn how to restrict the ability to access OneDrive files in Microsoft Dynamics 365 Guides.
ms.author: mhart
ms.date: 01/20/2022
ms.topic: how-to
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Restrict the ability to access OneDrive files in Dynamics 365 Guides

If you [have a scenario where you need to protect your company information](restricted-mode-overview.md), you can restrict the ability for Microsoft Dynamics 365 Guides users from accessing OneDrive files. Restricting the ability to access OneDrive files is also helpful in a situation where a service account is shared between users and you want to prevent users from accessing each other's files.

## Restrict access to OneDrive files

1. Sign in to the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?#/users) as an admin.

1. In the left pane, select **Users** > **Active users**, and then select **Add a user**.

   :::image type="content" source="media/restricted-mode-files-add-user.jpg" alt-text="Screenshot of the admin portal with Add user controls highlighted.":::

    > [!IMPORTANT]
    > It's critical to create a NEW ACCOUNT to make sure that the user will not have access to the licenses required to access OneDrive files.

1. Fill out the user information, and then select **Next**.

1. Select the **Dynamics 365 Guides** and **Microsoft Teams** license check boxes.

   :::image type="content" source="media/restricted-mode-files-select-licenses.jpg" alt-text="Screenshot showing Dynamics 365 Guides and Microsoft Teams check boxes selected.":::

    > [!NOTE]
    > The name of the Teams license may vary based on the products you have installed.

1. Clear the **Office for the Web** and **SharePoint** license check boxes, and then select **Next**.

   :::image type="content" source="media/restricted-mode-files-clear-licenses.jpg" alt-text="Screenshot showing SharePoint and Office for the Web check boxes cleared.":::

1. In the **Optional settings** section, leave the default value (no administration access), and then select **Next**.

1. In the **Review and finish** section, make sure the information is correct, and then select **Finish adding** when you're ready.

1. The last step confirms that the user was added correctly. Select **Close**.

## Next steps

- [Overview of restricting capabilities in Dynamics 365 Guides](restricted-mode-overview.md)
- [Restrict calling and the ability to search and access contacts](restricted-mode-calling.md)
- [Restrict the ability to sign out of the HoloLens app](restricted-mode-signout.md)
