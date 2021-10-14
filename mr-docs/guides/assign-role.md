---
author: Mamaylya
description: Assign an Author or Operator role to users in Microsoft Dynamics 365 Guides.
ms.author: mamaylya
ms.date: 06/10/2021
ms.topic: article
title: Assign an Author or Operator role to a user to control whether a user can author a guide or just view a guide
ms.reviewer: v-bholmes
---

# Assign an Author or Operator role to an individual user in Dynamics 365 Guides

If you're a Microsoft Dynamics 365 Guides admin, you can assign an Author or Operator role to users to limit what they can do in the apps. The Restricted Author and 
Restricted Operator roles provide an extra layer of control. [Learn about the privileges provided by each role](admin-role-types.md).

> [!NOTE]
> You can also assign user roles in bulk by using [Azure Active Directory groups](admin-assign-role-groups.md).

## Prerequisites

To assign user roles:

- You must have an active Dynamics 365 Guides license. For more information, see [Buy a subscription or sign up a free trial](setup-step-one.md).

- The latest Dynamics 365 Guides solution must be installed. For more information, see [Update to the latest solution](upgrade.md).

- You must have access to the Power Platform admin center and have full admin privileges.

## Assign roles to a user
> [!NOTE]
> Users can take up to one hour to appear in the Dynamics 365 admin center after the licenses are added in the Microsoft 365 admin center.

1. Open the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), in the **Environments** page, select the Guides solution, select the **More environment actions** (ellipsis **...**) button, and then select **Settings**.

    ![Settings command.](media/access-teams-9.PNG "Settings command")

2. In the **Settings** page, select **Users**.

    ![User button.](media/add-user-roles-0.PNG "User button")

3. Select **Add user**. In the **Add user** pane on the right side of the screen, enter the user's name, and the select **Add**.

    ![Add user.](media/add-user-4.PNG "Add user")

4. Select user and select **Manage security roles**

    ![Add user roles.](media/add-user-roles.PNG "Add user roles")

5. Under **Manage security roles**, make sure that the **Basic User** check box is selected.

    ![Basic User check box.](media/basic-user-role.PNG "Basic User check box")

    
6. Select the check box(es) for the appropriate role(s) for the selected user(s), and then select **Save**.

    ![Author and Operator check boxes.](media/select-role.PNG "Author and Operator check boxes")

    [Learn about the different Author and Operator roles](admin-role-types.md).

    > [!NOTE
    > If you want the user to have admin privileges, select the **System Administrator** check box.



## Troubleshooting

If users don't appear in the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), select **Add user**. In the **Add user** dialog box, enter the account details, and then select **Add**. Users added to the instance should appear in the user list within a few minutes.

![Adding a user in Power Platform admin center.](media/select-manage-users2.PNG "Adding a user in Power Platform admin center")

## See also

[Add additional user accounts to Dynamics 365 Guides](add-users.md)<br>
[Learn about the Author and Operator roles](admin-role-types.md)<br>
[Assign roles in bulk through Azure AD groups](admin-assign-role-groups.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
