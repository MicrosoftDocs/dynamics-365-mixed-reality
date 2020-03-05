

# Use access teams to limit access to specific guides and guides content in Dynamics 365 Guides

A Microsoft Dynamics 365 administrator can use [access teams](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/use-access-teams-owner-teams-collaborate-share-information) 
to easily customize who can see specific guides and guides content (3D models, images, or videos) in Dynamics 365 Guides. Access teams 
are useful when you want to grant different user permissions for specific records in [Common Data Service](https://docs.microsoft.com/powerapps/maker/common-data-service/data-platform-intro). 
For example, you might want to limit access of certain guides to a specific factory location, or limit access to guides that are in progress.

>[!NOTE]
>Dynamics 365 offers additional ways to customize and configure access to specific records in Common Data Service. Advanced 
configuration, such as the creation of [Owner teams](https://docs.microsoft.com/en-us/dynamics365/customerengagement/on-premises/developer/use-access-teams-owner-teams-collaborate-share-information), 
is not covered in this topic.

## How access teams work with the Operator and Author user roles

You can assign an Operator or Author role to a user to determine whether that user has the ability to create and edit guides or just use them. When you assign an Operator or Author role, that role automatically grants the user access to all guides in the instance. To limit access to specific guides or guides content (3D models, images, or videos), you must reduce privileges for the Operator or Author role and use access teams.

## Overall process for limiting access to a guide

The process for limiting access includes these basic steps:

1.	Create a new security role with reduced privileges.

2.	Grant access for the new security role to the Guides model-driven app.

3.	Assign the new security role to a user or users.

4.	Create an access team and add users to the team.

5.	Share the guide with the access team.

Each of these steps is covered in detail in this document.

## Create a new security role with reduced privileges

To take advantage of access teams, the first step is to create a new Dynamics 365 security role with reduced Guides privileges. A user assigned this new security role will only have access to guides that have been shared with them directly or via an access team.

>[!NOTE]
>This documentation shows how to restrict access to the **Guides** entity. You can use the same steps to restrict access to other types of Dynamics 365 Guides records (3D models, images, or videos) to limit their visibility to certain users or teams.

1.	In the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), on the **Environments** page, choose an environment with an installed Guides solution, select the **More environment actions** (...) button, and then select **Settings**.

    SCREEN SHOT GOES HERE
 
2.	On the **Settings** page, under **Users + permissions**, select **Security roles**.

    SCREEN SHOT GOES HERE
 
3.	Select the check box next to the **Dynamics 365 Guides Operator** role, and then at the top of the screen, select **More Actions > Copy Role**. Copying the role ensures that your changes will not be overridden the next time the Guides solution is updated. 

    SCREEN SHOT GOES HERE 

4.	Name the new role "Dynamics 365 Guides Restricted Operator", and then select **OK**.

    SCREEN SHOT GOES HERE

5.	In the **Security Role: Dynamics 365 Guides Restricted Operator** window, select the **Custom Entities** tab, and then in the **Guides** entity row, select the dot in the second column to change the read privileges from **Organization** level to **User** level. Select **Save and Close** at the top of the window when you’re done.

>[!NOTE]
>The **Key** at the bottom of the window describes the different privilege levels. For more information, see [Security roles and privileges](https://docs.microsoft.com/en-us/dynamics365/customerengagement/on-premises/admin/security-roles-privileges). 

    SCREEN SHOT GOES HERE
