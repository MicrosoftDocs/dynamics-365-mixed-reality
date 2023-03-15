---
title: Common challenges and requirements
description: Consider questions regarding business and regulation requirements before implementing Dynamics 365 Guides
ms.date: 03/13/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Common challenges and requirements

When implementing Guides in regulated industries, it is a common mistake not to consider the business and regulation requirements from the beginning. In the implementation process, stakeholders from the business, IT, and Quality Assurance (QA) must work together to get requirements from the three competence areas aligned. Involve the competence areas throughout the work and have them approve how to govern and operate the framework established around Guides.

Identify if QA processes and audit trails will be supported by existing processes and systems or implemented as part of the Guides solution. This includes how traceability of the individual guides and versions are to be managed and stored.

For a successful scaling of Guides after a pilot, it is advised to address questions such as:

- Which components are part of the Guides set up and how do the components (such as the PC version of Guides, HoloLens Guides app, Power Apps, Power Platform environments) stay in sync functionally?

- How do you ensure the validated state of the components is maintained and adheres to regulatory requirements?

- Which parts of the Guides set up require an audit trail? What metadata will support this?

- When major and minor revisions to the content of a guide is needed, how will your organization version the guide?

- Is your data under regulatory control? If so, which regulations? For example, this could be FDA, or EMEA within the life science industry.

- How do you define approval, and what regulatory requirements (for example, GxP) apply?

- How does your organization segregate data under regulatory controls and non-regulatory controls? For example, GxP versus non-GxP data.

- How do you make access to content easy to scale? Consider this when building your data model.

- What naming standards will be relevant to introduce from the beginning? For example, name of guides, content, Active Directory (AD) groups, business units, and folders.

- What roles/personas are involved in the guides lifecycle?

- Who will manage the security and segregation of duty? And how?

- How will you uniquely link the approved guides to the specific positions where they are to be executed? For example, via QR code, guide ID, or guide name.

- How and who will maintain users and subscriptions?

- Do you want to make use of a user-based or multi-user based (device-based) setup on the device for executing guides? This relates to subscription management from an operation, privacy, and cost perspective.

- How do we consider data privacy of named users? Should user statistics be enabled and how will it impact potential audit log requirements?

- Is it required to know who has launched a specific guide? If a device-based setup is chosen, this might require considerations of additional documentation of execution via Power Apps or paper depending on regulatory requirements.

- How will you establish a software development life cycle (SDLC) to ensure continuous compliance of components like Power Apps?

- How will you manage storage capacity over time in Power Platform?

- How will you manage the reuse of assets used in multiple guides?

- Is DevOps tooling in place and SDLC SOP created for Power Apps?

- Is a Power Platform qualification required and in place?

- Has your organization's QA approved the establishment of a risk-based agile delivery and continuous compliance?

- If considered relevant by your organizations' QA, has the qualification of infrastructure (Intune & Autopilot) and HoloLens devices (OS & Guides application) been conducted?

Additional questions might apply due to your industry's specific requirements. Therefore, it is advised to have a continuous dialogue with business, IT, and QA to ensure all requirements are addressed.

## Next steps

- [Prerequisites for implementation and planning roll-out](prerequisites-for-implementation-and-planning-roll-out.md)
