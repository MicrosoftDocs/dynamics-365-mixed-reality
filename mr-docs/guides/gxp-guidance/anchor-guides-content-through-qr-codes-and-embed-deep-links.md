---
title: Anchor guides content through QR codes and embed deep links
description: Learn about anchoring guides content to pieces of equipment with QR codes and embedded QR code links when implementing Dynamics 365 Guides in a regulated industry
ms.date: 03/13/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Anchor guides content through QR codes and embed deep links

As an instructional tool, the attractiveness and effectiveness of Guides partly stem from the use of 3D content such as arrows to nudge end-users' attention towards specific points of interest on machinery.

To create a successful and safe guide, the author should follow [3D object best practices](../hololens-app-place-holograms.md#best-practices-for-working-with-3d-content) when authoring instructions and your organization needs to choose a way for Guides to continuously place holograms correctly in physical space (where the author intends a hologram to appear in relation to machinery).

For example, if a 3D arrow indicates that the end-user must connect a wire to socket three out of five neighboring sockets, all stakeholders in your organization want to ensure an accurate placement of the hologram. Otherwise, you risk misguiding the operator and potentially cause an incorrect, potentially dangerous, assembly or operation of equipment.  

The placing of 3D objects in space is achieved through one of [four available anchoring methods](../pc-app-anchor.md#four-ways-to-anchor-a-guide): Azure Object Anchors (in preview), QR code anchor, circular code anchor, and holographic anchor.

For Guides usage in a regulated setting, the [QR code anchor](../pc-app-anchor-qr-code.md) is the recommended anchoring method. When using this method, a guide is launched by scanning a digital or printed QR code through the HoloLens, and all 3D elements are positioned in the production area with the QR code representing point zero in X Y Z axis.

We recommend generating a unique QR code for each station or piece of equipment that has an associated guide and [embed a deep link](../pc-app-anchor-embed-qr-code-link.md) in each QR code to a unique, validated, guide existing in an execution environment. This approach helps you be compliant with your organization's quality management processes because only approved and specific guides can be launched on location.

Without deep links embedded, operators are presented with an overview of selectable guides from the execution environment with the risk of selecting the wrong guide. This poses a risk, particularly if you have machinery with similar instructions, or have multiple guides for the same machinery, like switching settings.

When working with QR code anchors at a production site, best practices regarding [printing settings, size, location, orientation, and contrast](../pc-app-anchor-qr-code.md#best-practices-for-qr-code-anchors) help you succeed with anchoring and expedite QA validation of your guides. However, your industry's specific requirements might collide with these anchor best practices: you might be forced to compromise with best practices to stay compliant. For example, your organization requires laminated QR codes in a lab setting, even though glossy materials can negatively affect scanning due to reflected light.

## Next steps

- [Reusage of guides across sites](reusage-of-guides-across-sites.md)
