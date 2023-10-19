---
author: davepinch
description: Add additional user accounts to a Microsoft Dynamics 365 Guides license.
ms.author: davepinch
ms.date: 02/01/2023
ms.topic: how-to
title: Add users in Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# Add users to Dynamics 365 Guides

To add additional users to Microsoft Dynamics 365 Guides, you must first assign the Dynamics 365 Guides license to a new or existing user in the Microsoft 365 admin center. Then, in the Power Platform admin center, configure the roles that the users will have access to (Author, Operator, or Admin).

## Add a new user

1. Open the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home).

1. [Add a user](/microsoft-365/admin/add-users/add-users).

   - For **Licenses**, select **Dynamics 365 Guides**.

   - For **Optional settings**, leave the **User (no administrator access)** check box selected unless the user will be an admin. In that case, select the **Global administrator** check box.

   - If you selected the **Automatically create a password** option, make a note of the password. The user will need this password to sign in.

After you add user accounts, the next step is to assign the **Author**, **Operator**, or **Admin** user role for the solution. For more information, see [Assign user roles](assign-role.md).

## Assign a Dynamics 365 Guides license to an existing user

1. Open the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home).

1. [Assign licenses to users](/microsoft-365/admin/manage/assign-licenses-to-users#use-the-active-users-page-to-assign-licenses).

   - Select **Dynamics 365 Guides**. Then, under **Apps**, make sure that the **Common Data Service**, **Dynamics 365 Guides**, and **PowerApps for Dynamics 365 Mixed Reality** check boxes are selected.

## Add a guest user

Anyone who is not part of your organization, but has a Microsoft Entra account, can be added as a guest by a global admin. The user can then access Dynamics 365 Guides content in your organization as an operator. [Learn about adding a guest user in Dynamics 365 Guides.](../guides/admin-add-guest-user.md)

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

## Next steps

- [Assign user roles](assign-role.md)
- [Add a guest user](admin-add-guest-user.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
