

# Organize guides into folders in Dynamics 365 Guides (for admins)

As an admin, you can organize guides into folders for easier management of permissions. A folder may contain guides and sub-folders, and each folder can be assigned an owner that is inherited by child items in that folder. Folders are useful for managing groups of guides with the same permissions, such as guides for a specific team or product. When deleting a folder, all items in that folder are also deleted, recursively.

> [!IMPORTANT]
> For the May 4 release, you can create folders and set permissions for those folders if you're an admin. The folders won't appear in the HoloLens and PC apps, however, until a later release.

## Create a folder

1.	Sign in to the instance by using your admin credentials.
<<same tip as on https://docs.microsoft.com/en-us/dynamics365/mixed-reality/guides/admin-deactivate-guide>>

2.	In Power Apps, select the **Guides** app tile.
<<same screenshot as above>>

3.	In the left pane, select **Folders** to view all folders created in the instance.

    SCREEN SHOT GOES HERE 

4.	At the top of the screen, select **New** to create a new folder.

    SCREEN SHOT GOES HERE 

5.	Enter the name and owner of the folder. You can also select an existing folder as the **Parent Folder**, or leave blank to create a folder at the root level.

6.	Select **Save & Close** on the toolbar to save the folder and return to the folder list. After saving, you can add guides and subfolders to the folder.

## Add a guide to a folder

1.	In the left pane, select **Guides**, and then locate the guide you want to add to the folder.

    SCREEN SHOT GOES HERE

2.	On the **General** tab, in the **Parent Folder** field, enter the parent folder name or search for it.

3.	At the top of the screen, select **Save** or **Save & Close**.

> [TIP]
> To move a guide back to the root folder, return to the guide details and delete the contents of the **Parent Folder** field.

## Change the owner of a folder

When you change the owner of a folder, any guides or subfolders within that folder will be assigned to that owner. This allows you to easily manage access for a group of related guides.

To change the owner of a folder:

1.	In the left pane, select **Folders** to view the list of folders in the instance.

2.	Go to the desired folder, and then at the top of the screen, select the **Assign** button to display the folder information.

    SCREEN SHOT GOES HERE

3.	In the **Assign Folder** dialog box, select the box to the right of the **Assign to** label to toggle between **Me** and **User or team**. If **Me** is selected, the folder is assigned to you. If **User or team** is selected, you can enter the owner in the **User or team** field or search for an owner.

    SCREEN SHOT GOES HERE

4.	Select **Assign** to save the new owner. 
