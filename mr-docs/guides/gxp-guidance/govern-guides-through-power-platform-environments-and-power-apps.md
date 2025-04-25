---
title: Govern guides through Microsoft Power Platform environments and Power Apps
description: Learn about using Microsoft Power Platform or Power Apps to separate guides according to their life cycle stage.
ms.date: 03/20/2023
ms.topic: conceptual
author: prashantyvr
ms.author: prashan
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Govern guides through Microsoft Power Platform environments and Power Apps

Organizations must be in control of their data, and they must control who has access to what, and when. To govern guides, we recommend that regulated industry companies separate them according to their life cycle stage. For example, is a specific guide under development, or is it approved for everyday use? Depending on the life cycle stage of a guide, specific roles in your organization either should be allowed to access and edit the guide and its content, or should be restricted from accessing the guide at all.

To achieve this separation of guides according to their life cycle stage, you can create [Microsoft Power Platform environments](/power-platform/admin/environments-overview) that correspond to the relevant life cycle stages for your organization and industry. A typical life cycle consists of authoring, validation, execution, and archiving stages.

:::image type="content" source="media/gxp-lifecycle.png" alt-text="Diagram of a typical guide life cycle.":::

Practically speaking, a given guide exists in only one environment at a time. However, [multiple versions of a guide can exist in different environments simultaneously](strategy-for-versioning-guides.md). By separating guides according to their life cycle stage, you help reduce the risk of production errors that can occur if a machine operator follows the instructions in an unfinished, unvalidated, or obsolete guide. At the same time, we recommend that organizations enforce role-based access control through [business units](/power-platform/admin/create-edit-business-units) and [security roles](/power-platform/admin/security-roles-privileges), so that employees have access only to environments where they have duties to fulfill. In this way, you ensure a strict split between data and user access.

To facilitate a smooth flow of guides between environments, we recommend that you use [Power Apps](/power-apps/powerapps-overview) to enable the relevant employees to transfer guides from one environment to another. In this way, your organization can establish an audit trail, where the required metadata is added to support the regulatory requirements of your industry, company quality controls, and traceability.

The following diagram shows the recommended flow structure between four typical environments. Arrows indicate the directions that guides can be transferred in. For example, a guide can be transferred from authoring to validation, and then back again if it's judged to be incorrect or not precise enough to be approved. However, a guide can't bypass the validation environment. It must go through validation before it's transferred to execution, where it's used by operators on a production line, for example.

:::image type="content" source="media/flow-structure.png" alt-text="Diagram of the recommended flow structure between four environments.":::

To make the concept of environments that match life cycle stages more concrete, the rest of this article provides a more thorough description of each of the four previously mentioned example environments: [authoring](#example-environment-1-authoring-environment), [validation](#example-environment-2-validation-environment), [execution](#example-environment-3-execution-environment), and [archiving](#example-environment-4-archive-environment). Although this environment structure and the flow between environments in it are typically relevant to regulated industry companies, they might not be relevant to your specific company or compliant with the specific regulations that you're subject to. To identify the relevant structure and flow for your company, we recommend that you facilitate internal stakeholder workshops. For more information, go to [The Guides user journey](prerequisites-for-implementation-and-planning-roll-out.md#the-guides-user-journey).

## Example environment 1: Authoring environment

During the first stage of a guide's life cycle, your organization creates the guide on a PC, together with the tasks and steps that users of the guide will follow. You then place holographic 3D content in the physical space to help users understand the step-by-step instructions. This process is also known as [authoring](../authoring-overview.md). While guides are being authored, we recommend that they exist in an environment that is dedicated to authoring.

Because the guides are still being created at this stage, and they are unvalidated and perhaps even incomplete, it's crucial that users in a lab, for example, should not be able to use them. By authoring guides in a dedicated authoring environment, the authors can create, develop, test, and evaluate the holographic content and wording without any risk that the guides will be used before they are finalized, approved, and released for everyday use.

In your organization, an author might be a training consultant, a project engineer, or an operator who has specialized knowledge of a specific piece of production equipment. While guides are in this first stage of their life cycle, it's the author's responsibility to:

- Add the regulatory-required metadata in preparation for the approval process.
- Ensure that content and placement in three-dimensional space work as intended before the guide is transferred to the next environment, the validation environment.

## Example environment 2: Validation environment

The validation environment is used to validate, reject, and approve guides that authors created in the authoring environment.

Most likely, validation is a duty of your quality assurance (QA) specialists. The QA specialists evaluate, among other things, the guide's content (such as adherence to standard operating procedures \[SOPs\]), the placement of 3D objects in the physical space, and the overall quality.

As a result of these evaluations, the QA specialists decide whether a guide is ready to be used at a production site, for example, and can therefore be transferred to the execution environment, or whether it needs additional authoring before it can be approved for use. In the latter case, the guide is transferred back to the authoring environment so that the author can improve the augmented instructions by using Power Apps.

If holographic elements such as 3D arrows are included in the content that instructs the user, the validation must be done at least partially on a HoloLens device. In this way, QA specialists can access, for example, the 3D arrows that nudge the user's attention toward a specific point of interest on the machine, and they can verify that these arrows are precisely placed and not potentially misleading.

Although technical reviewers or subject matter experts might have to support the QA process or be responsible for the technical/subject matter expert review, QA has final approval.

> [!NOTE]
> Compared to the authoring environment, the validation environment might require more regulatory controls and limitations on changes, access, and traceability.

## Example environment 3: Execution environment

After guides are authored, validated, and approved, they reside in the execution environment, where they become read-only. Guides in this environment are ready to be used at a site (for example, on a production line in a manufacturing company).

At the site, a unique reference to the approved guides is set: printed QR codes are placed on machinery, or next to equipment on tablets or other surfaces. Operators wear a HoloLens device and scan the QR codes through the HoloLens camera. Each QR code has an embedded link. Therefore, when it's scanned, a specific guide is opened from the execution environment. The operator then follows the guide's instructions for the relevant activity or process.

Alternatively, your organization can use tablets or mobile phones instead of HoloLens devices to open, view, and follow the instructional guides. Nevertheless, HoloLens devices offer some advantages over tablets and mobile phones:

- HoloLens overlays holographic images on the real world. Therefore, users interact with digital content in a more immersive way than tablets and mobile phones can provide.
- You can use QR codes with a HoloLens device but not with a tablet or mobile phone.
- Unlike tablets and mobile phones, HoloLens is a hands-free device that enables users to interact with digital content through voice commands, gestures, and eye tracking. Therefore, users can easily follow the guide while they perform tasks with their hands.

When there is a separate environment for execution, users can have full confidence in the correctness and quality of the instructions that are provided. Because authoring options are locked in this environment, operators, QA, and managers know that intentional or accidental edits to guides aren't possible. The execution environment is only for operators' day-to-day use of guides.

> [!NOTE]
> Compared to the authoring environment, the execution environment might require more regulatory controls and limitations on changes, access, and traceability.

## Example environment 4: Archive environment

Eventually, the guides that your organization has authored, approved, and used become obsolete and must be retired. For example, guides might become obsolete when your organization replaces machinery to optimize production flows. If the new machinery is handled differently, new instructions for operating the production equipment are needed.

A guide might also become obsolete because an operator realizes that the instructions in it could be more efficient or accurate. In this case, the guide must be updated by creating a new, corrected version. Because it's recommended that you track the evolution of your guides, the process of updating an inefficient or inaccurate guide involves duplicating the guide if it has been accessible in the execution environment, and then making the guide in the execution environment obsolete. For more information, go to [Versioning guides strategy](strategy-for-versioning-guides.md).

You should keep obsolete guides for audit trail purposes, because audit trails might be a regulatory or business quality requirement. We recommend that you retire guides in an environment that is dedicated to archiving. The retention period for guides in the archive environment should be set according to industry requirements and other standards in your organization.

> [!NOTE]
> Compared to the authoring environment, the archive environment might require more regulatory controls and limitations on changes, access, and traceability.

## Next steps

- [Common challenges and requirements](common-challenges-and-requirements.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
