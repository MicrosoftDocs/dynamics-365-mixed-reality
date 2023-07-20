---
author: annitachow
description: Learn how to organize guides and assets into folders in Dynamics 365 Guides.
ms.author: anchow
ms.date: 07/19/2023
ms.topic: how-to
title: Create folders in Dynamics 365 Guides to organize your guides and assets
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Create folders in Dynamics 365 Guides to organize your guides and assets

Authors can organize their guides as well as the content of their guides by creating folders. A folder can contain guides, subfolders, and assets (3D parts, images, videos, and object anchors). Folders can be organized to contain all the contents needed for one guide or multiple guides. You can create a hierarchy of folders with subfolders. Each folder can be assigned an owner. When you delete a folder, all items in that folder are also deleted.

[Open the model-driven app](open-model-driven-app.md) in Guides to manage folders.

## Prerequisites

- Guides Admin or Author role

## Create a folder

1. In the left pane, select **Folders** to view all folders created in the instance, and then, at the top of the screen, select **New** to create a new folder.

    ![Folders command highlighted in left pane.](media/folders-command.PNG "Folders command highlighted in left pane")

1. In the **New Folder** screen, enter the name and owner of the folder. You can select an existing folder in the **Parent Folder** field, or leave the **Parent Folder** field blank to create a folder at the root level.

    ![New command highlighted at top of Power Apps screen.](media/folders-new.PNG "New command highlighted at top of Power Apps screen")

1. At the top of the screen, select **Save & Close** to save the folder and return to the folder list. After saving, you can add guides, subfolders, or assets to the folder.

## Add a guide or asset to a folder

1. In the left pane, under **Content** select the guide or type of asset you want to add. Then select the particular guide or asset you want to add to the folder.

1. On the **General** tab, in the **Parent Folder** field, enter the folder name or search for it.

    ![General tab and Parent Folder field highlighted.](media/folders-general-tab.PNG "General tab and Parent Folder field highlighted")

1. At the top of the screen, select **Save** or **Save & Close**.

> [!TIP]
> To move a guide or asset back to the root folder, return to the guide details and delete the contents of the **Parent Folder** field.

## View the contents of a folder

1. In the left pane, select **Folders** to view the list of folders in the instance.

1. Select the desired folder. The list of active folders, guides, images, 3D models, videos, and object anchors display.

## Next steps

- [Create or find a guide](create-guide.md)
- [Move your folder structure from one environment to another](admin-export-import-folders.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
