---
author: alwinv
description: Learn best practices for using Object Anchors to anchor a guide in Dynamics 365 Guides
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

For best results, target objects should be fixed and stationary during the scanning process. They should not have any parts that change during scanning or differ from the 3D source model as this might impact HoloLens ability to detect the object.

## Object size

To achieve accurate detection and alignment, the target object should be 1–10 meters for each dimension, as shown below.

![Diagram showing minimum object size](media/AOA-object-size.PNG "Diagram showing minimum object size")

## Topology

Object Anchors works best on larger objects that have unique surfaces and asymmetric features.

- Do not use symmetrical objects as this can cause confusion about the orientation of the object.

- Use objects that have unique shapes and edges.

- Do not use objects that are mainly composed of thin pipes or wires.

## Object detection

Prior to starting object detection, make sure that your HoloLens 2 has a good understanding of the space by pre-scanning your environment before doing object detection. Look at the surrounding walls and unique objects with your HoloLens.

Then look at your target object to avoid false positives. This allows HoloLens to easily differentiate and detect the object. For larger objects, move around the object so that HoloLens is able to generate a better representation of the physical space. Standing in one spot limits the amount of surface information, which means that HoloLens might not meet its detection thresholds.

## Materials

Highly reflective and dark materials are difficult to detect with HoloLens. If HoloLens is unable to detect the surface, Object Anchors will not be able to use sensor data for alignment and detection.

## Next steps

- [Anchor a guide by using Object Anchors](pc-app-anchor-azure-object.md)