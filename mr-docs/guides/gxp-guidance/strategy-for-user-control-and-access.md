---
title: User control and access strategy
description: Learn about restricting access and user controls.
ms.date: 03/23/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# User control and access strategy

When you implement Dynamics 365 Guides, we recommend your organization considers how to take control of users and their access. What a user can access and do in Guides on PC and HoloLens is impacted by the business unit, [owner teams](/power-apps/developer/data-platform/use-access-teams-owner-teams-collaborate-share-information), and security roles assigned to the user.

[Security roles](/dynamics365/customerengagement/on-premises/admin/security-roles-privileges) provides users with privileges to perform certain actions. The Guides application has two primary security roles, [Author and Operator](../admin-role-types.md), that can be [assigned to users](../assign-role.md). As a default, these roles supply access on an Organization-level, the highest level of access. Therefore, all available guides in the environment are visible to users with the role assigned unless individual restrictions to the specific users have been set. However, in a regulated industry setting, you will likely deviate from the default settings or roles. In these cases, you can:

- [Modify existing security roles](/dynamics365/customerengagement/on-premises/admin/create-edit-security-role#edit-a-security-role) directly.
- Modify existing security indirectly by [copying an existing security role](/dynamics365/customerengagement/on-premises/admin/create-edit-security-role#create-a-security-role-by-copy-role) and [editing the copy role](/dynamics365/customerengagement/on-premises/admin/create-edit-security-role#edit-a-security-role).
- [Create a new security role](/dynamics365/customerengagement/on-premises/admin/create-edit-security-role).

The specific access settings you set depends on your business requirements, but could, for instance, restrict access from organization-level to business unit-level. When modifying existing security roles, we recommend indirectly rather than directly. If you modify the existing security roles directly, there is an increased risk that your customizations are reset to default settings when an update to the Guides application has been deployed. However, whether modifying directly or indirectly, we recommend verifying that your customizations are still in place after updating the Guides solution.

In addition to the security roles, your organization can restrict and control access from more perspectives, such as security aspects like business units and owner teams.

As each user can only be assigned to one business unit, specific users can be included in owner teams belonging to other business units if the user has cross-organizational duties in relation to Guides.  
  
By utilizing the default team in Dataverse for business unit, you can link to an Active Directory Group ensuring that only access is given through proper Identity and Access Management (IAM) assignment within the organization.

## Next steps

- [Strategy for access control and IAM](strategy-for-access-control-and-iam.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
