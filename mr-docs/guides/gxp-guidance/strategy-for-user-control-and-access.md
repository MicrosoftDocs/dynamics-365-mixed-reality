---
title: User control and access strategy
description: Learn about restricting access and user control.
ms.date: 03/23/2023
ms.topic: conceptual
author: prashantyvr
ms.author: prashan
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# User control and access strategy

When you implement Dynamics 365 Guides, we recommend that your organization considers how it will control users and their access. The business unit, [owner teams](/power-apps/developer/data-platform/use-access-teams-owner-teams-collaborate-share-information), and security roles that are assigned to a user affect what that user can access and do in Guides on a PC and a HoloLens device.

[Security roles](/dynamics365/customerengagement/on-premises/admin/security-roles-privileges) give users privileges to perform specific actions. The Guides application has two primary security roles that can be [assigned to users](../assign-role.md): [Author and Operator](../admin-role-types.md). By default, these roles grant access at an organization level, the highest level of access. Therefore, all available guides in the environment are visible to users that these roles are assigned to, unless restrictions have been set that are specific to individual users.

However, in a regulated industry setting, you will probably deviate from the default settings or roles. In these cases, you can:

- [Modify existing security roles](/dynamics365/customerengagement/on-premises/admin/create-edit-security-role#edit-a-security-role) directly.
- Modify existing security roles indirectly by [copying an existing security role](/dynamics365/customerengagement/on-premises/admin/create-edit-security-role#create-a-security-role-by-copy-role) and [editing the copy](/dynamics365/customerengagement/on-premises/admin/create-edit-security-role#edit-a-security-role).
- [Create a new security role](/dynamics365/customerengagement/on-premises/admin/create-edit-security-role).

The specific access settings that you use depend on your business requirements, but they might, for example, restrict access from the organization level to the business unit level. When you modify existing security roles, we recommend that you do so indirectly instead of directly. If you modify the existing security roles directly, you increase the risk that your customizations will be reset to default settings when an update to the Guides application is deployed. However, regardless of whether you modify security roles directly or indirectly, we recommend that you verify that your customizations are still in place after the Guides solution is updated.

Your organization can restrict and control access based on factors besides security roles, such as business units and owner teams.

Each user can be assigned to only one business unit. Therefore, if specific users have cross-organizational duties in relation to Guides, they can be included in owner teams that belong to other business units.

By using the default team in Dataverse for a business unit, you can link to an Active Directory group. In this way, you ensure that access is given only through a proper identity and access management (IAM) assignment in the organization.

## Next steps

- [Access control and identity and access management strategy](strategy-for-access-control-and-iam.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
