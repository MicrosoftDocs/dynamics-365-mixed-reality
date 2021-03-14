---
title: "Assign Author and Operator roles to a Dynamics 365 Group Team that is linked to an Azure Active Directory Group to limit the actions of a group of users in all Dynamics 365 Guides | MicrosoftDocs"
description: How to Assign Author and Operator roles to a Dynamics 365 Group Team that is linked to an Azure Active Directory Group.
author:  v-mhoag
manager: anhaman
ms.service: Guides
ms.component: pa-user
ms.topic: conceptual
ms.date: 03/12/2021
ms.author: v-mhoag
ms.custom: ""
ms.reviewer: ""
ms.assetid: 
search.audienceType: 
  - enduser
search.app: 
  - Guides
  - PowerApps
  - D365CE
---
<!-- comment -->

# Assign Author and Operator roles to a Dynamics 365 Group Team that is linked to an Azure Active Directory Group.

## Operator and Author roles for individual users ##

You can assign an **Operator** or **Author** role to individual users to specify whether that user can create and edit guides or just use them. When you assign an **Operator** or **Author** role, that role automatically grants the user access to all guides in the instance. To limit access to specific guides or guide content (3D models, images, or videos), you can use the **Restricted Author** and **Restricted Operator** roles that are already set up in your Guides solution. Users who are assigned one of these roles will have access only to guides that they create themselves, guides/content that is explicitly shared with them or guides shared with one of their teams.


For information on the Author and Operator roles for D365 Guides [How access teams work with the Operator and Author user role](https://docs.microsoft.com/en-us/dynamics365/mixed-reality/guides/admin-access-teams#how-access-teams-work-with-the-operator-and-author-user-roles)


## Assigning Roles to groups of users ##

It is common for organizations to use Azure Active Directory to organize users into logical groups for easier management.  We assume your organization has created an Azure Active Directory Group to organize the users who will work as guide authors or guide operators.  See:  [Creating a basic group and add members - Azure Active Directory]( https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)

For an overview of Groups see the community article : 
[Groups in Microsoft 365 and Azure, and Which is Right for You](https://docs.microsoft.com/en-us/microsoft-365/community/all-about-groups)

By linking an Azure Active Directory group to a Dynamics Team, Dynamics365 Guides roles can be inherited by any user added to the Azure Active Directory Group.

### Create an Azure Active Directory Group ###
 
Create an Azure Active Directory Security Group or an Azure Active Directory Office Group. See: [Create a basic group and add members - Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal) 

### Create a Dynamics365 Group Team ###

Azure Active Directory Groups are either Office or Security Groups.  Depending on which type of Azure Active Directory Group was used, create a Dynamics365 Azure Active Directory Security Group Team or an Azure Active Directory Office Group Team. See: [Create and manage group teams - Power Platform](https://docs.microsoft.com/en-us/power-platform/admin/manage-group-teams#create-a-group-team)  

The Dynamics365 Team can be linked to the Azure Active Directory Group that is used to manage your users.   Roles can be assigned to this team. 

### Assign D365 Guides Roles to the Team - Option 1 ###

Update the D365 Guides roles to include the D365 Group Team that was created in the step above using the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments).

1. select the environment to update and access the settings. 
2. In the “Access” section, select “See All” under the security roles heading. 
3. The “Basic User” role must be added to the group to enable D365 Guides for the users in this group team.   
4. Click on the role name “Basic User” to see more detail. 
5. Click on the “Add people” action button at the top of the view. 
6. Search for the Dynamics 365 Group Team created in Step 1 above. Select the Group Team when it is shown in the search results and select “add” to confirm. 
7. Select the [Dynamics 365 Guides role](https://docs.microsoft.com/en-us/dynamics365/mixed-reality/guides/assign-role)    that is to be applied to this team to see more detail:  
- Dynamics 365 Guides Author 
- Dynamics 365 Guides Operator
- Dynamics 365 Guides Restricted Author
- Dynamics 365 Guides Restricted Operator

8. Click on the role name  to see more detail.
9. Click on the “Add people” action button at the top of the view.

10. Search for the Dynamics 365 Group Team created in above. Select the Group Team when it is shown in the search results and select “add” to confirm.

Repeat the above steps for any additional roles that are to be applied to the Group Team 

### Assign D365 Guides Roles to the Team - Option 2 ###

Update the D365 Guides roles to include the D365 Group Team that was created in the step above using the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments).  See  [Add roles to group teams](https://docs.microsoft.com/en-us/power-platform/admin/manage-teams) 

1. Select the name of the environment to update and access the settings.
2. In the detail page of the environment, click on Environment URL link to access the details of the environment.  
3. In the title bar select the gear icon then select “Advanced Settings” .  
4. In top menu bar  click caret to the right of “Settings” and  click “Security” from the System’s column.
5. Select “Teams”  
6. Choose team type from the drop down at the top of the page (All Azure Active Directory (AAD) Office Group Teams, or All AAD Security Group Teams).
7. When the team to be updated is shown, click on the team name link to modify the team.
8. At the top of the page, the “manage roles” options is available.

Note: the “manage roles” button at the top will not be shown as an option on the list of group teams page  if the checkbox to the left of a group team is selected.  Manage roles is only available when in the context of the group team details page.  

Example: If the steps above were completed to apply the author role to an AAD Office Group, then anyone in the group will have a role that will allow them to create a Guide and Guide will be owned by group referenced in the first step allowing access and edit privileges. 


[!INCLUDE[footer-include](../includes/footer-banner.md)]