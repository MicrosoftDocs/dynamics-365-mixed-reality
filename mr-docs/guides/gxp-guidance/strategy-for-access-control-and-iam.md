---
title: Strategy for access control and IAM
description: Learn about access control of Guides and Identity and Access Management in a regulated industry
ms.date: 03/09/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Strategy for access control and IAM

When working in a regulated industry, maintaining full control of access is key. To do so, we recommend using the principle of least privilege (PoLP). PoLP is an information security concept stating that a user should only be granted access to the specific data, resources, and/or applications that are needed to complete the required task.

To properly configure your Identity and Access Management (IAM) and maintain full access control of Guides content, we recommend you define roles, functionalities, and environments. If your organization has facilitated stakeholder workshops as suggested in prerequisites for implementation and planning roll-out, you have most of the information needed to define these roles.

**Define roles**

To properly set up your IAM, consider which roles are involved in the process flow that guides undergo from their creation to archiving. In a process flow that adheres to regulated industry requirements, two roles are mandatory: an author and a QA. The guide needs to be authored and it needs to be validated.

Consider if a process owner would be involved in the initial steps of the Guides user journey. For example, a process owner could request the creation of a guide based on a need identified in production. If you wish to integrate the Guides process flow with existing processes such as a Quality Management System (QMS) or a Learning Management System (LMS), you might need a role that handles the integration process and ensures that systems are in sync.  
  
QA might need support to do validation from a technical reviewer that validates the guide in-depth with their HoloLens. There is an operator role who launches and follows the instructions in the guide. The roles within your Guides flow fully depend upon your organization, your processes, and your needs. Identifying these roles in the preliminary implementation phases is key.

:::image type="content" source="media/defined-roles.png" alt-text="Example of a set of defined roles within a Guides process flow":::

**Define functionalities**

When the necessary roles have been defined, define which technical features each of these roles require.  
  
The author role creates and develops guides and need access to the Guides PC app, the Guides Mobile app, Guides via HoloLens, and, potentially, a Power App enabling the author to transfer the guide further in the process flow (to review by QA). This is necessary to create, configure, and test the guide. However, they might not need any further involvement.  
  
The QA role has nothing to do with the actual creation of the guide, but it is critical that they can view the guide, the related content, and the metadata to approve or reject the guide. These are other functionalities than those of the author. There might be other reviewers involved in the process as well, but they shouldn't have the right to edit the guide.

To limit the number of users that can edit the guide, assign a role within the flow who is responsible for delivering feedback across roles throughout the entire Guides flow. This is especially useful if you use both the Power Platform and a QMS without automated integrations. In that case, this role would also be the binding link between the two platforms, ensuring that any comments made in the QMS in relation to rejection of a particular guide, are delivered to the author so they can adjust the guide accordingly. Introducing this linking role means that the author's access can be restricted to Power Platform only, and the QA's access can be restricted to the QMS only. This way you ensure that each role has limited access that keeps them within their defined role, their defined functionality, and their field of expertise. It is possible to support this process further if system integrations are made point-to-point or via a middle-layer integration platform.

:::image type="content" source="media/defined-functionalities.png" alt-text="Example of a set of defined functionalities within a Guides flow":::

**Create the access control structure**

When roles and functionalities have been defined, determine which environment they belong to. Assigning specific roles to specific environments ensures that content remains compliant and controlled by the right roles. The following example demonstrates the combined roles, functions, and environments.

:::image type="content" source="media/combo-roles-functions-env.png" alt-text="Example of combined roles, functions, and environments":::

The environments each represent different stages of the content's life cycle. While adhering to the PoLP and keeping the defined roles and needed functionalities in mind, it is possible to place each role within each environment. As illustrated, the author has access to the authoring environment and no other environments. This decision is based upon the definition of the role and the related functionalities which are to create, configure and test guides. Hence, this role does not need access to any other parts of the content's lifecycle.

The configured roles, functionalities, and environments can all be linked to your organization's existing IAM system by defining an [AD security group](/windows-server/identity/ad-ds/manage/understand-security-groups) with specific access and security elements related to each role. The benefit of this setup is that when users are granted a specific role, they are automatically provided with the necessary access to perform the assignments of the role they have. Furthermore, this IAM setup ensures that changes and terminations of access happen in a controlled and automated process in sync with the onboarding and offboarding of employees within the organization.

:::image type="content" source="media/all-managed-elements.png" alt-text="A full overview of elements that can be managed by AD groups and linked to the IAM process and other systems of relevance":::

## Next steps

- [Strategy for content and 3D toolkit ownership](strategy-for-content-and-3d-toolkit-ownership.md)
