---
author: amaraanigbo
description: Learn about using rich text formatting in instruction card text for Dynamics 365 Guides
ms.author: soanigbo
ms.date: 02/24/2022
ms.topic: article
title: Use rich text formatting in instruction card text in Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# Use rich text formatting in instruction card text in Dynamics 365 Guides

> [!NOTE]
> This is an unsupported feature and is subject to change.

If you want to use colors or rich-text formatting (bold, color, italic, font size, or underline) in your Dynamics 365 Guides instruction card text, you can add a small subset of HTML tags directly to an instruction card in the PC app.

**HTML tags in the PC app**

![Screenshot of PC app with HTML markdown in instruction card.](media/HTML-pc-app.jpg "Screenshot of PC app with HTML markdown in instruction card")

**Results in the HoloLens app**

![Screenshot of HoloLens app with HTML results.](media/html-hololens-app.jpg "Screenshot of HoloLens app with HTML results")

## Supported tags

Dynamics 365 Guides supports the following subset of tags.

|Tag|Description|
|--------------|---------------------------------------------------------------------------------------|
|``<b>``|Bold.|
|<color=*argument*>|Text color. The argument can be a hexadecimal code beginning with # or a named color. Hexadecimal colors can be RGB (six characters). Recognized color names are black, blue, green, orange, purple, red, white, and yellow. **NOTE:** Make sure to use lowercase for colors ("yellow", for example). Otherwise, the colors won't be applied. For cyan, use the hexadecimal code #00FFFF.|
|``<i>``|Italic.|
|<size=*argument*>|Font size. The argument is a number, followed by one of the following units: px, em, or %. If no unit is given, px (pixel) is implied. In the Dynamics 365 Guides 3D UI, one px equals about one-half millimeter and the base text size is 16.8 mm. Percentages and em units set the text size relative to the base size. For example, "120%" and "1.2em" are equivalent. To prevent the UI from overflowing, Dynamics 365 Guides sets a minimum size of 70% (22px) and maximum of 130% (42px).
|``<u>``|Underline.|
