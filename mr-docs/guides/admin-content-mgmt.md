---
title: Guide content management
description: Learn about assigning ownership or sharing a folder or a guide in Microsoft Dynamics 365 Guides.
author:  annitachow
ms.topic: conceptual
ms.date: 07/19/2023
ms.author: anchow
ms.reviewer: v-wendysmith
---

# Guide content management

Guides and their assets (3D parts, images, videos, and object anchors) can be assigned owners or shared with other in your organization. If you organized your guides and their assets into folders, you can assign ownership to the folder. If you don't have your guides and assets organized into folders, you can assign ownership to a guide.

> [!NOTE]
> By default, Authors and Restricted authors have access to all assets unless otherwise specified. Admins can restrict access by managing permissions or creating a new security role. See [Restrict access to assets](admin-restrict-access-assets.md).

## Folder ownership and access

When an admin or author creates a folder in Microsoft Dynamics 365 Guides, they assign an owner to the folder. You can add guides, assets, and subfolders to the new folder. Admins and authors have access to all items in that folder and its subfolders.

Admins and authors can assign ownership of the folder to another person or team, or keep ownership and share the folder.

## Guide ownership and access

When you create a guide in Microsoft Dynamics 365 Guides, you're automatically assigned as the owner of the guide. If you want to share ownership of the guide with others in your organization, you can:

Assign ownership of the guide to another person or team, or keep ownership of the guide, but let someone else work on it with you by using the **Share** option.

> [!NOTE]
> You can also assign the ownership of a guide to yourself if you have a role with the Assign privilege. You must be a system administrator to re-assign ownership of a guide that belongs to someone else.

For more information on privileges, teams, and controlling access to apps, see the following articles.

|To|See this article|
|---------------------------------------|-----------------------------------------------------|
|Learn how privileges and access work| [How access to a record (guide) is determined](/power-platform/admin/how-record-access-determined)|
|Learn about the three types of teams (*owner* team, Azure Active Directory *group* team, or *access* team)|[Manage teams](/power-platform/admin/manage-teams)|
|Control access to the Dynamics 365 Guides HoloLens app or PC app|[Security roles and privileges](/power-platform/admin/security-roles-privileges#team-members-privilege-inheritance)|
|Control access to the Guides model-driven app| [Share a model-driven app using Power Apps](/powerapps/maker/model-driven-apps/share-model-driven-app)|

## Next steps

- [Assign owner of a guide or folder](admin-access-assign.md)