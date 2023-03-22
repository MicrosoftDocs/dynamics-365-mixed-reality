---
title: Govern guides through Power Platform environments and Power Apps
description: Learn about the separation of guides according to the life cycle stages using Power Platform or Power Apps
ms.date: 03/20/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Govern guides through Power Platform environments and Power Apps

Organizations must be in control of their data and who has access to what and when. To govern guides, we recommend regulated industry companies separate guides according to their life cycle stage. For example, is a specific guide under development or approved for daily usage? Depending on the life cycle stage of a guide, certain roles in your organization should be allowed to access and edit the guide and its content or restricted from accessing the guide altogether.

The separation of guides according to life cycle stages can be achieved by creating Power Platform [environments](/power-platform/admin/environments-overview) corresponding to the relevant life cycle stages for your organization and industry. A typical life cycle is authoring, validation, execution, and archive.

:::image type="content" source="media/gxp-lifecycle.png" alt-text="A typical guides life cycle":::

Practically, a specific guide only lives in one environment at a time. However, [multiple versions of a guide can exist in different environments simultaneously](strategy-for-versioning-guides.md). By separating guides according to their life cycle stage, you reduce potential production errors resulting from a machine operator following instructions in an unfinished, non-validated or obsolete guide. At the same time, we recommend your organization enforces role-based access control through [business units](/power-platform/admin/create-edit-business-units) and [security roles](/power-platform/admin/security-roles-privileges) so that employees only have access to environments in which they have duties to fulfill. In this way, you ensure a strict split between data and user access.

To facilitate a smooth flow of guides between environments, we recommend [Power App](/power-apps/powerapps-overview) to enable the relevant employees to transfer guides from one environment to another. Hereby, your organization can establish an audit trail with the required metadata being added to support the regulatory requirements of your industry, company quality controls, and traceability.

The recommended flow structure between typical environments is illustrated below (arrows indicate the directions in which guides can be transferred). For instance, a guide can be transferred from authoring to validation and back again if it is deemed incorrect or not precise enough to be approved. However, a guide can't bypass the validation environment and must go through validation before being transferred to execution where it's used by operators at a production line for example.

:::image type="content" source="media/flow-structure.png" alt-text="The recommended flow structure between 4 environments":::

To make the concept of environments matching a life cycle stage more tangible, you'll find more thorough descriptions of the example environments: [authoring](#example-environment-1-authoring-environment), [validation](#example-environment-2-validation-environment), [execution](#example-environment-3-execution-environment), and [archiving](#example-environment-4-archive-environment). However, while the environment structure and flow between them is typically relevant for regulated industry companies, it might not be a relevant setup for your company or compliant with the specific regulations you are subject to. To identify the relevant structure and flow for your company, we recommend facilitating internal stakeholder workshops. For more information, see The Guides user journey in [prerequisites for implementation and planning roll-out](prerequisites-for-implementation-and-planning-roll-out.md).

## Example environment 1: Authoring environment

During the first stage of a guide's life cycle, your organization creates the guide on the PC with its tasks and steps to be followed by end-users of the guide. Then, you place holographic 3D content in the physical space to help the users' understanding of the step-by-step instructions. This process is also known as [authoring](../authoring-overview.md). When guides are being authored, we recommend they exist in an environment dedicated to authoring.

Since the guides in this environment are under creation, non-validated, and maybe even incomplete, it is paramount that end-users in a lab, for instance, cannot start using them. This is exactly the reason behind creating an authoring environment; that authors of a guide can create, develop, test, and evaluate the holographic content and wording without risking the guide being used before it is finalized, approved, and released for day-to-day usage.  
  
In your organization, an author could be a training consultant, a project engineer, or an operator with specialized knowledge of a particular piece of production equipment.

When guides are in this stage of their life cycle, it is the author's responsibility to:

- Add the regulatory required metadata in preparation for the approval process.

- Make sure content and placement in a 3-dimensional space works as intended before transferring the guide to the next environment: the validation environment.

## Example environment 2: Validation environment

The validation environment is used for validating, rejecting, and approving guides created by authors in the authoring environment.  
  
Most likely, validating guides is a duty for your quality assurance (QA) specialists. The QA specialist validates, among other things, the guide's content (such as standard operating procedure (SOP) adherence), the placement of 3D objects in the physical space, and the overall quality.

As a result of these evaluations, QA decides whether the guide is ready to use at, for example, a production site and therefore transferred to the execution environment, or if the guide needs additional authoring before being approved for use. In the latter case, the guide is transferred back to the authoring environment to improve the augmented instructions by using Power App.

If holographic elements, like 3D arrows, are included in the content instructing the user, the review needs to be done – at least partially – through a HoloLens device. That way, QA can access, for example, the 3D arrows nudging the user's attention towards a specific point of interest on the machine and can verify if these are precisely placed and not potentially misleading.

Potentially, technical reviewers or subject matter experts must support the QA process or be responsible for the technical/subject matter expert review, but QA has final approval.

> [!NOTE]
> Compared to the authoring environment, the validation environment might require additional regulatory controls and limitations to changes, access, and traceability.

## Example environment 3: Execution environment

The execution environment is the space where authored, validated, and approved guides live in read-only mode. When in this environment, guides are ready to use at a production line in a manufacturing company, for example.

At the site, a unique reference to the approved guides is set: printed QR codes are placed on machinery or displayed next to equipment on tablets or other surfaces. Operators wear a HoloLens and scan the QR codes through the HoloLens camera. Each QR code has an embedded link, meaning a specific guide from the execution environment is launched upon scanning. From here on, the operator follows the guide's intuitive and efficient instructions on how to handle the relevant activity or process.

With a separate environment for execution, end users can have full confidence in the correctness and quality of the provided instructions. Operators, QA, and managers know that intentional or accidental edits to guides aren't possible because authoring options are locked in this environment. The execution environment is solely for operators' day-to-day use of guides.

> [!NOTE]
> Compared to the authoring environment, the execution environment might require additional regulatory controls and limitations to changes, access, and traceability.

Alternatively, instead of HoloLens devices, your organization can use tablets or mobile phones to launch, view, and follow the instructional guides. However, for regulated industry usage, HoloLens is the recommended choice: HoloLens overlays holographic images on the real world, allowing users to interact with digital content in a more immersive way than mobile phones or tablets can provide. Furthermore, unlike mobile phones or tablets, the HoloLens is a hands-free device that allows users to interact with digital content using voice commands, gestures, and eye tracking. This makes it easier for users to follow the guide while performing tasks with their hands.

## Example environment 4: Archive environment

Eventually, the guides your organization has authored, approved, and utilized become obsolete. This happens, for instance, when your organization replaces machinery to optimize production flows. The new machinery is handled differently, which results in the need for new instructions on how to operate the production equipment.  
  
Guides can also become obsolete because an operator realizes that instructions in a guide could be more efficient or accurate. In these cases, the related guide needs to be updated by creating a new, corrected version. Because it is recommended to keep track of the evolution of guides, updating a faulty or less efficient guide involves a duplication of the guide if it has been accessible in the execution environment and make the guide in the execution environment obsolete. For more information, see [guides versioning](strategy-for-versioning-guides.md).

You should keep obsolete guides for audit trail purposes as this can be a regulatory or business quality requirement. We recommend retiring guides in an environment dedicated to archiving. The retention period for guides in the archive environment should be set according to industry requirements and other standards in your organization.

> [!NOTE]
> Compared to the authoring environment, the archive environment might require additional regulatory controls and limitations to changes, access, and traceability.

## Next steps

- [Common challenges and requirements](common-challenges-and-requirements.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
