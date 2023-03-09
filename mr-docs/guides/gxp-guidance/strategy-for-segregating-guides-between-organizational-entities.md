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

# Strategy for segregating guides between organizational entities

In regulated industries, organizations are usually comprised of several factories, labs, departments, divisions etc. When implementing Guides into such organizations, you will need to make strategic decisions on how to ensure that guides are only visible and editable to the relevant entities and individuals. This can be achieved by segregating guides between organizational entities with the help of [Folders](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/admin-create-folders) and [Business Units](https://learn.microsoft.com/en-us/power-platform/admin/create-edit-business-units).

The recommendation is to consider whether the use of Folders or the use of Business Units in the Power Platform suits your organization the best. There might be specific requirements from IT, and the chosen approach might also depend upon the Identity and Access Management (IAM) process within your organization. The Folder functionality in Guides allows you to manage groups of guides with the same permissions, while Business Units provides a more restricted and tailored segregation of data. The Business Unit approach and the other security concepts that have been referenced in this documentation should be investigated and evaluated first to find the right fit when looking into separate access for multiple organizational units within an environment.

Firstly, you create Business Units matching your business requirements, for instance, based on your organizational structure. Secondly, you place data and guides in the relevant Business Units, meaning users can only access data in the Business Unit they are assigned to. This segregation gives you an advantage from an end-user perspective (provides a simpler view for the user and follows the principle of least privilege), but also when adding the aspect of the process around the approval flow that will help you ensure that relevant guides are visible from the exact group of, for example, the expected QA.

On top of Business Units, you can manually [share a guide](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/admin-share-guide) or manually [assign ownership](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/admin-access-assign). However, keep it only for simple implementations of Guides where manual assignment is sufficient. If you plan for an enterprise scalable rollout of Guides, and access is controlled and centralized in the organization, consider a Business Unit approach. Creating Business Units will also by default<u>,</u> create matching [Owner Team](https://learn.microsoft.com/en-us/power-apps/developer/data-platform/use-access-teams-owner-teams-collaborate-share-information) which can be considered if you have users where their access needs go across the organization. While a user can only be assigned to one business unit at a time, you would not assign the upper-level Business Unit for that user, but instead map access to the business unit that corresponds to the needed access.


