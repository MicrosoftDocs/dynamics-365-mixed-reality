---
author: alwinv
description: Understand common reasons why Azure Object Anchors might fail when anchoring a guide
ms.author: alwinv
ms.date: 07/07/2023
ms.topic: troubleshooting-general
title: Troubleshoot Azure Object Anchors
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Troubleshoot anchoring a guide with Azure Object Anchors (Preview)

Common errors that might occur when anchoring a guide in Dynamics 365 Guides with Azure Object Anchors.

## 3D model conversion failure

The top reasons for 3D model conversion failure in the Guides model-driven app include:

- The 3D model uses an unsupported file format.

- The physical dimensions of the 3D model are larger than 10 meters or smaller than 1 meter.

- The 3D model file is bigger than the maximum supported file size (150 MB).

For more information, see [best practices for choosing a target object](pc-app-anchor-azure-object.md#best-practices-for-choosing-a-target-object-for-your-object-anchor) and [convert the file](pc-app-anchor-azure-object.md#convert-the-file-in-the-guides-model-driven-app).

## Object anchor failure on HoloLens

The top reasons for object anchor failure on HoloLens include:

- Incorrect **Length Unit** type specified during model conversion.

- Incorrect gravity direction specified during model conversion.

- The 3D model provided during model conversion doesn't resemble the surfaces of the actual object detected by the HoloLens sensors.

You can confirm object measurements and **Length Unit** type by double-clicking the object anchor in the PC app to open the **Properties** tab.
  
![Properties tab with My chair measurements](media/AOA-chair-properties.PNG "Properties tab with My chair measurements")

- If the dimensions of the object in the **Properties** tab are different from the actual object dimensions by a factor of 2 or more, an incorrect **Length Unit** type was likely used.

- If the gravity direction of the model in the **Properties** tab (the down direction) is different from the actual orientation of the object in its environment, an incorrect gravity direction was likely used (for example, if the chair in the above example is shown upside down or with its legs pointing to the side instead of pointing down).

3D models that are converted correctly may not be detected on HoloLens if their model geometries differ greatly from the surfaces detected by HoloLens. You can view the object anchor geometry in the **Properties** tab and compare that with the Surface Reconstruction (SR) mesh of the object as seen by HoloLens. To view the object’s SR mesh, air tap while viewing the object in the HoloLens shell. A large difference in geometry between the anchor geometry and SR mesh indicates potential difficulty with object anchoring.
