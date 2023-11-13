---
title: Restrict access to assets
description: Learn how to restrict access to specific assets Microsoft Dynamics 365 Guides.
author:  annitachow
ms.topic: how-to
ms.date: 07/24/2023
ms.author: anchow
ms.reviewer: v-wendysmith
---

# Restrict access to assets

To restrict access to certain assets (3D parts, images, videos, and object anchors) create a [new security role](/power-platform/admin/create-edit-security-role) in the Power Platform admin center.

> [!IMPORTANT]
> We don't recommend restricting access to assets because restricted users only have access to assets they or their team own or if the assets are specifically shared with them. This includes the assets in the **Toolkit** provided in Guides.

## Prerequisites

- You must have Admin permission.

- You must have an active Dynamics 365 Guides license. For more information, see [Buy a subscription or sign up a free trial](buy-guides.md).

- The latest Dynamics 365 Guides solution must be installed. For more information, see [Update to the latest solution](upgrade.md).

- You must have access to the Microsoft Power Platform admin center and have full admin privileges.

## Restrict access to an asset

1. Open the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), select the Guides solution in the **Environments** page, and then select **Settings**.

    ![Screenshot of Power Platform admin center with Settings > Security Roles  highlighted.](media/ppa-security-roles.png "Power Platform admin center with Settings > Security Roles  highlighted")

1. On the **Settings** page, select **Security roles**. Select **New**.

1. Name the new role and fill out the appropriate information. 

1. Under **Custom Tables**, select the asset type (3D object, images, videos, or object anchors) you want to restrict. Set the permissions on **Create**, **Read**, or **Write** to **User**. For Write access, **Append** and **AppendTo** are required.

   > [!TIP]
   > The default, **Organization**, means the asset type is available to all users within the organization.

    ![Screenshot of Power Platform admin center with Security Roles showing User permissions.](media/ppa-security-roles-record-level.png "Screenshot of Power Platform admin center with Security Roles showing User permissions.")

   > [!IMPORTANT]
   > Changing the permissions of the default roles provided by Guides is not recommended and could result in unexpected behavior. Changing permissions on other tables could result in unexpected behavior.

1. Select **Save**.

1. [Assign your restricted users](/power-platform/admin/assign-security-roles) to this new role.