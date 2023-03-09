---
title: 
description: 
ms.date: 03/09/2023
ms.topic: 
ms.service: 
author: 
ms.author: 
manager: 
---

# Strategy for security and separations of environment access

Access to environments and content should be restricted and generally follow a least privilege principle. In Power Platform, this can be handled on different levels.

As mentioned in govern guides through Power Platform environments and Power Apps<u>,</u> you can use different Power Platform environments and user roles with limited access to drive compliance in the life cycle of a guide. This should be implemented by only giving the user access to required environments and by assigning only relevant security roles in these environments. To learn more about security roles, see [Security roles and privileges.](https://learn.microsoft.com/en-us/power-platform/admin/security-roles-privileges)

While planning the setup, decide the extent of automatically assigned access. Determine how the process should integrate with the company's existing practices for controlling assignment of access rights and, for example, integration to the Identity Access Management (IAM) system.

It is recommended to create Azure Active Directory (AD) Security Groups for each environment and assign to the respective environment. The advantage to this is that you can limit access to an environment based on the membership of the specific Security Group. This is done via the [Power Platform admin center.](https://aka.ms/PPAC) Read more about restricting access to an environment in Guides here.

After assignment, only users that are members of the Azure AD Security Groups will be created in the respective Power Platform environments. For more information about assigning Azure AD Security Groups, see [<u>Control user access to environments</u>](https://learn.microsoft.com/en-us/power-platform/admin/control-user-access). Be sure to separate both Test and Production environments and create separate security groups for all environments to specifically control access.

To effectively manage the assignment of security roles, it is advised to create [Owner Teams](https://learn.microsoft.com/en-us/power-apps/developer/data-platform/use-access-teams-owner-teams-collaborate-share-information) that match the personas/[roles](https://euc-word-edit.officeapps.live.com/we/wordeditorframe.aspx?new=1&ui=en%2DUS&rs=en%2DUS&wdenableroaming=1&mscc=1&hid=90CF93A0-E096-6000-0CBA-08E81472FF99&wopisrc=https%3A%2F%2Fnnit.sharepoint.com%2Fsites%2FGxPGuides-MicrosoftNNITCollaborationsite%2F_vti_bin%2Fwopi.ashx%2Ffiles%2F506bcf89cd82467ca3b09ea2cc5f49ff&wdorigin=DocLib&wdhostclicktime=1675755270396&jsapi=1&jsapiver=v1&newsession=1&corrid=510cce6c-fa60-4c7f-a5e2-14bddc424357&usid=510cce6c-fa60-4c7f-a5e2-14bddc424357&sftc=1&cac=1&mtf=1&sfp=1&wdredirectionreason=Unified_SingleFlush&rct=Normal&ctp=LeastProtected#_Access_control_and) relevant for the system. For information about managing teams see [Microsoft Dataverse teams management](https://learn.microsoft.com/en-us/power-platform/admin/manage-teams).

The usage of Owner Teams has two major benefits:

1.  Assigns security roles by leveraging Azure AD Security Groups and linking to existing IAM processes.

2.  Simplifies the assignment process. An author, for example, needs both the Author Role and the Basic User Role to access the required functionality. By assigning the security roles to an Author team, it is possible to give new authors the necessary roles just by adding them to the Owner Team.

![](media/image2.png)

If your organization are utilizing the platform with [<u>Business Units</u>](https://learn.microsoft.com/en-us/power-platform/admin/create-edit-business-units), an Owner Team are automatically created per Business Unit . The Owner Team can be used to assign the proper security roles if this specific Business Unit only contains users for one role, for instance Author(s). However, in many cases, multiple roles are divided into one Business Unit which require additional Owner Teams to be created and assign relevant security roles. Note that each user is per default to be assigned to the one Business Unit as part of the user creation process, but additional access to other Business Units can be done by assigning to specific Owner Team. 

For effective management you need a scalable setup. It is recommended to automate permission management as much as possible. The process should preferably be linked to the IAM system. An example of a high-level process for creating a new Author (where the user has an existing user account):

1.  A request is initiated to create an author via IAM system.

2.  The request is routed through an approval chain.

3.  The user is assigned relevant Azure AD groups:

    1.  Group that gives the user correct licenses, for example, Dynamics 365 Guides license

    2.  Group(s) that gives the user access to relevant Power Platform environments

    3.  Group(s) that gives the user membership of relevant Power Platform teams, which gives user the necessary security roles

4.  User is assigned to the correct Business Unit

    1.  This is normally a manual process but can be automated with Power App and/or Power Automate to ensure consistent assignment and link IAM.

For setups with multiple Business Units, the above process requires that Azure AD security groups are created in each business unit for every role to add the user to the correct teams. Alternatively, the assignment to teams can be done directly in Power Platform.

In case steps are handled directly in Power Platform, it is recommended to create a supporting process to facilitate and eliminate error. For example, implement a Canvas App that can help the administrator assign membership to teams and to assign the user to the correct Business Unit.


