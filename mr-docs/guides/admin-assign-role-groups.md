---
title: Assign Dynamics 365 Guides Author and Operator roles to a Microsoft Entra group 
description: Learn how to assign Author and Operator roles to a Dynamics 365 group team that's linked to a Microsoft Entra group.
author:  davepinch
ms.topic: article
ms.date: 11/08/2021
ms.author: davepinch
ms.reviewer: v-wendysmith
---

# Assign Author and Operator roles to a Dynamics 365 group team linked to a Microsoft Entra group

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

You can assign [Dynamics 365 Guides Author and Operator roles](admin-role-types.md) to a Dynamics 365 group team linked to a Microsoft Entra group to make it easier to organize and manage user roles. By linking Microsoft Entra Security groups or Microsoft 365 groups to a Dynamics 365 group team, Dynamics 365 Guides roles can be inherited by any user added to the Microsoft Entra group. To get an overview of Microsoft Entra groups and managing group teams, see the following links:

- [Groups in Microsoft 365 and Entra, and Which is Right for You](/microsoft-365/community/all-about-groups)

- [Manage group teams](/power-platform/admin/manage-group-teams)

> [!NOTE]
> SharePoint groups are not supported by Dynamics 365. Only Microsoft Entra Security groups or Microsoft 365 groups are supported by Dynamics 365 group teams.

## Create a Microsoft Entra group

To learn how to create a Microsoft Entra Security group or a Microsoft 365 group, see [Create a basic group and add members using Microsoft Entra admin center](/entra/fundamentals/how-to-manage-groups).

## Create a Dynamics 365 group team

The type of group you create in Dynamics 365 depends on the type of Microsoft Entra group you're starting with (Security or Microsoft 365). For more information, see [Create a group team](/power-platform/admin/manage-group-teams#create-a-group-team).  

For more information on how to link a Microsoft Entra group to a Dynamics 365 group team, see [Manage group teams](/power-platform/admin/manage-group-teams). 

> [!NOTE] 
> When setting a value for **membership type** by selecting one of the options (**Members**, **Members & Guests**, **Guests**, or **Owners**), be aware that this value determines which users in the group will flow into the Dynamics 365 group team. Setting the **membership type** is similar to setting a pass-through filter. For example, if **Members** is selected and a guest is added to the group, the guest will not flow down into the team and will not inherit the role from the Dynamics 365 group team.  

## Two ways to assign roles to a team

You can assign roles to a team in two ways: 

- Option 1: Assign a group team to a Dynamics 365 Guides role. In this case, the additions must be made to the Basic User role and any additional roles that you want to modify. This is the best option if you need to assign a role to many Dynamics 365 group teams.

- Option 2: Assign a Dynamics 365 Guides role to a group team. This is the best option if you need to modify a small number of Dynamics 365 group teams. For example, if you add the Author role to a Microsoft 365 group, anyone in the group will have a role that will allow them to create and edit a guide. The guide will be owned by the group.

### Option 1: Assign a group team to a Dynamics 365 Guides role

For this option, you'll update a role to include the Dynamics 365 group team that was created using the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments).

1. In the Power Platform admin center, select the environment that you want to update.

2. In the **Access** section, under **Security roles**, select **See all**.

    ![power platform admin.](media/power-platform-admin-center-env-setting.PNG "power platform admin")
 
3. Under **Role**, select **Basic User**. 

    ![basic user.](media/power-platform-enviro-roles.PNG "basic users")
    
    > [!NOTE]
    > The **Basic User** role must be added to the group to enable Dynamics 365 Guides for the users in this group team. 

4. At the top of the screen, select **Add people**.

    ![Add people command at top of Power Platform screen.](media/power-platform-security-role-add-people.PNG "Add people command at top of Power Platform screen")
    
5. Search for the Dynamics 365 group team created above, select it in the search results, and then select **Add**.

    ![add group.](media/power-platform-security-add-group.PNG "Add group")
 
6. Repeat the steps above for the [Dynamics 365 Guides role](/dynamics365/mixed-reality/guides/assign-role) that you want to apply to this team. Dynamics 365 Guides roles include:

    - Dynamics 365 Guides Author
    
    - Dynamics 365 Guides Operator
    
    - Dynamics 365 Guides Restricted Author
    
    - Dynamics 365 Guides Restricted Operator

    [Learn more about the different Author and Operator roles](admin-role-types.md).

7. Repeat the above steps for any additional roles that you want to apply to the group team.

> [!NOTE]
> When a user is added to a Microsoft Entra group, it doesn't show up in the team until the user signs in. 

### Option 2: Assign a Dynamics 365 Guides role to a group team

For this option, you'll update the Dynamics 365 Guides role to include the Dynamics 365 group team created using the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments). For more information, see [Add roles to group teams](/power-platform/admin/manage-teams).

1. In the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), in the **Environments** page, select the same Guides solution, select the **More environment actions** (ellipsis **...**) button, and then select **Settings**.

    ![Settings command.](media/access-teams-9.PNG "Settings command")

2. In the **Settings** page, select **Teams**.

    ![Teams button.](media/access-teams-14.PNG "Teams button")
 
3. Choose the team to modify, and then select the **Team options** (ellipsis) button.

    ![select team options.](media/power-platform-admin-center-env-teams.png "select team options")

4. Select **Manage security roles**.

    ![select manage security roles.](media/power-platform-admin-center-env-teams-manage-roles.png "manage security roles")

5. Confirm that the **Basic User** role is selected, and then select any additional roles that you want to apply to the group.

    ![Select roles.](media/power-platform-admin-center-env-teams-manage-roles-security.png "Select roles")
    
    [Learn more about the different Author and Operator roles](admin-role-types.md).
    
> [!NOTE]
> When a user is added to a Microsoft Entra group, it doesn't show up in the team until the user signs in. 

## See also

- [Learn about the different Author and Operator roles](admin-role-types.md)
- [Assign an Author or Operator role to an individual user](assign-role.md)
