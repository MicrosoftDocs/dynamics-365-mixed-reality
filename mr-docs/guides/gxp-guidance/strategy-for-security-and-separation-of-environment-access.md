---
title: Security and separation of environment access strategy
description: Learn about restricted access, separate environments, and other security controls.
ms.date: 03/24/2023
ms.topic: article
author: prashantyvr
ms.author: prashan
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Security and separation of environment access strategy

[!INCLUDE [azure-ad-to-microsoft-entra-id](../../includes/azure-ad-to-microsoft-entra-id.md)]

Access to environments and content should be restricted and should generally follow the principle of least privilege (PoLP). In Microsoft Power Platform, this access can be handled at different levels.

As was mentioned in [Govern guides through Microsoft Power Platform environments and Power Apps](govern-guides-through-power-platform-environments-and-power-apps.md), you can use different Microsoft Power Platform environments and user roles that have limited access to drive compliance in the life cycle of a guide. To implement this approach, give users access only to required environments and assign only relevant security roles in those environments. To learn more about security roles, go to [Security roles and privileges](/power-platform/admin/security-roles-privileges).

When you're planning the setup, decide on the extent of automatically assigned access. Determine how the process should integrate with the company's existing practices for controlling the assignment of access rights and, for example, integration with the identity and access management (IAM) system.

We recommend that you create Microsoft Entra security groups for each environment and assign them to the appropriate environment. The advantage of this approach is that you can limit access to an environment based on membership in a specific security group. This membership-based access is set up in [Power Platform admin center](https://aka.ms/PPAC). For more information, go to [Restrict access to an environment in Dynamics 365 Guides by using security groups](../admin-security.md).

After assignment, only users who are members of the Microsoft Entra security groups can be created in the corresponding Microsoft Power Platform environments. For more information about how to assign Microsoft Entra security groups, go to [Control user access to environments](/power-platform/admin/control-user-access). Be sure to separate both test and production environments, and create separate security groups for all environments to specifically control access.

To effectively manage the assignment of security roles, we recommend that you create [owner teams](/power-apps/developer/data-platform/use-access-teams-owner-teams-collaborate-share-information) that match the personas/roles that are relevant for the system. For information about how to manage teams, go to [Microsoft Dataverse teams management](/power-platform/admin/manage-teams).

The use of owner teams has two major benefits:

- It assigns security roles by taking advantage of Microsoft Entra security groups and linking to existing IAM processes.
- It simplifies the assignment process. For example, to access the required functionality, an author needs both the author role and the basic user role. By assigning the security roles to an author team, you can give new authors the necessary roles just by adding them to the owner team.

:::image type="content" source="media/author-team.png" alt-text="Diagram that shows an example of an owner team and security roles.":::

If your organization is using the platform that has [business units](/power-platform/admin/create-edit-business-units), an owner team is automatically created for each business unit. If a business unit contains users for only one role (for example, authors), the owner team can be used to assign the correct security roles. However, in many cases, a single business unit contains users for multiple roles. Therefore, additional owner teams must be created and assigned relevant security roles. By default, each user is assigned to one business unit during the user creation process. However, access to other business units can be granted through assignment to a specific owner team.

For effective management, you need a scalable setup. We recommend that you automate permission management as much as possible. The process should preferably be linked to the IAM system. Here is an example of a high-level process for creating a new author (where the user has an existing user account):

1. A request is initiated to create an author through the IAM system.
1. The request is routed through an approval chain.
1. The user is assigned relevant Microsoft Entra groups:

    - A group that gives the user the correct licenses (for example, a Dynamics 365 Guides license)
    - Groups that give the user access to relevant Microsoft Power Platform environments
    - Groups that give the user membership in relevant Microsoft Power Platform teams that give the user the necessary security roles

1. The user is assigned to the correct business unit. Assignment is usually a manual process, but it can be automated through Power Apps or Power Automate to ensure consistent assignment and to link IAM.

For setups that have multiple business units, you must create Microsoft Entra security groups for every role in each business unit to add the user to the correct teams. Alternatively, you can assign teams directly in Microsoft Power Platform.

If steps are completed directly in Microsoft Power Platform, we recommend that you create a supporting process to facilitate and eliminate error. For example, implement a canvas app that helps the administrator assign membership to teams and assign the user to the correct business unit.

## Next steps

- [Test and deployment strategy](strategy-for-test-and-deployment.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
