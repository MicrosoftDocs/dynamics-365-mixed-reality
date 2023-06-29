---
author: Mamaylya
description: Learn how to organize guides into folders in Dynamics 365 Guides
ms.author: mamaylya
ms.date: 06/22/2023
ms.topic: how-to
title: Organize guides into folders in Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Create folders in Dynamics 365 Guides to organize your guides

Folders are useful for managing groups of guides with the same permissions, such as guides for a specific team or product. Permissions assigned to folders do not give permissions to guides within those folders, however. A folder can contain guides and subfolders. Each folder can be assigned an owner. When you delete a folder, all items in that folder are also deleted.

## Prerequisites

- Guides admin or author role

## Create a folder

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. In the left pane, select **Folders** to view all folders created in the instance, and then, at the top of the screen, select **New** to create a new folder.

    ![Folders command highlighted in left pane.](media/folders-command.PNG "Folders command highlighted in left pane")

1. In the **New Folder** screen, enter the name and owner of the folder. You can select an existing folder in the **Parent Folder** field, or leave the **Parent Folder** field blank to create a folder at the root level.

    ![New command highlighted at top of Power Apps screen.](media/folders-new.PNG "New command highlighted at top of Power Apps screen")

1. At the top of the screen, select **Save & Close** to save the folder and return to the folder list. After saving, you can add guides and subfolders to the folder.

## Add a guide to a folder

1. In the left pane, select **Guides**, and then locate the guide you want to add to the folder.

1. On the **General** tab, in the **Parent Folder** field, enter the parent folder name or search for it.

    ![General tab and Parent Folder field highlighted.](media/folders-general-tab.PNG "General tab and Parent Folder field highlighted")

1. At the top of the screen, select **Save** or **Save & Close**.

> [!TIP]
> To move a guide back to the root folder, return to the guide details and delete the contents of the **Parent Folder** field.

## Change the owner of a folder

When you change the owner of a folder, any guides or subfolders within that folder will be assigned to that owner. This allows you to easily manage access for a group of related guides.

1. In the left pane, select **Folders** to view the list of folders in the instance.

1. Go to the desired folder, and then at the top of the screen, select **Assign** to display the folder information.

    ![Assign command highlighted at top of screen.](media/folders-assign.PNG "Assign command highlighted at top of screen")

1. In the **Assign Folder** dialog box, select the box to the right of the **Assign to** label to toggle between **Me** and **User or team**. If **Me** is selected, the folder is assigned to you. If **User or team** is selected, you can enter the owner in the **User or team** field or search for an owner.

1. Select **Assign** to save the new owner.

## Next steps

- [Create or find a guide](create-guide.md)
- [Move your folder structure from one environment to another](admin-export-import-folders.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
