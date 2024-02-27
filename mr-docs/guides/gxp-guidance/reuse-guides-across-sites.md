---
title: Reuse guides across sites
description: Learn about using guides across multiple sites in a regulated industry, and how to avoid issues.
ms.date: 03/21/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Reuse guides across sites

If you have similar production lines or machinery across factories or labs, you might find that a specific guide is applicable at multiple sites. However, if guide access is provided through [business units](/power-platform/admin/create-edit-business-units), you can encounter issues when you try to share the guide across sites.

In such cases, you can copy the guide in question and put the copy in the business unit that is associated with the new site. You can then use the copy of the guide either as a functional replica of the original guide or as a template that you reuse steps and tasks, text, images, and 3D objects from when you author guides. In both cases, you not only save your organization authoring time and cost but also ensure consistency in similar procedures across factories.

Your organization should consider the impact that the copy process has on the use of QR codes with deep links, on the content in the guide, and on the related metadata, such as the name and ID.

## Copy process impacts

- **QR code with deep links**: We recommend that you generate a unique QR code for each station or piece of equipment that has an associated guide. In each QR code, [embed a deep link](../pc-app-anchor-embed-qr-code-link.md) to a unique, validated guide in an [execution environment](govern-guides-through-power-platform-environments-and-power-apps.md#example-environment-3-execution-environment). This approach helps you comply with your organization's quality management processes, because only specific, approved guides can be opened on a location. If your organization is using [unique QR codes with deep links](anchor-guides-content-through-qr-codes-and-embed-deep-links.md) to unique, validated guides, when you copy existing guides or use them as templates, you must generate a unique QR code with deep links for the copy.
- **Content in the guide**: When a guide is copied, all content in the copy matches the content in the original. However, it's important to ensure that:

    - The QR code in the guide is replaced with a new, unique QR code (if your organization is using unique QR codes with deep links to unique, validated guides).
    - The new QR code is placed in exactly the same location where the original QR code was placed on the original machinery or equipment. Otherwise, Dynamics 365 Guides can't correctly place content in physical space, because the QR code functions as the anchor point.
    - *All* content in the guide is applicable to the new use case, regardless of how similar the new use case is to the original use case. For example, you might have to update the first step card if the name of the guide is changed, or if it refers to a different standard operating procedure (SOP) than the original guide.
    - All the 3D content that directs user attention is validated and adjusted for correct placement.

- **Metadata**:

    - A copy is automatically registered with a new ID. We recommend that you store the ID of the original guide as hidden metadata. Although this approach isn't mandatory, it enables full traceability in relation to the origin of the copy. You should decide whether to use this approach when you define your [data model](prerequisites-for-implementation-and-planning-roll-out.md).
    - All metadata in a copy must be wiped, and the author must fill in new metadata that corresponds to the appropriate business unit and potential quality assurance (QA) requirements for approval.

## Next steps

- [Asset governance](asset-governance.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
