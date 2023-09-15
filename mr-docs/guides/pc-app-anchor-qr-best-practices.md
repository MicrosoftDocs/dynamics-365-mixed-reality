---
author: alwinv
description: Learn best practices for using QR codes to anchor a guide in Dynamics 365 Guides
ms.author: alwinv
ms.date: 09/14/2023
ms.topic: conceptual
title: Best practices for QR code anchors
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Best practices for QR code anchors

Keep the following points in mind when working with QR code anchors:

- **Printing settings**. Make sure to print the anchor on matte stock and don't laminate it.

  - Glossy materials can negatively affect scanning due to reflected light.

  - Bubblejet printers produce a better matte finish.

- **Size**. You can print QR codes in multiple sizes. For best detection and scanning comfort, we recommend printing the provided anchor with a width of **101 mm to 400 mm**. This recommendation is for any QR code anchor following Version 1 QR codes. Anchor sizes outside of this recommended range might result in detection failure or reduced alignment precision for version 1 QR codes.

  > [!NOTE]
  > If you use your own QR code anchor, refer to QRCode.com for additional advanced QR code documentation. QR codes other than version 1 can increase the number of modules, which decreases their relative size. We recommend printing your anchor at a size where each independent module side measures a minimum of 3.5 mm.

    Anchors that are smaller than the recommended size impact the user experience while scanning. Due to the position of the QR scanning cameras, users need to aim below the anchor and may need to get uncomfortably close for scanning to succeed. Smaller sizes are also sensitive to variable lighting conditions. Any small reflective highlights on the anchor might cause a smaller anchor to have more of the information obscured, making the anchor unreadable.

    Anchors that are larger than the recommended size require users to move father away from the anchor. Scanning from a greater distance results in decreased accuracy.

- **Position**. Make sure that the anchor is always positioned flat. Don't distort it or place it on a curved surface. Otherwise, alignment and detection will be negatively affected.

[!INCLUDE [anchor-best-practices-location](../includes/anchor-best-practices-location.md)]

- **Orientation**. The way that you orient the anchor can have a big impact on scanning performance.

  - Position the anchor on a vertical surface to minimize light reflections, if possible.

  - Don't use reflective materials for the support surface.

  - Very reflective surfaces that are located behind the anchor, and direct exposure to sun or artificial light, can negatively affect scanning performance.

[!INCLUDE [anchor-best-practices-scanning-angle](../includes/anchor-best-practices-scanning-angle.md)]

  - The ideal scanning range is from 50 to 150 centimeters (cm).

- **Contrast**. The brightness for the provided anchor is set to a 30-percent gray background. This setting provides the best adaptability for a wide variety of environments.

  - If you have trouble detecting an anchor that you provide, try to adjust the anchor's image brightness so that it matches the average environmental brightness around the anchor.

## Next steps

- [Anchor a guide using a QR code anchor](pc-app-anchor-QR-code.md)
- [Effect of calibration, pre-scanning, and environment](pc-app-anchor-improve-hologram-precision.md)
- [Effect of anchor types/placement](pc-app-anchor-types-placement-precision.md)
- [More best practices for QR code detection](/windows/mixed-reality/develop/advanced-concepts/qr-code-tracking-overview#best-practices-for-qr-code-detection)