---
title: Common challenges and requirements
description: Learn what you should consider about business and regulation requirements before you implement Dynamics 365 Guides.
ms.date: 03/21/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Common challenges and requirements

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

When you implement Dynamics 365 Guides in a regulated industry, it's important that you consider the business and regulatory requirements from the very beginning. Failure to do so is a common mistake. During the implementation process, stakeholders from the business, IT, and quality assurance (QA) must work together to align requirements from the three competence areas. Be sure to involve the competence areas throughout the process, and have them approve the process for governing and operating the framework that is established for Guides. Identify whether QA processes and audit trails can be supported by existing processes and systems or implemented as part of the Guides solution. Determine the traceability for the management and storage of the individual guides and versions.

To help ensure successful scaling of Guides after a pilot, you should consider questions such as the following:

- Which components are part of the Guides setup, and how do those components stay in sync functionally? (Components of the Guides setup include the PC version of Guides, the HoloLens Guides app, Power Apps, and Microsoft Power Platform environments.)
- How do you ensure that the validated state of the components is maintained and adheres to regulatory requirements?
- Which parts of the Guides setup require an audit trail? What metadata will support the audit trail?
- When major and minor revisions of a guide's content are needed, how will your organization version the guide?
- Is your data under regulatory control? If so, which regulations are you subject to? Examples in the life science industry include the United States Food and Drug Administration (FDA) and Europe, Middle East, and Africa (EMEA).
- How do you define approval, and what regulatory requirements, such as Good \{industry\} Practice (GxP), apply?
- How does your organization segregate data under regulatory controls and non-regulatory controls? An example is GxP versus non-GxP data.
- How do you make access to content easy to scale? Consider this question when you build your data model.
- What relevant naming standards should you introduce from the beginning? Examples include the names of guides, content, Microsoft Entra groups, business units, and folders.
- What roles/personas are involved in the guide life cycle?
- Who will manage security and the segregation of duty, and how?
- How will you uniquely link the approved guides to the specific positions where they must be run? For example, you can establish a link through a QR code, the guide ID, or the guide name.
- Who will maintain users and subscriptions, and how?
- Do you want to use a user-based setup or a multi-user-based (device-based) setup on the device for running guides? This setup is related to subscription management from operation, privacy, and cost perspectives.
- How do you consider the data privacy of named users? Should user statistics be enabled, and how will they affect potential audit log requirements?
- Do you have to know who has opened a specific guide? For a device-based setup, consider other documentation requirements for execution through Power Apps or on paper, based on regulatory requirements.
- How will you establish a software development life cycle to ensure continuous compliance of components such as Power Apps?
- How will you manage storage capacity over time in Microsoft Power Platform?
- How will you manage the reuse of assets that are used in multiple guides?
- Is Azure DevOps tooling in place? Have standard operating procedures (SOPs) been created for the Power Apps software development life cycle, and are they in place?
- Is a Microsoft Power Platform qualification required and in place?
- Has your organization's QA approved the establishment of risk-based agile delivery and continuous compliance?
- If your organization's QA considers this point relevant, has the qualification of infrastructure (Intune and Autopilot) and HoloLens devices (the operating system and the Guides application) been conducted?

More questions might apply, depending on your industry's specific requirements. Therefore, we recommend that you have a continuous dialogue with the business, IT, and QA to ensure that all requirements are addressed.

## Next steps

- [Prerequisites for implementation and planning rollout](prerequisites-for-implementation-and-planning-roll-out.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
