---
title: Anchor guide content through QR codes and embed deep links
description: Learn about using QR codes and embedded QR code links to anchor guide content to pieces of equipment when you implement Dynamics 365 Guides in a regulated industry.
ms.date: 09/14/2023
ms.topic: conceptual
author: prashantyvr
ms.author: prashan
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Anchor guide content through QR codes and embed deep links

One reason why Dynamics 365 Guides is attractive and effective as an instructional tool is that 3D content such as arrows can be used to nudge the user's attention toward specific points of interest on machinery.

To create successful and safe guides, authors should follow [3D object best practices](../hololens-app-place-holograms.md#best-practices-for-working-with-3d-content) when they author instructions. In addition, your organization should choose a way to ensure that Guides correctly places holograms in physical space, in the exact locations where the author intends holograms to appear in relation to machinery. For example, if there are five sockets next to each other, and a 3D arrow should indicate that the user must connect a wire to socket 3, all stakeholders in your organization want to ensure accurate placement of the hologram. Otherwise, there is a risk that you will misguide the operator and cause equipment to be assembled or operated in an incorrect and potentially dangerous manner.  

3D objects are placed in space through one of [four anchoring methods](../pc-app-anchor.md#four-ways-to-anchor-a-guide):

- Object anchors (in preview)
- QR code anchors
- Circular code anchors
- Holographic anchors

If Guides is used in a regulated setting, [QR code anchors](../pc-app-anchor-qr-code.md) are the recommended anchoring method. An operator then opens a guide by scanning a digital or printed QR code through a HoloLens device. All 3D elements are positioned in the production area, and the QR code represents point zero on the X, Y, and Z axes.

We recommend that you generate a unique QR code for each station or piece of equipment that has an associated guide. In each QR code, [embed a deep link](../pc-app-anchor-embed-qr-code-link.md) to a unique, validated guide in an [execution environment](govern-guides-through-power-platform-environments-and-power-apps.md#example-environment-3-execution-environment). This approach helps you comply with your organization's quality management processes, because only specific, approved guides can be opened for a location.

If deep links aren't embedded, operators get an overview of all the guides that are available for selection in the execution environment. Therefore, there is a risk that they will select the incorrect guide, especially if different machinery has similar instructions or the same machinery has multiple guides.

Follow the [best practices for print settings, size, location, orientation, and contrast](../pc-app-anchor-qr-best-practices.md) for QR code anchors at a production site. These practices help you successfully anchor and do quality assurance (QA) validation of your guides. However, they might sometimes conflict with your industry's specific requirements. For example, your organization might require laminated QR codes in a lab setting, even though glossy materials can negatively affect scanning because of reflected light. Therefore, to remain compliant, you might have to compromise about best practices.

## Next steps

- [Reuse guides across sites](reuse-guides-across-sites.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
