---
title: Add licenses, users, and roles to Microsoft Entra security groups 
description: Learn how to use Microsoft Entra groups and add users, assign licenses, and assign Author and Operator roles that link to a Dynamics 365 group team.
author:  davepinch
ms.topic: how-to
ms.date: 04/24/2024
ms.author: prashan
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Add licenses, users, and roles to Microsoft Entra security groups

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

Use [Microsoft Entra security groups](/entra/fundamentals/concept-group-based-licensing) to better organize and manage Guides users and user roles.

For example, you have 15 Authors and 20 Operators. Create an Entra security group for your Authors, adding them as users and assigning them licenses. Create another Entra security group for your Operators adding them as users and assigning them licenses. When you create a Dataverse team for your authors and one for your operators, link these teams to your Entra security groups. The Entra security group memberships sync automatically from the security group to the Dataverse group team. Then, you can assign the roles to the Dataverse teams rather than to each individual.

## Prerequisites

- You must have an [active Dynamics 365 Field Servie or Guides license](buy-guides.md).

- The [Dynamics 365 Guides solution must be installed](install-guides.md).

## Add users and assign licenses with a Microsoft Entra security group

1. [Create a Microsoft Entra security group and add users.](/entra/fundamentals/how-to-manage-groups)

1. [Assign Field Servie or Guides licenses to the Entra security group.](/entra/identity/users/licensing-groups-assign)

   > [!IMPORTANT]
   > Make sure each group is assigned Dynamics 365 Guides, Common Data Service, and PowerApps for Guides.

1. [Create a Dataverse group team](/power-platform/admin/manage-group-teams#create-a-group-team) in the environment where you installed the Guides solution, linking the group to the Microsoft Entra security group you created.

   > [!NOTE]
   > When setting a value for **membership type** by selecting one of the options (**Members**, **Members & Guests**, **Guests**, or **Owners**), be aware that this value determines which users in the group will flow into the Dataverse group team. Setting the **membership type** is similar to setting a pass-through filter. For example, if **Members** is selected and a guest is added to the group, the guest will not flow down into the team and will not inherit the role from the Dataverse group team.  

1. Repeat this process for each group of users.

## Assign Guides roles to a Dataverse group team

You can assign roles to a team in two ways:

- **Assign a Dataverse group team to a Guides role**. In this case, the additions must be made to the Basic User role and any other roles that you want to modify. This assignment is the best option if you need to assign a role to many Dataverse group teams.

- **Assign a Guides role to a Dataverse group team**. This assignment is the best option if you need to modify a few Dataverse group teams. For example, if you add the Author role to a Microsoft 365 group, anyone in the group has a role that allows them to create and edit a guide. The guide is owned by the group.

### Assign a Dataverse group team to a Guides role

For this option, update a role to include the Dataverse group team that was created using the Power Platform admin center.

1. [Access a Guides role.](/power-platform/admin/database-security#assign-security-roles-to-users-in-an-environment-that-has-a-dataverse-database)

1. Under **Role**, select **Basic User**.

   > [!NOTE]
   > The **Basic User** role must be added to the group to enable Dynamics 365 Guides for the users in this group team.

1. Select **Members** > **Add people**, then search and select the Dataverse group team you created. Then select **Add**. Repeat for each Dataverse group team.

1. Repeat these steps for each Guides role.

### Assign a Guides role to a Dataverse group team

For this option, update the Guides role to include the Dataverse group team created using the Power Platform admin center.

1. [Access the Dataverse group team.](/power-platform/admin/manage-teams)

1. Confirm that the **Basic User** role is selected, and then select any other roles that you want to apply to the group.

1. Repeat these steps for each Dataverse group team.

## Next steps

- [Set up a Guides device license for multiple operators](device-license.md)
- Contact your Guides users to have them [install the PC app and set up their HoloLens](install-pc-hololens-apps.md)
