---
title: Security and separation of environment access strategy
description: Learn about restricted access, separate environments, and other security controls.
ms.date: 03/24/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Security and separation of environment access strategy

Access to environments and content should be restricted and generally follow a least privilege principle. In Power Platform, this can be handled on different levels.

As mentioned in [govern guides through Power Platform environments and Power Apps](govern-guides-through-power-platform-environments-and-power-apps.md), you can use different Power Platform environments and user roles with limited access to drive compliance in the life cycle of a guide. To implement, only give the user access to required environments and  assign only relevant security roles in these environments. To learn more about security roles, see [Security roles and privileges](/power-platform/admin/security-roles-privileges).

While planning the setup, decide the extent of automatically assigned access. Determine how the process should integrate with the company's existing practices for controlling assignment of access rights and, for example, integration to the Identity Access Management (IAM) system.

We recommend creating Azure Active Directory (AD) Security Groups for each environment and assigning to the respective environment. The advantage to this is that you can limit access to an environment based on the membership of the specific Security Group. This is done through the [Power Platform admin center](https://aka.ms/PPAC). For more information, see [restricting access to an environment in Dynamics 365 Guides](../admin-security.md).

After assignment, only users that are members of the Azure AD Security Groups can be created in the respective Power Platform environments. For more information about assigning Azure AD Security Groups, see [Control user access to environments](/power-platform/admin/control-user-access). Be sure to separate both test and production environments and create separate security groups for all environments to specifically control access.

To effectively manage the assignment of security roles, we recommend creating [owner teams](/power-apps/developer/data-platform/use-access-teams-owner-teams-collaborate-share-information) that match the personas/roles relevant for the system. For information about managing teams see [Microsoft Dataverse teams management](/power-platform/admin/manage-teams).

The usage of owner teams has two major benefits:

1. Assigns security roles by leveraging Azure AD Security Groups and linking to existing IAM processes.

1. Simplifies the assignment process. An author, for example, needs both the author role and the basic user role to access the required functionality. By assigning the security roles to an author team, it is possible to give new authors the necessary roles just by adding them to the owner team.

:::image type="content" source="media/author-team.png" alt-text="Example of an owner team and security roles.":::

If your organization is utilizing the platform with [business units](/power-platform/admin/create-edit-business-units), an owner team is automatically created per business unit. The owner team can be used to assign the proper security roles if this specific business unit only contains users for one role, for instance authors. However, in many cases, multiple roles are divided into one business unit which requires additional owner teams to be created and assigned relevant security roles. By default, each user is assigned to one business unit during the user creation process, but additional access to other business units can occur by assigning to a specific owner team.

For effective management you need a scalable setup. We recommend automating permission management as much as possible. The process should preferably be linked to the IAM system. An example of a high-level process for creating a new author (where the user has an existing user account):

1. A request is initiated to create an author through the IAM system.

1. The request is routed through an approval chain.

1. The user is assigned relevant Azure AD groups:

    - Group that gives the user correct licenses, for example, Dynamics 365 Guides license.
    - Groups that give the user access to relevant Power Platform environments.
    - Groups that give the user membership of relevant Power Platform teams, which give the user the necessary security roles.

1. The user is assigned to the correct business unit, which is normally a manual process but can be automated with Power App or Power Automate to ensure consistent assignment and link IAM.

For setups with multiple business units, the process requires that Azure AD security groups are created in each business unit for every role to add the user to the correct teams. Alternatively, you can assign teams directly in Power Platform.

In case steps are handled directly in Power Platform, we recommend creating a supporting process to facilitate and eliminate error. For example, implement a Canvas App that can help the administrator assign membership to teams and to assign the user to the correct business unit.

## Next steps

- [Strategy for test and deployment](strategy-for-test-and-deployment.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
