---
title: Segregate guides between organizational entities strategy
description: Learn about ways to segregate guides between users or organizational groups.
ms.date: 03/21/2023
ms.topic: article
author: prashantyvr
ms.author: prashan
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Segregate guides between organizational entities strategy

In regulated industries, organizations can have several factories, labs, departments, and divisions. When you implement Dynamics 365 Guides in such organizations, make strategic decisions about how you will ensure that only the relevant entities and individuals can view and edit guides. You can use [folders](../admin-create-folders.md) and [business units](/power-platform/admin/create-edit-business-units) to segregate guides between organizational entities.

We recommend that you consider whether the use of folders or business units in Microsoft Power Platform best suits your organization. There might be specific requirements from IT, and the approach that you choose might also depend on the identity and access management (IAM) process in your organization. The folder functionality in Guides enables you to manage groups of guides that have the same permissions. Business units provide a more restricted and tailored segregation of data. Investigate the business unit approach and the other Good \{industry\} Practice (GxP) security concepts to find the right fit when you need separate access for multiple organizational units in an environment.

First, create business units that match your business requirements, based on your organizational structure, for example. Next, put data and guides in the relevant business units, so that users can access data only in the business unit that they are assigned to. The advantages of this segregation from a user perspective are that it provides a simpler view to users, and it follows the principle of least privilege (PoLP). It's also advantageous for the approval flow process, because it helps ensure that relevant guides are visible to a specific group, such as quality assurance (QA).

On top of business units, you can manually [share a guide](../admin-share-guide.md) or manually [assign ownership](../admin-access-assign.md). Use these approaches only for simple implementations of Guides, where manual assignment is sufficient. If you're planning for an enterprise-scalable rollout of Guides, and access is controlled and centralized in the organization, consider a business unit approach. By default, when you create business units, matching [owner teams](/power-apps/developer/data-platform/use-access-teams-owner-teams-collaborate-share-information) are created. Consider these owner teams if you have users whose access must go across the organization. Although a user can be assigned to only one business unit at a time, you should not assign the upper-level business unit for that user. Instead, map access to the business unit that corresponds to the required access.

## Next steps

- [User control and access strategy](strategy-for-user-control-and-access.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
