---
title: "Assign Author and Operator roles to a Dynamics 365 Group Team that is linked to an Azure Active Directory Group to limit the actions of a group of users in all Dynamics 365 Guides | MicrosoftDocs"
description: How to Assign Author and Operator roles to a Dynamics 365 Group Team that is linked to an Azure Active Directory Group.
author:  MattHoag-MS
manager: anhaman
ms.service: crm-online
ms.topic: article
ms.date: 04/14/2021
ms.author: v-mhoag
ms.reviewer: v-bholmes
---

# Assign Author and Operator roles to a Dynamics 365 Group Team linked to an Azure Active Directory Group

You can assign an **Operator** or **Author** role to a user to specify whether that user can create and edit guides as an author or use them as an operator.  When you assign an **Operator** or **Author** role, that role automatically grants the user access to all guides in the instance. To limit access to specific guides or guide content (3D models, images, or videos), you can use the **Restricted Author** and **Restricted Operator** roles. **Restricted Authors** have access only to what they have created in the instance, while **Restricted Operators** have access only to what has been shared with or assigned to them.

Users with the roles of **Restricted Author** and **Restricted Operator** will only have access to:

- Guides/content that the user created (unless access was explicitly removed)

- Guides that were explicitly shared with them or shared with an owner team they are a member of

- Guides that were assigned to the user or assigned to an owner team that the user is a member of

## Assign roles to groups of users

You can use Azure Active Directory to organize users into logical groups for easier management. By linking Azure Active Directory Security or Office groups to a Dynamics Team, Dynamics 365 Guides roles can be inherited by any user added to the Azure Active Directory Group. To get an overview of Azure Active Directory groups and managing group teams, see the following links:

- [Groups in Microsoft 365 and Azure, and Which is Right for You](https://docs.microsoft.com/microsoft-365/community/all-about-groups)

- [Manage group teams](https://docs.microsoft.com/power-platform/admin/manage-group-teams)

> [!NOTE]
> SharePoint groups are not supported by Dynamics 365.  Only Azure Active Directory Office or Security groups are supported by Dynamics 365 Group Teams.

### Create an Azure Active Directory group

To learn how to create an Azure Active Directory Security group or an Azure Active Directory Office group, see [Create a basic group and add members using Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal).

### Create a Dynamics 365 Group Team

Azure Active Directory Groups that can be used with Dynamics 365 are either Office or Security Groups.  Depending on which type of Azure Active Directory Group was used, create a Dynamics 365 Azure Active Directory Security Group Team or an Azure Active Directory Office Group Team. See: [Create and manage group teams - Power Platform](https://docs.microsoft.com/power-platform/admin/manage-group-teams#create-a-group-team)  

The Dynamics 365 Team can be linked to the Azure Active Directory Group that is used to manage your users. D365 Guides roles can be assigned to this team. Members of the Azure Active Directory Group will inherit the roles from the Dynamics 365 Team.

For more information on how to link an AAD Group to a Dynamics 365 Team see the [Manage group teams - Power Platform](https://docs.microsoft.com/power-platform/admin/manage-group-teams).  When setting a value for  **membership type** by selecting one of the options (Members/Members&Guests/Guests/Owners) be aware that this determines which users in the group will flow into the Dynamics 365 team.  Setting the **membership type** is similar to setting a pass-through filter. If membership type: “members” is selected and a guest is added to the group, the guest will not flow down into a team that has a membership type of “members”.  This guest will not inherit the role from the Dynamics 365 Group Team.  

Two options are available for assigning roles to a team.  

- Option 1 is to **add people** to a role using groups.  In this case these additions must be made to the Basic User role and any additional roles that are to be modified.  This is the best option if many Dynamics 365 Group Teams need to have a role assigned.
- Option 2 is to modify the Dynamics 365 Group Team to **add one or more roles**.  This is the best option if a small number of Dynamics 365 Group Teams require modification.

### Option 1: Assign a Group Team to a Dynamics 365 Guides Role

Update a role to include the Dynamics 365 Group Team that was created in the step above using the [Power Platform admin centre](https://admin.powerplatform.microsoft.com/environments).

1. Select the environment to update and access the settings.
1. In the “Access” section, select “See All” under the security roles heading.
 ![power platform admin](media/Power-Platform-admin-center-env-setting.png "power platform admin")
1. The “Basic User” role must be added to the group to enable Dynamics 365 Guides for the users in this group team.
1. Click on the role name “Basic User” to see more detail.
![basic user](media/Power-Platform-Enviro-Roles.png "basic users")
1. Click on the “Add people” action button at the top of the view.
    ![add people](media/Power-Platform-security-role-add-people.png "Add people")
1. Search for the Dynamics 365 Group Team created in Step 1 above. Select the Group Team when it is shown in the search results and select “add” to confirm.
 ![add group](media/Power-Platform-security-add-group.png "Add group")
1. Repeat the steps above for the [Dynamics 365 Guides role](https://docs.microsoft.com/dynamics365/mixed-reality/guides/assign-role) that is to be applied to this team. Guides roles include:
    - Dynamics 365 Guides Author
    - Dynamics 365 Guides Operator
    - Dynamics 365 Guides Restricted Author
    - Dynamics 365 Guides Restricted Operator

1. Click on the role name  to see more detail.
1. Click on the “Add people” action button at the top of the view.

1. Search for the Dynamics 365 Group Team created in above. Select the Group Team when it is shown in the search results and select “add” to confirm.

Repeat the above steps for any additional roles that are applied to the Group Team.

### Option 2: Assign Dynamics 365 Guides Roles to a Group Team

Update the Dynamics 365 Guides roles to include the Dynamics 365 Group Team that was created in the step above using the [Power Platform admin centre](https://admin.powerplatform.microsoft.com/environments).  See [Add roles to group teams](https://docs.microsoft.com/power-platform/admin/manage-teams).

1. Select the name of the environment to update and access the settings.
1. In the detail page of the environment, click on Environment URL link to access the details of the environment.  
![click url](media/Power-Platform-admin-center-env-url.png "click url")
1. In the title bar select the gear icon then select “Advanced Settings”.
![select gear](media/Power-Platform-admin-center-env-adv-settings.png "select gear")  
1. In top menu bar click caret to the right of “Settings” and click “Security” from the System’s column.
![select security](media/D365-admin-center-advanced-settings-security.png "select security")
1. Select “Teams”.
![select teams](media/D365-admin-center-advanced-settings-teams.png "select teams")
1. Choose team type from the drop down at the top of the page (All Azure Active Directory (AAD) Office Group Teams, or All AAD Security Group Teams).
 ![select groups dropdown](media/D365-admin-center-advanced-settings-groups.png "select groups dropdown")
1. When the team to be updated is shown, click on the team's name link to modify the team.
![select group name](media/D365-admin-center-advanced-settings-groupname.png "select group name")
1. At the top of the page, the “manage roles” option is available.
![select manage roles](media/D365-admin-center-advanced-settings-manage-roles.png "manage roles")

Note: the “manage roles” button at the top will not be shown as an option on the list of group teams page if the checkbox to the left of a group team is selected.  Manage roles is only available in the context of the group team details page.  

Example: If the steps above were completed to apply the author role to an AAD Office Group, then anyone in the group will have a role that will allow them to create and edit a guide and the guide will be owned by the group referenced in the first step allowing access and edit privileges.
