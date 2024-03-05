---
title: Share a guide or folder in Dynamics 365 Guides
description: Learn how to share a guide or folder in Microsoft Dynamics 365 Guides by using an access team.
author:  davepinch
ms.topic: how-to
ms.date: 02/26/2024
ms.author: davepinch
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Share a guide or folder in Dynamics 365 Guides

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

You can share a guide or a folder through the model-driven app. For more information, see [Guide content management.](admin-content-mgmt.md)

## Share a folder

By organizing all guides and assets a user might need into a folder, you can share the folder rather than having to share the guide or the assets individually.

> [!NOTE]
> By default, Authors and Restricted authors have access to all assets (3D parts, images, videos, and object anchors). Although not recommended, admins can restrict access by creating a new security role. See [Restrict access to assets.](admin-restrict-access-assets.md)

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. In the left pane, select **Folders** to view the list of folders in the environment.

1. Select the desired folder, and then at the top right of the screen, select **Share** > **Copy link**.

   :::image type="content" source="media/share-folder.png" alt-text="Screenshot showing Share and copy link.":::

1. Share the link with the appropriate users.

## Share a guide

You can share a guide with other users if you're an administrator or if you have the Share privilege. Share a guide with a specific user or an [access team](admin-access-teams.md).

> [!IMPORTANT]
> [Assigning ownership of a guide](admin-access-assign.md) to a user or team is the preferred method for controlling who can use specific guides. Sharing a guide does not change ownership of the guide.

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. Find the guide that you want to share, select the check box next to the guide name, and then select **Share**.

   :::image type="content" source="media/share-guide.png" alt-text="Screenshot showing a selected guide and the Share button highlighted.":::

1. On the **Share records** page, use the search box to find and select the appropriate team or user name.

1. Under **Manage share access**, select the team, and then select specific permissions:

   - For operators, select **Read** permissions (and **Append to** if you want to [collect operations data](../guides/analytics-overview.md)).
   - For authors, select **Read**, **Write**, **Append**, and **Append to** permissions.

     :::image type="content" source="media/manage-share-access.jpg" alt-text="Screenshot showing Manage share access to select permissions to share a guide.":::

1. Select **Share**.

   > [!NOTE]
   > When you share a guide, the content (images, videos, and 3D objects) associated with the guide is not automatically shared. To share the contents, go to the next step.

## Share specific content of a guide

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. Find the guide that you want to share and open it.

1. Select the **All Content** tab.

1. Scoll to the content you want to share and select it. You can select more than one item.

1. Select the **More (ellipsis ...)** button, and then select **Share**.

   :::image type="content" source="media/mda-all-content-tab.PNG" alt-text="Screenshot of All Content tab in the Guides model-driven app with video selected and Share command highlighted.":::

1. On the **Share records** page, use the search box to find and select the appropriate team or user name.

1. Under **Manage share access**, select the team, and then select specific permissions:

   - For operators, select **Read** permissions (and **Append to** if you want to [collect operations data](analytics-overview.md)).
   - For authors, select **Read**, **Write**, **Append**, and **Append to** permissions.

     :::image type="content" source="media/manage-share-access.jpg" alt-text="Screenshot showing Manage share access to select permissions to share content.":::

1. Select **Share**.

## Next steps

- [Assign an Operator or Author role to an individual user](assign-role.md)
- [Assign roles in bulk by using Microsoft Entra groups](admin-assign-role-groups.md)
- [Restrict access to an environment by using security groups](admin-security.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
