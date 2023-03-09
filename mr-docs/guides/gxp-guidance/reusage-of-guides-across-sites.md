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

# Reusage of guides across sites

If you have similar production lines or machinery across factories or labs, you might find that a specific guide is applicable at multiple sites. However, if guide access is provided through Business Units, you can encounter issues with cross-site sharing of guides.  
  
In such instances, the guide in question can be copied and the copy subsequently placed in the Business Unit associated with the new site. In this way, the copy guide can be utilized as a functional replica of the original guide, or the copied guide can be utilized as 2) a template from which steps and tasks, i.e., orchestrations of text, images, 3D models etc., are reused during guides authoring. Potentially, replicating existing guides or utilizing them as templates for new guides might not only save your organization authoring time (and hereby cost) but also ensure consistency in similar procedures across factories.

However, it is recommended that your organization pays particular attention to the impact the copy process has on, among other things, the usage of QR codes with deep links, content in the guide and the related metadata such as name, ID etc.

It is recommended to generate a unique QR code for each station, equipment etc. that has an associated guide and [<u>embed a deep link</u>](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/pc-app-anchor-embed-qr-code-link) in each QR code to a unique, validated, guide existing in an Execution environment. This will assist you in being compliant with your organization's quality management processes because only approved and specific guides will be launchable on location.

**QR code with deep links**

-   If your organization, as recommended, generates unique QR codes with deep links to unique validated guides, you will still have to do this when replicating existing guides or utilizing guides as templates.

**Metadata**

-   The copy will automatically be registered with a new ID. While not mandatory, it is advised to store the ID of the original guide as hidden metadata. This enables full traceability in relation to the origin of the copy. Whether or not to store the ID of the original guide as hidden metadata the copy guide is something you will decide upon when defining your data model.

-   All metadata in the copy needs to be wiped and the author must fill out new metadata that corresponds to the given Business Unit and potential QA requirements for approval.

**The content in the guide**

When copied, all guide content will match the content in the original. However, it is of utmost importance to ensure that:

-   the QR code in the guide is replaced with the new, unique QR code (in the case your organization is using unique QR codes with deep links to unique, validated guides)

-   the QR code is placed at the exact same location as on the original machinery or equipment. Otherwise, Guides can't place content correctly in physical space since the QR code function as anchor point.

-   all content within the guide is applicable for the new use case however similar the use case might be to the original. Your organization can face instances where information in the first step card needs to be updated, for example, if the name of the guide is changed, or if it refers to another SOP than the original guide.

-   all the 3D content shepherding end-user attention must be validated and adjusted for correct placement.

-   (if your organization, as recommended generates unique QR codes with deep links to unique validated guides


