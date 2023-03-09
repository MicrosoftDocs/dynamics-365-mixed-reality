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

# Strategy for user control and access 

When you implement Guides, it is recommended your organization considers how to take control of users and their access. What a user can access and do in Guides on PC and HoloLens is impacted by the Business Unit and [Owner Teams](https://learn.microsoft.com/en-us/power-apps/developer/data-platform/use-access-teams-owner-teams-collaborate-share-information) to which the user is assigned as well as the security roles that is assigned to the user.

[Security roles](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/admin/security-roles-privileges?view=op-9-1#security-roles) provides users with privileges to perform certain actions. The Guides application has two primary security roles, [Author and Operator](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/admin-role-types), that can be [assigned to users](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/assign-role). As a default, these roles supply access on an Organization-level, i.e., the highest level of access. Hereby, all available guides in the environment will be visible to users with the role assigned unless individual restrictions to the specific users have been set. However, in a regulated industry setting, you will likely wish to deviate from the default settings or roles. In these cases, you can do the following:

1.  [Modify existing security roles](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/admin/create-edit-security-role?view=op-9-1#edit-a-security-role) directly

2.  Modify existing security indirectly by [copying an existing security role](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/admin/create-edit-security-role?view=op-9-1#create-a-security-role-by-copy-role) and [editing the copy role](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/admin/create-edit-security-role?view=op-9-1#edit-a-security-role)

3.  [Create a new security role](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/admin/create-edit-security-role?view=op-9-1#create-a-security-role)

The specific access settings you set will depend on your business requirements, but could, for instance, be to restrict access from Organization-level to Business Unit-level. When modifying existing security roles, it is recommended to do it indirectly (option 2) rather than directly (option 1): If you modify the existing security roles directly, there is an increased risk that your customizations will be reset to default settings when an update to the Guides application has been deployed. However, whether modifying through option 1 or 2, it is advised to verify that your customizations are still in place after updating the Guides solution.

In addition to the security roles, your organization can restrict and control access from more perspectives – for instance, security aspects like Business Units and Owner Teams.

As each user can only be assigned to one Business Unit, specific users can be included in Owner Teams belonging to other Business Units if the user has cross-organizational duties in relation to Guides.  
  
By utilizing the default Team in Dataverse for Business Unit, this can be linked to an Active Directory Group ensuring that only access is given through proper Identity and Access Management (IAM) assignment within the Organization.


