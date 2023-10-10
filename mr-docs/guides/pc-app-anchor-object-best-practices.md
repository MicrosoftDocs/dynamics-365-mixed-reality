---
author: alwinv
description: Learn best practices for using object anchors to anchor a guide in Dynamics 365 Guides
ms.author: alwinv
ms.date: 09/14/2023
ms.topic: conceptual
title: Best practices for choosing a target object for your object anchor
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Best practices for choosing a target object for your object anchor

Keep the following recommendations in mind when choosing a target object for your object anchor.

## Static objects

For best results, target objects should be fixed and stationary during the scanning process. They shouldn't have any parts that change during scanning or differ from the 3D source model as it might impact HoloLens ability to detect the object.

## Object size

To achieve accurate detection and alignment, the target object should be 1–10 meters for each dimension.

![Diagram showing minimum object size](media/AOA-object-size.PNG "Diagram showing minimum object size")

## Topology

Object anchors works best on larger objects that have unique surfaces and asymmetric features.

- Don't use symmetrical objects, which can cause confusion about the orientation of the object.

- Use objects that have unique shapes and edges.

- Don't use objects that are mainly composed of thin pipes or wires.

## Object detection

Prior to starting object detection, make sure that your HoloLens 2 has a good understanding of the space by prescanning your environment before doing object detection. Look at the surrounding walls and unique objects with your HoloLens.

Then look at your target object to avoid false positives, which allows HoloLens to easily differentiate and detect the object. For larger objects, move around the object so that HoloLens is able to generate a better representation of the physical space. Stand in one spot to limit the amount of surface information, which means that HoloLens might not meet its detection thresholds.

## Materials

Highly reflective and dark materials are difficult to detect with HoloLens. If HoloLens is unable to detect the surface, object anchors can't use sensor data for alignment and detection.

## Next steps

- [Anchor a guide using object anchors](pc-app-anchor-object.md)
- [Effect of calibration, prescanning, and environment](pc-app-anchor-improve-hologram-precision.md)
- [Effect of anchor types/placement](pc-app-anchor-types-placement-precision.md)