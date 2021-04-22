

# Organize guides into folders and set permissions in Dynamics 365 Guides 

As an admin, you can organize guides into folders for easier management of permissions. A folder may contain guides and sub-folders, and each folder can be assigned an owner that is inherited by child items in that folder. Folders are useful for managing groups of guides with the same permissions, such as guides for a specific team or product. When deleting a folder, all items in that folder are also deleted, recursively.

Create a folder

1.	Sign in to the instance by using your admin credentials.
<<same tip as on https://docs.microsoft.com/en-us/dynamics365/mixed-reality/guides/admin-deactivate-guide>>

2.	In Power Apps, select the Guides app tile.
<<same screenshot as above>>

3.	Select Folders on the left-side menu to view all folders created on the instance.

 

4.	In the menu above the grid, select New to create a new folder.

 

5.	Specify the name and owner of the folder. You can also select an existing folder as the parent folder, or leave blank to create a root folder.
6.	Select Save & Close on the toolbar to save the folder and return the folder list. Once saved, you can guides and folders to the folder.

Add a guide to a folder

1.	Select Guides from the side menu and locate the guide you want to add to the folder.

 

2.	On the General tab, edit the Parent Folder field to select the parent folder.
3.	Select Save or Save & Close from the toolbar.

Tip: to move a guide back to the root folder, return to the guide details and delete the contents of the Parent Folder field.

Change owner of a folder

When you change the owner of a folder, the guides and sub-folders inherit the same owner. This allows you to easily manage access to a group of related guides.

To change the owner of a folder:

1.	Select Folders from the side menu to view the list of folders on the instance.
2.	Navigate to the desired folder and select the Assign button on the menu above the folder information.

 

3.	The process of changing a folder owner is the same as changing a guide owner. Click the box next to the Assign to label to toggle between “Me” and “User or team”. If “Me” is shown, the folder is assigned to you. If “User or team” is shown, tap the box below it to select the owner.

 

4.	Select the Assign button to save the new owner. 
