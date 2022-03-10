---
author: melissahellmund
description: Learn how to create an access team to assign ownership of a guide in Microsoft Dynamics 365 Guides.
ms.author: mehellmu
ms.date: 04/05/2022
ms.topic: article
title: Create an access team to assign ownership of a guide in Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# Create an access team to assign ownership of a guide in Dynamics 365 Guides

[Assigning the ownership of a guide](admin-access-assign.md) to a user in Microsoft Dynamics 365 Guides is the preferred method for controlling who can use specific guides. If teams change frequently, resulting in a need to create and delete teams often, a Dynamics 365 admin (or other user with the Share privilege) can share guides with [access teams](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/use-access-teams-owner-teams-collaborate-share-information) to control who can see specific guides and guide content (3D models, images, or videos).

> [!NOTE]
> Dynamics 365 offers additional ways to customize and configure access to specific records in Microsoft Dataverse. However, this topic doesn't cover advanced configuration, such as the creation of [owner teams](/dynamics365/customerengagement/on-premises/developer/use-access-teams-owner-teams-collaborate-share-information).

For more information on how privileges and access works, see [How access to a record (guide) is determined](https://docs.microsoft.com/power-platform/admin/how-record-access-determined).

For more information on the three types of teams (*owner* team, Azure Active Directory *group* team, or *access* team), see [Manage teams](https://docs.microsoft.com/power-platform/admin/manage-teams).

## How access teams work with the Operator and Author user roles

You can assign an Operator or Author role to a user to specify whether that user can create and edit guides as an author or use them as an operator. When you assign an Operator or Author role, that role automatically grants the user access to all guides in the environment. To limit access to specific guides or guide content (3D models, images, or videos), you can use the Restricted Operator and Restricted Author roles. [Learn more about the different roles](admin-role-types.md).

> [!IMPORTANT]
> If you have already restricted access to guides or guides content by creating your own security role with reduced privileges, you’ll need to remove that security role and replace it with one of the built-in security roles as described in this article.

## Assign a restricted security role

To prevent a specific user from accessing all guides by default, you can update the user's security role to the Restricted Operator role. Once assigned, they will be able to see only guides assigned or shared with them or teams they are members of.

> [!NOTE]
> The steps outlined in this procedure show how to restrict operator privileges. You can restrict author privileges in a similar way. This article also shows how to restrict access to the **Guides** entity. You can use the same steps to restrict access to other types of Dynamics 365 Guides records (3D models, images, or videos) to limit their visibility to certain users or teams.

1. In the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), in the **Environments** page, select the environment, select the **More environment actions** (**...**) button, and then select **Settings**.

    ![Settings command.](media/access-teams-9.PNG "Settings command")

2. In the **Settings** page, select **Users**.

    ![Users button.](media/access-teams-10.PNG "Users button")

3. Select a specific user by selecting the user's full name.

    ![Select a user.](media/access-teams-11.PNG "Select a user")

4. Select **Manage Roles** to open the **Manage User Roles** dialog box, and then do the following:

    1. If it's selected, clear the check box for the **Dynamics 365 Guides Operator** role.

    2. Select the check box for the **Basic User** role.

    3. Select the check box for the **Dynamics 365 Guides Restricted Operator** role.

    4. Select **OK**.

    ![Clear and select roles.](media/manage-user-basic-user-restricted-op.PNG "Clear and select roles")

## Create an access team

A user can be associated with more than one access team.

> [!NOTE]
> If you or someone else has already created an access team that you want to use, skip ahead to the next procedure.

1. In the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), in the **Environments** page, select the same Guides solution, select the **More environment actions** (ellipsis **...**) button, and then select **Settings**.

    ![Settings command.](media/access-teams-9.PNG "Settings command")

2. In the **Settings** page, select **Teams**.

    ![Teams button.](media/access-teams-14.PNG "Teams button")

3. Select **Create team**.

    ![New button.](media/access-teams-15.PNG "New button")

4. In the **New team** pane on the right side of the screen, set the **Team name**, **Business unit**, and **Administrator** fields. Change the value of the **Team type** field to **Access**, and then select **Next**.

    ![New team settings.](media/access-teams-16.PNG "New team settings")

5. To add users to the team, select the **More information** (ellipsis) button next to the team name, and then select **Manage team members**.

    ![Manage team members.](media/access-teams-17.PNG "Manage team members")

6. Select **Add members to the team**.

    ![Add members to the team.](media/access-teams-17A.PNG "Add members to the team")

7. On the right side of the screen, under **Add team members**, enter the name(s) of the user(s) that you want to add, and then select **Add**.

    ![Search and add team members.](media/access-teams-17B.PNG "Search and add team members")

## See also

- [Use access teams and owner teams to collaborate and share information](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/use-access-teams-owner-teams-collaborate-share-information?view=op-9-1)
- [Assign an Operator or Author role to an individual user](assign-role.md)
- [Assign roles in bulk by using Active Directory groups](admin-assign-role-groups.md)
- [Restrict access to an environment by using security groups](admin-security.md)
= [Learn more about security roles and privileges](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/admin/security-roles-privileges)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
