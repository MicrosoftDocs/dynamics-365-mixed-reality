---
author: RobertButterworthMS
ms.author: robutter
description: Learn how to review a 3D object after exporting it as a GLB file to make sure it meets performance targets for Microsoft Dynamics 365 Guides or Power Apps.
ms.date: 02/02/2022
ms.topic: how-to
title: Review a 3D object to use with Dynamics 365 Guides or Power Apps
ms.reviewer: v-brycho
---

# Review a 3D object to use with Dynamics 365 Guides or Power Apps

After exporting a GLB file to use with Microsoft Dynamics 365 Guides or Power Apps, you can preview it with the Windows [3D Viewer](https://www.microsoft.com/p/3d-viewer/9nblggh42ths). Use 3D Viewer to visualize the individual texture channels and view stats. Information like triangle count and draw calls help confirm that the model [meets the recommended performance targets](optimize-models.md#performance-targets).

1. Open [3D Viewer](https://www.microsoft.com/p/3d-viewer/9nblggh42ths).

2. Drag a GLB file into the viewport (or select **File** > **Open** to browse for a GLB file).

3. Select the **Stats & Shading** tab on the right side of the screen to start visualizing different components of the GLB file.

4. Use the check boxes to turn the different viewport visualizations on or off.

5. If your device has a camera, you can move the **Mixed reality** slider to the **On** position and place the asset to preview it in your world.

    ![Screenshot of 3D Viewer.](media/review-3d-model.jpg "Screenshot of 3D Viewer")

Ensure that your model conforms to the [recommended optimization](optimize-models.md#performance-targets) for the platform you're creating content for.

> [!TIP]
> The [Babylon.JS Web Viewer](https://sandbox.babylonjs.com/) is another great option if uploading the model is not a concern.

If the model requires further editing or animation work in another staging application, use an intermediate file format like FBX. FBX is an
 Autodesk exchange format designed to preserve authoring data that might be required by your staging application.

## See also

- [Overview of preparing 3D objects](index.md)
- [Convert 3D objects](convert-models.md)
- [Optimize 3D objects](optimize-models.md)
- [Tutorials for converting and optimizing 3D objects](tutorials-overview.md)
- [Best practices for converting and optimizing 3D objects](best-practices.md)
