---
title: About the Author and Operator user roles in Dynamics 365 Guides
description: Learn about the Author, Operator, Restricted Author, and Restricted Operator user roles in Dynamics 365 Guides
author:  davepinch
ms.topic: article
ms.date: 11/08/2021
ms.author: davepinch
ms.reviewer: v-wendysmith
---

# About the Author and Operator roles in Dynamics 365 Guides

If you're a Microsoft Dynamics 365 Guides admin, you can assign a Dynamics 365 Guides Author or Dynamics 365 Guides Operator role to users to limit what they can do in the apps. The Dynamics 365 Guides Restricted Author and Dynamics 365 Guides Restricted Operator roles provide an extra layer of control by limiting access to guides. Users who are assigned the Restricted Author and Restricted Operator roles **do not** inherit access to any guides or guide content (3D models, images, or videos) created in the environments that they are permitted to access.

The following table describes the privileges that each role grants.

| Role | Description |
|---|---|
| Dynamics 365 Guides Author | Use the PC app and HoloLens app to create, edit, and operate guides. Users who have the Author role can also rename and deactivate existing guides. |
| Dynamics 365 Guides Operator | Use the HoloLens app to view and operate a guide. Users who have the Dynamics 365 Guides Operator role can also save time by skipping the **Select Mode** dialog box when they open a guide. |
|Dynamics 365 Guides Restricted Author| Use the PC app and HoloLens app to create, edit, and operate guides or use guides content that:<br>- The user created<br>- Were explicitly shared with them or shared with an owner team they are a member of<br>- Were assigned to the user or assigned to an owner team that the user is a member of|
|Dynamics 365 Guides Restricted Operator|  Use the HoloLens app to view and operate a guide or access guides content that: <br>- The user created<br>- Were explicitly shared with them or shared with an owner team they are a member of<br>- Were assigned to the user or assigned to an owner team that the user is a member of |
|App Access|  This is a system role that should not be assigned to any users, groups, or teams. <br> The purpose of this role is to enable a service application to perform data integration between Microsoft Dataverse and other Microsoft services including the Azure Object Anchor service. |

See the following links for more information:

|Area|Link|
|------------------------------------------------------------|-------------------------------------------------------------------------|
|Dynamics 365 Guides Restricted Author and Restricted Operator roles in access teams|[Share a guide or guide content in Dynamics 365 Guides by using an access team](admin-access-teams.md#assign-a-restricted-security-role)|
|System roles in Power Platform|[System and application users](/power-platform/admin/system-application-users)|
|Azure Object Anchor service|[Object Anchors Service](https://azure.microsoft.com/services/object-anchors/)|

> [!IMPORTANT]
> If you followed the instructions in the [Try or buy, and deploy Dynamics 365 Guides](setup-step-one.md) topic when you set up Dynamics 365 Guides, any users that you added were automatically assigned the **Dynamics 365 Guides Author** role. You must explicitly assign the **Dynamics 365 Guides Operator** role to specific users if you don't want them to have **Author** role privileges.

## See also

- [Assign a role to an individual user](assign-role.md)
- [Assign a role through Azure Active Directory groups](admin-assign-role-groups.md)
- [Restrict access to an environment by using security groups](admin-security.md)
- [Assign or share a guide by changing ownership](admin-access-assign.md)
- [Assign or share a guide through an access team](admin-access-teams.md)
