---
title: Access control and identity and access management strategy
description: Learn about access control of Dynamics 365 Guides and identity and access management (IAM) in a regulated industry.
ms.date: 03/24/2023
ms.topic: article
author: prashantyvr
ms.author: prashan
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Access control and identity and access management strategy

In a regulated industry, maintaining full control of access is key. We recommend that you use the principle of least privilege (PoLP). PoLP is an information security concept that states that users should be granted access only to the specific data, resources, or applications that they need to complete the required task.

To configure identity and access management (IAM) and maintain full access control of Dynamics 365 Guides content, we recommend that you define roles, functionalities, and environments. If your organization has facilitated stakeholder workshops as suggested in [Prerequisites for implementation and rollout](prerequisites-for-implementation-and-planning-roll-out.md), you already have most of the information that you need to define these roles.

## Define roles

To set up IAM, consider which roles are involved in the process flow that guides undergo from creation through archiving. In a process flow that adheres to regulated industry requirements, two roles are mandatory: author and quality assurance (QA). Every guide must be authored, and it must be validated.

Consider whether a process owner will be involved in the initial steps of the Guides user journey. For example, a process owner can request the creation of a guide based on a need that is identified in production. If you want to integrate the Guides process flow with existing processes, such as a quality management system (QMS) or a learning management system (LMS), consider a role that handles the integration process and ensures that systems are in sync.

QA might need support from a technical reviewer who uses a HoloLens device to do in-depth validation of the guide. There is an operator role that opens the guide and follows the instructions in it.

The roles in your Guides flow fully depend on your organization, your processes, and your needs. Identification of these roles in the preliminary implementation phases is key.

:::image type="content" source="media/defined-roles.png" alt-text="Diagram that shows an example of a set of defined roles in a Guides process flow.":::

## Define functionalities

When the necessary roles have been defined, determine which technical features each role requires.

The author role creates and develops guides and needs access to the Guides PC app, the Guides Mobile app, and Guides through HoloLens. To transfer a guide further in the process flow (to review by QA), the author role might also need access to an app that is created in Power Apps. Authors must have this access so that they can create, configure, and test guides. However, after they have completed those tasks, they might not need to be involved any further.

The QA role has nothing to do with creating guides, but it must be able to view a guide, the related content, and the metadata to approve or reject the guide. These functionalities differ from those of the author role. Although other reviewers might also be involved in the process, they should not have the right to edit the guide.

To limit the number of users who can edit a guide, assign a role that is responsible for delivering feedback across roles throughout the entire Guides flow. This role is especially useful if you use both Microsoft Power Platform and a QMS without automated integrations. In this case, the role is the binding link between the two platforms. It ensures that any comments that are made in the QMS about the rejection of a particular guide are delivered to the author. The author then adjusts the guide accordingly. If this linking role is introduced, the author role's access can be restricted to Microsoft Power Platform only, and the QA role's access can be restricted to the QMS only. In this way, you ensure that the users in each role have limited access that keeps them in their defined role, their defined functionality, and their field of expertise. This process can be supported further if system integrations are made point-to-point or through a middle-layer integration platform.

:::image type="content" source="media/defined-functionalities.png" alt-text="Diagram that shows an example of a set of defined functionalities in a Guides process flow.":::

## Create the access control structure

When roles and functionalities have been defined, determine which environment they belong to. By assigning specific roles to specific environments, you ensure that content remains compliant and controlled by the right roles. The following diagram shows an example of the combined roles, functionalities, and environments.

:::image type="content" source="media/combo-roles-functions-env.png" alt-text="Diagram that shows an example of combined roles, functionalities, and environments.":::

Each environment represents a different stage of the content's life cycle. As you place each role in its appropriate environment, adhere to the PoLP, and keep the defined roles and required functionalities in mind. As the preceding diagram shows, the author role has been granted access to the authoring environment but no other environments. This decision is based on the definition of the role and the related functionalities, which are to create, configure, and test guides. Therefore, this role doesn't need access to any other parts of the content's life cycle.

The configured roles, functionalities, and environments can all be linked to your organization's existing IAM system by defining an [Active Directory security group](/windows-server/identity/ad-ds/manage/understand-security-groups) where specific access and security elements are related to each role. The benefit of this setup is that when users are granted a specific role, they automatically get the access that they need to perform the assignments of that role. Furthermore, this IAM setup ensures that changes and terminations of access occur through a controlled and automated process and are in sync with the onboarding and offboarding of employees in the organization.

:::image type="content" source="media/all-managed-elements.png" alt-text="Diagram that shows a full overview of elements that can be managed by Active Directory groups and linked to the IAM process and other relevant systems.":::

## Next steps

- [Content and toolkit ownership strategy](strategy-for-content-and-3d-toolkit-ownership.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
