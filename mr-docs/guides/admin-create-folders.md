---
author: annitachow
description: Learn how to organize guides and assets into folders in Dynamics 365 Guides.
ms.author: anchow
ms.date: 07/24/2023
ms.topic: how-to
title: Create folders in Dynamics 365 Guides to organize your guides and assets
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Create folders in Dynamics 365 Guides to organize your guides and assets

Authors can organize their guides as well as the content of their guides by creating folders. A folder can contain guides, subfolders, and assets (3D parts, images, videos, and object anchors). You can create a hierarchy of folders with subfolders. Each folder can be assigned an owner. When you delete a folder, all items in that folder are also deleted.

Folders are a great way to organize guides and their content especially if you have multiple assets that are all associated with a particular guide or set of guides.

## Prerequisites

- Guides Admin or Author role

## Create a folder

1. [Open the model-driven app](open-model-driven-app.md) in Guides to manage folders.

1. In the left pane, select **Folders** to view all folders created in the instance, and then, at the top of the screen, select **New** to create a new folder.

    ![Folders command highlighted in left pane.](media/folders-command.PNG "Folders command highlighted in left pane")

1. In the **New Folder** screen, enter the name and owner of the folder. You can select an existing folder in the **Parent Folder** field, or leave the **Parent Folder** field blank to create a folder at the root level.

    ![New command highlighted at top of Power Apps screen.](media/folders-new.PNG "New command highlighted at top of Power Apps screen")

1. At the top of the screen, select **Save & Close** to save the folder and return to the folder list. After saving, you can add guides, subfolders, or assets to the folder.

## Add a guide or asset to a folder

1. In the left pane of the model-driven app, under **Content** select Guides or the type of asset you want to add.

   > [!NOTE]
   > 3D parts in the **Toolkit** can't be added to folders.

1. Then, select the particular guide or asset you want to add to the folder. You can search or filter for the particular item.

1. On the **General** tab, in the **Parent Folder** field, enter the folder name or search for it.

    ![General tab and Parent Folder field highlighted.](media/folders-general-tab.PNG "General tab and Parent Folder field highlighted")

1. At the top of the screen, select **Save** or **Save & Close**.

> [!TIP]
> To move a guide or asset back to the root folder, return to the guide details and delete the contents of the **Parent Folder** field.

You can also upload assets to a folder in the PC app.

- [Import a custom 3D model to use as a 3D part.](pc-app-add-3D-part.md#import-a-custom-3d-model-to-use-as-a-3d-part)
- [Import an image or video](pc-app-add-media.md#import-an-image-or-video)

## View the contents of a folder

1. In the left pane, select **Folders** to view the list of folders in the instance.

1. Select the desired folder. All active folders, guides, images, 3D models, videos, and object anchors in the folder display.

## Next steps

- [Create or find a guide](create-guide.md)
- [Move your folder structure from one environment to another](admin-export-import-folders.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
