---
author: prashantyvr
description: Assign an Author or Operator role to users in Microsoft Dynamics 365 Guides.
ms.author: prashan
ms.date: 11/09/2023
ms.topic: how-to
title: Assign an Author or Operator role to a user to control whether a user can author a guide or just view a guide
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Assign an Author or Operator role to an individual user in Dynamics 365 Guides

As a Microsoft Dynamics 365 Guides admin, you can assign an Author or Operator role to users to limit what they can do in the apps. The Restricted Author and Restricted Operator roles provide an extra layer of control. [Learn about the privileges provided by each role](admin-role-types.md).

Choose how you want to assign roles to users and perform the appropriate task.

- To assign user roles in bulk using Microsoft Entra security groups, see [Assign roles to a Dynamics 365 group team linked to a Microsoft Entra group](admin-assign-role-groups.md).

- To assign roles to individual users, see the following steps.

## Prerequisites

- You must have an [active Dynamics 365 Field Servie or Guides license](buy-guides.md).

- The [Dynamics 365 Guides solution must be installed](upgrade.md).

- Admin permissions to the Microsoft Power Platform admin center.

## Assign roles to a user

> [!NOTE]
> Users can take up to one hour to appear in the Dynamics 365 admin center after the licenses are added in the Microsoft 365 admin center.

1. Open the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments).

1. Select the Guides solution in the **Environments** page and navigate to the **Users** page. See [Assign security roles](/power-platform/admin/assign-security-roles) for more information.

1. Select the user, and then select **Manage security roles**.

1. Under **Manage security roles**, select the appropriate check box:

   - **Basic User**: All users must have this role selected.
   - **System Administrator**: Only for users who need admin privileges.
   - Appropriate Guides role: See [role types](admin-role-types.md).

    ![Author and Operator check boxes.](media/select-role-1.png "Author and Operator check boxes")

1. Select **Save**.

## Next step

- [Set up a Guides device license for multiple operators](device-license.md)
- Contact your Guides users to have them [install the PC app and set up their HoloLens](install-pc-hololens-apps.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
