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

- You have access to the Microsoft Power Platform admin center and have full admin privileges.

## Assign roles to a user
> [!NOTE]
> Users can take up to one hour to appear in the Dynamics 365 admin center after the licenses are added in the Microsoft 365 admin center.

1. Open the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), select the Guides solution in the **Environments** page, select the **More environment actions** (ellipsis **...**) button, and then select **Settings**.

    ![Settings command.](media/access-teams-9.PNG "Settings command")

2. In the **Settings** page, select **Users**.

    ![User button.](media/add-user-roles-0.PNG "User button")

3. Select **Add user**, enter the user's name in the **Add user** pane on the right side of the screen, and then select **Add**.

    ![Add user.](media/add-user-4.PNG "Add user")

4. Select the user, and then select **Manage security roles**.

    ![Add user roles.](media/add-user-roles.PNG "Add user roles")

5. Under **Manage security roles**, make sure that the **Basic User** check box is selected.

    ![Basic User check box.](media/basic-user-role.PNG "Basic User check box")
    
6. Select the check box for the appropriate role, and then select **Save**.

    ![Author and Operator check boxes.](media/select-role-1.png "Author and Operator check boxes")

    [Learn about the different Author and Operator roles](admin-role-types.md).

    > [!NOTE
    > If you want the user to have admin privileges, select the **System Administrator** check box.

## See also

[Add additional user accounts to Dynamics 365 Guides](add-users.md)<br>
[Learn about the Author and Operator roles](admin-role-types.md)<br>
[Assign roles in bulk through Azure AD groups](admin-assign-role-groups.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
