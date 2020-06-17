---
author: Mamaylya
description: Assign an Author or Operator role to users in Microsoft Dynamics 365 Guides to control whether users can edit and view guides (Author role) or just view guides (Operator role).
ms.author: mamaylya
ms.date: 01/28/2020
ms.service: crm-online
ms.topic: article
title: Assign an Author or Operator role to a user to control whether a user can author a guide or just view a guide
ms.reviewer: v-brycho
---

# Assign an Author or Operator role to a user in Dynamics 365 Guides

If you're a Microsoft Dynamics 365 Guides admin, you can assign an **Author** or **Operator** role to users to limit what they can do in the apps. The following table describes the privileges that each role grants.

| Role | Description |
|---|---|
| Author | Use the PC app and HoloLens app to create, edit, and operate guides. Users who have the **Author** role can also rename and inactivate existing guides. |
| Operator | Use the HoloLens app to view and operate a guide. Users who have the **Operator** role can also save time by skipping the **Select Mode** dialog box when they open a guide. |

> [!IMPORTANT]
> If you followed the instructions in the [Try or buy, and deploy Dynamics 365 Guides](setup.md) topic when you set up Dynamics 365 Guides, any users that you added were automatically assigned the **Author** role. You must explicitly assign the **Operator** role to specific users if you don't want them to have **Author** role privileges.

## Prerequisites

Before you can modify user roles, the following prerequisites must be in place:

- You have an active Dynamics 365 Guides license. For more information, see [Try or buy, and deploy Dynamics 365 Guides](setup.md).

- The latest Dynamics 365 Guides solution is installed. For more information, see [Upgrade to the latest solution](upgrade.md).

- You have access to the Power Platform admin center and have full admin privileges.

## Assign user roles

1. Open the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), and sign in by using your admin credentials.

2. If the **Environments** page doesn't appear, select **Environments** in the left pane to open it.

3. Select the environment that you want to work with, select the **More environment actions** (**...**) button, and then select **Settings**.

    ![Settings command](media/environment-settings.PNG "Settings command")

4. Select **Users + permissions** to expand the list of options, and then select **Users**. If you're prompted to sign in to Dynamics 365, be sure to use your admin credentials.

    ![Users selected](media/users-setting.PNG "Users selected")
    
5. Select **Manage Users in Dynamics 365** at the top of the page. 

   ![Manage Users in Dynamics 365 command](media/select-manage-users.png "Manage Users in Dynamics 365 command")

6. Select one or more users, and then select **Manage Roles** at the top of the page.

    ![Manage Roles button](media/select-manage-roles.PNG "Manage Roles button")

7. In the **Manage User Roles** dialog box, make sure that the **Common Data Service User** check box is selected.

    ![Common Data Service User check box](media/common-data-service-user.PNG "Common Data Service User check box")

8. Select the check box for the appropriate role for the selected users, and then select **OK**.

    ![Author and Operator check boxes](media/select-role.PNG "Author and Operator check boxes")

## See also

[Add additional user accounts to Dynamics 365 Guides](add-users.md)<br>
[Overview of authoring a guide](authoring-overview.md)<br>
[Overview of operating a guide](operator-overview.md)
