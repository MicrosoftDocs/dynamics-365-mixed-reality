

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


