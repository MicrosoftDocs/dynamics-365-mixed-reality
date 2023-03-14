---
title: Reusage of guides across sites
description: Learn about using guides across multiple sites in a regulated industry and how to avoid issues
ms.date: 03/13/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Reusage of guides across sites

If you have similar production lines or machinery across factories or labs, you might find that a specific guide is applicable at multiple sites. However, if guide access is provided through business units, you can encounter issues with cross-site sharing of guides.  
  
In such instances, the guide in question can be copied and the copy subsequently placed in the business unit associated with the new site. In this way, the copy guide can be utilized as a functional replica of the original guide, or the copied guide can be utilized as a template from which steps and tasks, text, images, and 3D models are reused during guides authoring. Potentially, replicating existing guides or utilizing them as templates for new guides might not only save your organization authoring time and cost, but also ensure consistency in similar procedures across factories.

However, we recommend that your organization pay particular attention to the impact the copy process has on, among other things, the usage of QR codes with deep links, content in the guide and the related metadata such as name and ID.

We recommend generating a unique QR code for each station or piece of equipment that has an associated guide and [embed a deep link](../pc-app-anchor-embed-qr-code-link.md) in each QR code to a unique, validated, guide existing in an execution environment. This approach helps you be compliant with your organization's quality management processes because only approved and specific guides can be launched on location.

**QR code with deep links**

- If your organization, as recommended, generates unique QR codes with deep links to unique validated guides, you still have to do this when replicating existing guides or utilizing guides as templates.

**Metadata**

- A copy is automatically registered with a new ID. While not mandatory, we recommend storing the ID of the original guide as hidden metadata. This approach enables full traceability in relation to the origin of the copy. Whether or not to store the ID of the original guide as hidden metadata, the copy guide is something to decide upon when defining your data model.

- All metadata in a copy must be wiped and the author must fill out new metadata that corresponds to the given business unit and potential QA requirements for approval.

**The content in the guide**

When copied, all guide content matches the content in the original. However, it is of utmost importance to ensure that:

- The QR code in the guide is replaced with the new, unique QR code (in the case your organization is using unique QR codes with deep links to unique, validated guides).

- The QR code is placed at the exact same location as on the original machinery or equipment. Otherwise, Guides can't place content correctly in physical space since the QR code functions as the anchor point.

- All content within the guide is applicable for the new use case however similar the use case might be to the original. Your organization can face instances where information in the first step card needs to be updated, for example, if the name of the guide is changed, or if it refers to another SOP than the original guide.

- All the 3D content shepherding end-user attention must be validated and adjusted for correct placement.

- If your organization, as recommended, generates unique QR codes with deep links to unique validated guides, you will still have to do this when replicating existing guides or utilizing guides as templates.

## Next steps

- [Asset governance](asset-governance.md)
