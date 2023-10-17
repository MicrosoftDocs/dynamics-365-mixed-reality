---
author: davepinch
description: Add additional user accounts to a Microsoft Dynamics 365 Guides license.
ms.author: davepinch
ms.date: 08/10/2022
ms.topic: article
title: Add additional users in Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# Add additional user accounts to Dynamics 365 Guides

To add additional users to Microsoft Dynamics 365 Guides, you must first assign the Dynamics 365 Guides license to a new or existing user in the Microsoft 365 admin center. Then, in the Power Platform admin center, configure the roles that the users will have access to (Author, Operator, or Admin).

## Add a new user 

1. Open the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home).

2. In the left pane, select **Users**, and then select **Active users**.

3. On the **Active users** page, select **Add a user**.

    ![Add a user command.](media/add-additional-user.png "Add a user command")

4. On the **Set up the basics** page, fill in the information for the new user. When you've finished, select **Next**.

    ![Set up the basics page.](media/setup-basics.png "Set up the basics page")

    > [!NOTE]
    > By default, a password is automatically generated for new user accounts. Users must change this password the first time that they sign in by using their new account. If you want to set a permanent password instead of using an automatically generated password, select the **Let me create the password** option, and clear the **Require this user to change their password when they first sign in** check box.

5. On the **Assign product licenses** page, select the location for the user, and then, under **Licenses**, select the **[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]** check box. When you've finished, select **Next**.

    ![Assign product licenses page.](media/assign-license-user.png "Assign product licenses page")

6. On the **Optional settings** page, leave the **User (no administrator access)** check box selected unless the user will be an admin. In that case, select the **Global administrator** check box.

    ![Optional settings page.](media/user-optional-settings.png "Optional settings page")

7. Scroll down, expand the **Profile info** section, and fill in the user's profile information. When you've finished, select **Next**.

    ![Profile info section.](media/expanded-profile-info.png "Profile info section")

8. Review the information on the last page. To make changes, select the **Edit** button below the relevant sections. When you've finished, select **Finish adding**.

    ![Review page with Edit buttons.](media/review-page.png "Review page with Edit buttons")

8. If you selected the **Auto-generate password** option in step 4, make a note of the password. The user will need this password to sign in.

    ![Automatically generated password.](media/review-user-settings.png "Automatically generated password")

9. Select **Close**.

After you add user accounts, the next step is to assign the **Author**, **Operator**, or **Admin** user role for the solution. For more information, see [Assign user roles](assign-role.md).

## Assign a Dynamics 365 Guides license to an existing user

1. Open the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home). 

2. In the left pane, select **Users**, and then select **Active users**. 

3. Select the **More actions** (**...**) button for the user that you want to assign a license to, and then select **Manage product licenses**. 

    ![Select Manage product licenses.](media/select-manage-product-licenses.PNG "Select Manage product licenses")

4. In the dialog box that appears, on the **Licenses and Apps** tab, select the **Dynamics 365 Guides** check box. Then, under **Apps**, make sure that the **Common Data Service**, **Dynamics 365 Guides**, and **PowerApps for Guides** check boxes are selected. 

    ![Verify check boxes.](media/verify-check-boxes.PNG "Verify check boxes")

5. Select **Save changes**.

## Add a guest user

Anyone who is not part of your organization, but has a Microsoft Entra account, can be added as a guest by a global admin. The user can then access Dynamics 365 Guides content in your organization as an operator. [Learn about adding a guest user in Dynamics 365 Guides](admin-add-guest-user.md)

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

## What's next?

- [Assign user roles](assign-role.md)
- [Add a guest user](admin-add-guest-user.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
