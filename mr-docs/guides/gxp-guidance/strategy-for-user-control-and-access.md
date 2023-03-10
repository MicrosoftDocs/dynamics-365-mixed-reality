---
title: Strategy for user control and access
description: Learn about restricting access and user controls
ms.date: 03/09/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
---

# Strategy for user control and access

When you implement Guides, we recommend your organization considers how to take control of users and their access. What a user can access and do in Guides on PC and HoloLens is impacted by the business unit, [owner teams](/power-apps/developer/data-platform/use-access-teams-owner-teams-collaborate-share-information), and security roles assigned to the user.

[Security roles](/customerengagement/on-premises/admin/security-roles-privileges#security-roles) provides users with privileges to perform certain actions. The Guides application has two primary security roles, [Author and Operator](/guides/admin-role-types), that can be [assigned to users](/guides/assign-role). As a default, these roles supply access on an Organization-level, the highest level of access. Therefore, all available guides in the environment are visible to users with the role assigned unless individual restrictions to the specific users have been set. However, in a regulated industry setting, you will likely deviate from the default settings or roles. In these cases, you can do the following:

1. [Modify existing security roles](customerengagement/on-premises/admin/create-edit-security-role?view=op-9-1#edit-a-security-role) directly.

1. Modify existing security indirectly by [copying an existing security role](/customerengagement/on-premises/admin/create-edit-security-role#create-a-security-role-by-copy-role) and [editing the copy role](/customerengagement/on-premises/admin/create-edit-security-role#edit-a-security-role).

1. [Create a new security role](/customerengagement/on-premises/admin/create-edit-security-role#create-a-security-role).

The specific access settings you set depends on your business requirements, but could, for instance, restrict access from organization-level to business unit-level. When modifying existing security roles, we recommend indirectly (option 2) rather than directly (option 1). If you modify the existing security roles directly, there is an increased risk that your customizations are reset to default settings when an update to the Guides application has been deployed. However, whether modifying through option 1 or 2, we recommend you verify that your customizations are still in place after updating the Guides solution.

In addition to the security roles, your organization can restrict and control access from more perspectives – for instance, security aspects like business units and owner teams.

As each user can only be assigned to one business unit, specific users can be included in owner teams belonging to other business units if the user has cross-organizational duties in relation to Guides.  
  
By utilizing the default team in Dataverse for business unit, you can link to an Active Directory Group ensuring that only access is given through proper Identity and Access Management (IAM) assignment within the organization.
