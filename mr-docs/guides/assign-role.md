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

## Assign user roles

> [!NOTE]
> Users can take up to one hour to appear in the Dynamics 365 admin center after the licenses are added in the Microsoft 365 admin center.

1. Open the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), in the **Environments** page, select the same Guides solution, select the **More environment actions** (ellipsis **...**) button, and then select **Settings**.

    ![Settings command.](media/access-teams-9.PNG "Settings command")

2. In the **Settings** page, select **Teams**.

    ![Teams button.](media/access-teams-14.PNG "Teams button")

3. Select **Create team**.

    ![Create Team.](media/access-teams-15.PNG "Create Team")

4. On the right side of the screen, under **New team**, set the **Team name**, **Business unit**, and **Administrator** fields. Change the value of the **Team type** field to **Access**, and then select **Next**.

    ![New team settings.](media/access-teams-16.PNG "New team settings")

5. To add users to the team, select the ellipsis button next to the team name, and then select **Manage team members**.

    ![Manage team members.](media/access-teams-17.PNG "Manage team members")

6. Select **Add members to the team**.

    ![Add members to the team.](media/access-teams-17A.PNG "Add members to the team")

7. Use the search box to add one or more members to the team, and then select **Add**.

    ![Search and add team members.](media/access-teams-17B.PNG "Search and add team members")

    > [!IMPORTANT]
    > You can access Dynamics 365 Guides data through the **Guides Hub** tile.  The Guides model-driven app isn't intended as a replacement for authoring in the PC and HoloLens apps. If you use the model-driven app to create, update, or delete records, you might make Guides nonfunctional or prevent users from using the PC or HoloLens apps in the intended way. Currently, Guide modification through the model-driven app isn't fully supported and should be reserved for experienced Dynamics 365 developers who are familiar with Microsoft Dataverse.

8. Follow one of these steps:

    - If the users are already in the list, skip ahead to step 12 to assign user roles.

    - If you want to add one or more users, select **Add user** at the top of the page, enter the account details in the **Add user** dialog box, and then select **Add**. For more information, see the "Troubleshooting" section later in this article.

        > [!NOTE]
        > Users added to the instance will be added to the user list within a few minutes.

9. Open **Settings** > **Users**.

   ![Manage Users in Dynamics 365 command.](media/select-manage-users.PNG "Manage Users in Dynamics 365 command")

10. Select one or more users, and then select **Manage security roles** at the top of the page.

    ![Manage Roles button.](media/select-manage-roles.PNG "Manage Roles button")

11. Under **Manage security roles**, make sure that the **Basic User** check box is selected.

    ![Basic User check box.](media/basic-user-role.PNG "Basic User check box")

    > [!NOTE]
    > You may see a **Common Data Service** check box instead of a **Basic User** check box. If so, select that check box.

12. Select the check box for the appropriate role for the selected users, and then select **OK**.

    ![Author and Operator check boxes.](media/select-role.PNG "Author and Operator check boxes")
    
    [Learn about the different Author and Operator roles](admin-role-types.md).

13. If you want the user to have admin privileges, select the **System Administrator** check box.

## Troubleshooting

If users don't appear on the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), select **Add user**. In the **Add user** dialog box, enter the account details, and then select **Add**. Users added to the instance should appear in the user list within a few minutes.

![Adding a user in Power Platform admin center.](media/select-manage-users2.PNG "Adding a user in Power Platform admin center")

## See also

[Add additional user accounts to Dynamics 365 Guides](add-users.md)<br>
[Learn about the Author and Operator roles](admin-role-types.md)<br>
[Assign roles in bulk through Azure AD groups](admin-assign-role-groups.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
