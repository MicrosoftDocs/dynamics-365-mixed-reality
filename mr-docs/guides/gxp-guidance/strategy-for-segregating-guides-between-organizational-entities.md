---
title: Strategy for segregating guides between organizational entities
description: Learn about ways to segregate guides between users or organizational groups
ms.date: 03/09/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
---

# Strategy for segregating guides between organizational entities

In regulated industries, organizations are usually comprised of several factories, labs, departments, and divisions. When implementing Guides into such organizations, make strategic decisions on how to ensure that guides are only visible and editable to the relevant entities and individuals. This can be achieved by segregating guides between organizational entities with the help of [folders](/guides/admin-create-folders) and [business units](/power-platform/admin/create-edit-business-units).

We recommend considering whether the use of folders or the use of business units in Power Platform suits your organization the best. There might be specific requirements from IT, and the chosen approach might also depend upon the Identity and Access Management (IAM) process within your organization. The folder functionality in Guides enables you to manage groups of guides with the same permissions, while business units provides a more restricted and tailored segregation of data. The business unit approach and the other security concepts in the GxP documentation should be investigated and evaluated first to find the right fit when looking into separate access for multiple organizational units within an environment.

First, create business units matching your business requirements, for instance, based on your organizational structure. Second, place data and guides in the relevant business units, so that users can only access data in the business unit they are assigned to. This segregation gives you an advantage from an end-user perspective by providing a simpler view for the user and follows the principle of least privilege. This segregation is also advantageous when adding the aspect of the process around the approval flow to help you ensure that relevant guides are visible for a specific group, for example, QA.

On top of business units, you can manually [share a guide](/guides/admin-share-guide) or manually [assign ownership](/guides/admin-access-assign). However, keep it only for simple implementations of Guides where manual assignment is sufficient. If you plan for an enterprise scalable rollout of Guides and access is controlled and centralized in the organization, consider a business unit approach. Creating business units, by default, creates matching [owner teams](/power-apps/developer/data-platform/use-access-teams-owner-teams-collaborate-share-information) which can be considered if you have users where their access needs go across the organization. While a user can only be assigned to one business unit at a time, you would not assign the upper-level business unit for that user, but instead map access to the business unit that corresponds to the needed access.
