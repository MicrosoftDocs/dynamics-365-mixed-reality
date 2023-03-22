---
title: Reuse guides across sites
description: Learn about using guides across multiple sites in a regulated industry and how to avoid issues
ms.date: 03/21/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Reuse guides across sites

If you have similar production lines or machinery across factories or labs, you might find that a specific guide is applicable at multiple sites. However, if guide access is provided through [business units](/power-platform/admin/create-edit-business-units), you can encounter issues with cross-site sharing of guides.  
  
In such instances, you can copy the guide in question and place the copy in the business unit associated with the new site. In this way, you can use the copy guide as a functional replica of the original guide or as a template from which you can reuse steps and tasks, text, images, and 3D models during guides authoring. Potentially, replicating existing guides or utilizing them as templates for new guides might not only save your organization authoring time and cost, but also ensure consistency in similar procedures across factories.

We recommend that your organization consider the impact the copy process has on the use of QR codes with deep links, content in the guide, the related metadata such as name and ID.

We recommend generating a unique QR code for each station or piece of equipment that has an associated guide and [embed a deep link](../pc-app-anchor-embed-qr-code-link.md) in each QR code to a unique, validated guide in an [execution environment](govern-guides-through-power-platform-environments-and-power-apps.md#example-environment-3-execution-environment). This approach helps you be compliant with your organization's quality management processes because only approved and specific guides can be launched on location.

## Copy process impacts

- **QR code with deep links**: If your organization [generates unique QR codes with deep links](anchor-guides-content-through-qr-codes-and-embed-deep-links.md) to unique, validated guides when copying existing guides or using guides as templates, you must generate a unique QR code with deep links for the copy.

- **Metadata**

  - A copy is automatically registered with a new ID. While not mandatory, we recommend storing the ID of the original guide as hidden metadata. This approach enables full traceability in relation to the origin of the copy. Whether or not to store the ID of the original guide as hidden metadata, the copy guide is something to decide upon when defining your [data model](prerequisites-for-implementation-and-planning-roll-out.md).
  - All metadata in a copy must be wiped and the author must fill out new metadata that corresponds to the given business unit and potential quality assurance (QA) requirements for approval.

- **Content in the guide**: When copied, all guide content matches the content in the original. However, it is important to ensure that:

  - The QR code in the guide is replaced with the new, unique QR code (in the case your organization is using unique QR codes with deep links to unique, validated guides).
  - The QR code is placed at the exact same location as on the original machinery or equipment. Otherwise, Guides can't place content correctly in physical space since the QR code functions as the anchor point.
  - All content within the guide is applicable for the new use case however similar the use case might be to the original. For example, you might need to update the first step card if the name of the guide is changed or it refers to another standard operating procedure (SOP) than the original guide.
  - All the 3D content shepherding end-user attention must be validated and adjusted for correct placement.

## Next steps

- [Asset governance](asset-governance.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
