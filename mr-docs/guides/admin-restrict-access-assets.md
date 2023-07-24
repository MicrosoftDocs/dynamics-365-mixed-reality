---
title: Restrict access to certain assets in Dynamics 365 Guides
description: Learn how to restrict access to specific assets Microsoft Dynamics 365 Guides.
author:  annitachow
ms.topic: how-to
ms.date: 07/24/2023
ms.author: anchow
ms.reviewer: v-wendysmith
---

# Restrict access to assets

Admins can restrict access to certain assets (3D parts, images, videos, and object anchors) by managing permissions through security roles in the Power Platform admin center. To create a new security role that restricts access, [create a new role](/power-platform/admin/assign-security-roles) and then continue.

## Prerequisites

- You must have an active Dynamics 365 Guides license. For more information, see [Buy a subscription or sign up a free trial](setup-step-one.md).

- The latest Dynamics 365 Guides solution must be installed. For more information, see [Update to the latest solution](upgrade.md).

- You must have access to the Microsoft Power Platform admin center and have full admin privileges.

## Restrict access to an asset

1. Open the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), select the Guides solution in the **Environments** page, and then select **Settings**.

   :::image type="content" source="media/ppa-security-roles.png" alt-text="Screenshot of Power Platform admin center with Settings > Security Roles  highlighted.":::

1. In the **Settings** page, select **Security roles**. Select the specific security role.

1. Under **Custom Tables**, select the asset type (3D object, images, videos, or object anchors). Change the permissions on **Create**, **Read**, **Write**, **Append** and **AppendTo** to **User**.  

   > [!TIP]
   > For Write access, **Write**, **Append** and **AppendTo** are required.

   :::image type="content" source="media/ppa-security-roles-record-level.png" alt-text="Screenshot of Power Platform admin center with Security Roles  showing User permissions.":::

1. Select **Save**.