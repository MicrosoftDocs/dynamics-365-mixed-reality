---
author: davepinch
description: Learn about the different parts of the QR code anchor provided with Dynamics 365 Guides
ms.author: davepinch
ms.date: 09/15/2022
ms.topic: conceptual
title: Guides QR code anchor configuration
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Guides QR code anchor configuration

The following illustration shows the different parts of the QR code anchor provided with Dynamics 365 Guides:

![QR code illustration.](media/qr-code-anchor-dissected.PNG "QR code illustration")

1. **Anchor origin.** This location is used as the guide origin point for all the content in your guide.

1. **Alignment marks.** These marks can assist you in aligning the QR code anchor origin and orientation with specific feature points in your environment.

1. **Anchor width.** We recommend a width of 101 mm to 400 mm for the provided anchor, or for any QR code based on version 1.

1. **Optional cutline.** Cut along this line if you want to make the smallest possible anchor. Graphics above this line visually identify the anchor as a Dynamics 365 Guides anchor. Content below this line, including the margin marked in red, is required for maximizing detection rate.

1. **Module.** This square is one of many modules that make up the QR code anchor. Measure the width
of a module to ensure that it’s at least 3.5 mm in width and height.

   > [!NOTE]
   > When using deep-link QR codes, make sure they have the recommended minimum module size so they can be detected at a comfortable scanning distance.

1. **Anchor quiet zone.** This space is required to help locate the QR code anchor. It must be at least four modules wide. DO NOT CUT THIS PART OFF or you will see degradation in the detection rate.

## Next steps

- [Anchor a guide using a QR code anchor](pc-app-anchor-qr-code.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
