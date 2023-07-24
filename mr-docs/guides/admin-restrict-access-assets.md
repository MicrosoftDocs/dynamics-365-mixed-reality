---
title: Restrict access to certain assets in Dynamics 365 Guides
description: Learn how to restrict access to specific assets Microsoft Dynamics 365 Guides.
author:  annitachow
ms.topic: how-to
ms.date: 07/24/2023
ms.author: anchow
ms.reviewer: v-wendysmith
---

# Restrict a security role's access to certain asset types

Admins can restrict access to certain assets by managing permissions through security roles in the Power Platform admin center.

## Prerequisites

- You must have an active Dynamics 365 Guides license. For more information, see [Buy a subscription or sign up a free trial](setup-step-one.md).

- The latest Dynamics 365 Guides solution must be installed. For more information, see [Update to the latest solution](upgrade.md).

- You must have access to the Microsoft Power Platform admin center and have full admin privileges.


1. Open the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), select the Guides solution in the **Environments** page, and then select **Settings**.

   add image

1. In the **Settings** page, select **Security roles**. Select the specific security role.

1. Select the user you want to restrict access.

1. Under **Custom Tables**, select the asset type (3D object, images, videos, or object anchors). Change the permissions on Create, Read, Write, Append and AppendTo to User.  