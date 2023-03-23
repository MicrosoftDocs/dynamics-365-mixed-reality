---
title: Segregate guides between organizational entities strategy
description: Learn about ways to segregate guides between users or organizational groups.
ms.date: 03/21/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Segregate guides between organizational entities strategy

In regulated industries, organizations can have several factories, labs, departments, and divisions. When implementing Dynamics 365 Guides into such organizations, make strategic decisions on how to ensure that guides are only visible and editable to the relevant entities and individuals. You can segregate guides between organizational entities with the help of [folders](../admin-create-folders.md) and [business units](/power-platform/admin/create-edit-business-units).

We recommend you consider whether the use of folders or business units in Power Platform suits your organization the best. There might be specific requirements from IT, and the chosen approach might also depend upon the Identity and Access Management (IAM) process within your organization. The folder functionality in Guides enables you to manage groups of guides with the same permissions. Business units provide a more restricted and tailored segregation of data. Investigate the business unit approach and the other GxP security concepts to find the right fit when you need separate access for multiple organizational units in an environment.

First, create business units matching your business requirements, for instance, based on your organizational structure. Second, place data and guides in the relevant business units, so that users can only access data in the business unit they're assigned to. This segregation gives you an advantage from auser perspective as it provides a simpler view for the user and follows the least privilege principle. This segregation is also advantageous for the approval flow process to help you ensure that relevant guides are visible for a specific group, such as quality assurance (QA).

On top of business units, you can manually [share a guide](../admin-share-guide.md) or manually [assign ownership](../admin-access-assign.md). Use sharing and assigning ownership only for simple implementations of Guides where manual assignment is sufficient. If you plan for an enterprise scalable rollout of Guides and access is controlled and centralized in the organization, consider a business unit approach. By default, creating business units creates matching [owner teams](/power-apps/developer/data-platform/use-access-teams-owner-teams-collaborate-share-information). Consider these owner teams if you have users whose access must go across the organization. While a user can only be assigned to one business unit at a time, you wouldn't assign the upper-level business unit for that user, but instead map access to the business unit that corresponds to the needed access.

## Next steps

- [Strategy for user control and access](strategy-for-user-control-and-access.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
