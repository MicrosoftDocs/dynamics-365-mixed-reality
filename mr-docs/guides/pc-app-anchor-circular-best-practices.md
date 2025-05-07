---
author: alwinv
description: Learn best practices for using circular codes to anchor a guide in Dynamics 365 Guides
ms.author: alwinv
ms.date: 09/14/2023
ms.topic: best-practice
title: Best practices for circular code anchors
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Best practices for circular code anchors

Keep the following points in mind when you work with circular code anchors:

- **Material surface.** Make sure to print the anchor on matte stock, and don't laminate it. Glossy materials can negatively affect scanning due to reflected light. Also, make sure that the anchor is flat. An anchor that is curved or distorted can affect alignment and detection.

- **Same anchor for authoring and printing.** For best accuracy, use the same circular code anchor for authoring and operating.

- **Size.** Make sure that your anchor is the exact size indicated in this article. Incorrect anchor size causes guide misalignment.

  - Some applications and printers might change the size of the image.

  - If the anchor is larger than indicated, HoloLens interprets the scale difference in distance. Therefore, the anchor is identified as closer than it really is.

  - The best way to make sure that the anchor isn't resized is to print it from the PDF file.

[!INCLUDE [anchor-best-practices-location](../includes/anchor-best-practices-location.md)]

[!INCLUDE [anchor-best-practices-scanning-angle](../includes/anchor-best-practices-scanning-angle.md)]

  - Ideal scanning range is from 60 to 80 cm.

## Next steps

- [Anchor a guide using a circular code anchor](pc-app-anchor-circular-code.md)
- [Effect of calibration, prescanning, and environment](pc-app-anchor-improve-hologram-precision.md)
- [Effect of anchor types/placement](pc-app-anchor-types-placement-precision.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
