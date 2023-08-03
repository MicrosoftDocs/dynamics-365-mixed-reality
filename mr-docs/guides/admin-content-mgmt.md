---
title: Guide content management
description: Learn about assigning ownership or sharing a folder or a guide in Microsoft Dynamics 365 Guides.
author:  annitachow
ms.topic: conceptual
ms.date: 07/31/2023
ms.author: anchow
ms.reviewer: v-wendysmith
---

# Guide content management

Authors or admins can organize guides and their assets (3D parts, images, videos, and object anchors) into folders. Then, assign owners to the folders or share them with others. If you don't need the benefits of a folder structure, you can assign guides to an individual or team.

Assigning ownership of a folder or guide to a user or team is the preferred method for controlling who can use specific guides. Sharing a guide doesn't change ownership of the guide.

For example, if you have multiple users that need access to a guide and its assets:

- Create a team for those users.
- Create a folder and add the guide and all its assets. Assign the team as owners to the folder.

## Folder ownership and access

Authors can organize their guides and the content of their guides by creating folders. Folders can contain:

- Subfolders
- Guides
- Images
- 3D Objects
- Videos  
- Object anchors  

Folders can be organized to contain all the contents needed for one guide or multiple guides if you have a set of guides that need to be shared or grouped. There can also be other folders nested under a parent folder to create a hierarchy of folders.

When you create a folder in Microsoft Dynamics 365 Guides, you assign an owner to the folder. Owners have access to all items in that folder and its subfolders. You can assign ownership of the folder to another person or team, or keep ownership and share the folder.

> [!NOTE]
> By default, Authors and Restricted Authors have access to all assets. If you don't assign a folder to a user, but the user has access to an asset, the user can see the asset in the PC App and use them, but the folder properties for that asset won't display.

## Guide ownership and access

When you create a guide in Microsoft Dynamics 365 Guides, you're automatically assigned as the owner of the guide. You can assign ownership of the guide to another person or team. To keep ownership of the guide but let someone else work on it with you, use the **Share** option.

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

- [Change ownership of a guide or folder](admin-access-assign.md)