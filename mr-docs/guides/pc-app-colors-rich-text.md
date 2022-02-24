---
author: amaraanigbo
description: Learn about using rich text formatting in instruction card text for Dynamics 365 Guides
ms.author: soanigbo
ms.date: 01/18/2022
ms.topic: article
title: Use rich text formatting in instruction card text in Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# Use rich text formatting for instruction card text in Dynamics 365 Guides

> [!NOTE]
> This is an unsupported feature and is subject to change.

If you want to use colors or rich-text formatting (bold, color, italic, font size, or underline) in your Dynamics 365 Guides instruction card text, you can add a small subset of HTML markup directly to an instruction card in the PC app.

**HTML markdown in the PC app**

![Screenshot of PC app with HTML markdown in instruction card.](media/HTML-pc-app.jpg "Screenshot of PC app with HTML markdown in instruction card")

**Results shown in HoloLens app**

![Screenshot of HoloLens app with HTML results.](media/html-hololens-app.jpg "Screenshot of HoloLens app with HTML results")

The following subset of tags are supported.

|Tag|Description|
|--------------|---------------------------------------------------------------------------------------|
|``<b>``|Bold.|
|``<color=*argument*>``|Text color. The argument can be a hexadecimal code beginning with # or a named color. Hexadecimal colors begin with '#' and may be RGB (six characters). Recognized color names are: "black", "blue", "green", "orange", "purple", "red", "white", and "yellow". Make sure to use lowercase for colors ("yellow", for example). Otherwise, the colors won't be applied. For Cyan, use the hex code #00FFFF.|
|``<i>``|Italic.|
|``<size=*argument*>``|Font size. The argument is a number, followed by one of the following units: "px", "em", or "%". If no unit is given, "px" is implied. In the Dynamics 365 Guides 3D UI, one "pixel" equals about one-half millimetre and the base text size is 16.8 mm. Percentages and "em" units set the text size relative to the base size. For example, "120%" and "1.2em" are equivalent. To prevent the UI from overflowing, Dynamics 365 Guides sets a minimum size of 70% (22px) and maximum of 130% (42px).
|``<u>``|Underline.|
