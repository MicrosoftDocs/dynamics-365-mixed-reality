---
title: About the Author and Operator user roles in Dynamics 365 Guides
description: Learn about the Author, Operator, Restricted Author, and Restricted Operator user roles in Dynamics 365 Guides
author:  davepinch
ms.topic: concept-article
ms.date: 11/09/2023
ms.author: prashan
ms.reviewer: v-wendysmith
---

# About the Author and Operator roles in Dynamics 365 Guides

If you're a Microsoft Dynamics 365 Guides admin, you can assign an Author or Operator role to users to limit what they can do in the apps. When you assign an Operator or Author role, that role automatically grants the user access to all guides in the environment.

The Restricted Author and Restricted Operator roles provide an extra layer of control by limiting access to guides. Users who are assigned the Restricted Author and Restricted Operator roles **do not** inherit access to any guides or guide content (3D objects, images, or videos) created in the environments that they're permitted to access.

The following table describes the privileges that each role grants. All users must have the **Basic User** role assigned to them.

| Role | Description |
|---|---|
| Author | Use the PC app and HoloLens app to create, edit, and operate guides. Users who have the Author role can also rename and deactivate existing guides. |
| Operator | Use the HoloLens app to view and operate a guide. Users who have the Operator role can also save time by skipping the **Select Mode** dialog box when they open a guide. |
|Restricted Author| Use the PC app and HoloLens app to create, edit, and operate guides or use guides content that:<br>- The user created<br>- Were explicitly shared with them or shared with an owner team they're a member of<br>- Were assigned to the user or assigned to an owner team that the user is a member of|
|Restricted Operator| Use the HoloLens app to view and operate a guide or access guides content that: <br>- The user created<br>- Were explicitly shared with them or shared with an owner team they're a member of<br>- Were assigned to the user or assigned to an owner team that the user is a member of |
|App Access|  This is a system role that shouldn't be assigned to any users, groups, or teams. <br> The purpose of this role is to enable a service application to perform data integration between Microsoft Dataverse and other services including the object anchor service. |

For more information about system roles in Power Platform apps, see [system and application users.](/power-platform/admin/system-application-users)

> [!IMPORTANT]
> If you followed the instructions in the [Buy Dynamics 365 Guides](buy-guides.md) topic when you set up Dynamics 365 Guides, any users that you added were automatically assigned the **Author** role. You must explicitly assign the **Operator** role to specific users if you don't want them to have **Author** role privileges.

## Next steps

- [Assign a role to an individual user](assign-role.md)
- [Assign a role through Microsoft Entra groups](admin-assign-role-groups.md)
- [Restrict access to an environment by using security groups](admin-security.md)
- [Assign or share a guide by changing ownership](admin-access-assign.md)
- [Assign or share a guide through an access team](admin-access-teams.md)
