---
author: keno-msft
description: Everything you need to know about converting 3D models to use with Dynamics 365 Guides and Microsoft Power Apps
ms.author: keno
ms.date: 09/11/2020
ms.topic: article
title: Convert your 3D (CAD) models to use with Dynamics 365 Guides and Power Apps
ms.reviewer: v-brycho
---

# Convert your 3D (CAD) models to use with Dynamics 365 Guides or in mixed-reality components included in apps created with Power Apps

To use your 3D models with Microsoft Dynamics 365 Guides or in apps created with Power Apps that include mixed-reality components, you need to convert them to a file format that supports real-time rasterization. 

## Tools for exporting CAD models

You can export CAD models directly to glTF format or into intermediate formats that can be subsequently processed into glTF files. If your content-creation application does not have a glTF exporter, we recommend exporting to [FBX](https://aka.ms/FBXfileformat), [OBJ](https://go.microsoft.com/fwlink/?linkid=2149147), [STL](https://go.microsoft.com/fwlink/?linkid=2149062), or [PLY](https://go.microsoft.com/fwlink/?linkid=2149063), if available. If these formats are not available, there are third-party applications that can import many different file formats and export them as one of these supported file formats. 

Your use of third-party applications is subject to terms between you and the third party. [!include[cc-microsoft](../../includes/cc-microsoft.md)] does not endorse any particular third-party application and assumes no responsibility or liability for any third-party application you elect to use.

|Content-creation package|Description|
|-----------------------------------------------|---------------------------------------------------------------|
[Blender.org Blender](https://aka.ms/Blender_2.8)|Native import/export for Blender 2.8 or later|
[Autodesk 3DS Max](https://aka.ms/BabylonJS_Max2Babylon_Installation)|Babylon.JS plug-in for Max 2015 or later|
[Autodesk Maya](https://aka.ms/BabylonJS_Maya2Babylon_Installation)|Babylon.JS plug-in for Maya 2018 or later|
[Trimble SketchUp](https://aka.ms/SketchUp_glTF_Export)|Separate extensions for [import](https://go.microsoft.com/fwlink/?linkid=2149148) and [export](https://go.microsoft.com/fwlink/?linkid=2149148)|
|[Allegorithmic Substance Painter](https://aka.ms/SubstancePainter_glTF_Exporter)|Native exporter|
|[SideFX Houdini](https://aka.ms/Houdini_glTF_Exporter)|Native import/export|
|[Maxon Cinema 4D](https://go.microsoft.com/fwlink/?linkid=2149064)|Native export plug-in|

In situations where a CAD application doesn’t have an export option for FBX, OBJ, GLB, PLY, STL, or glTF, you can export an intermediate file, such as [JT](https://aka.ms/Jtfileformat) or [STEP](https://aka.ms/STEPfileformat), and then process that file to create a glTF file. 

> [!NOTE]
> For information on working with multiple animations in a single 3D model in 3DS Max, see [Use multiple animation clips in a 3DS Max model](https://doc.babylonjs.com/extensions/Exporters/3DSMax_to_glTF#single-animation-clip).

### See also
[Overview of preparing 3D models](index.md)<br>
[Optimize 3D models](optimize-models.md)<br>
[Best practices for converting and optimizing models](best-practices.md)<br>
[Tutorials for converting and optimizing 3D models](tutorials-overview.md)<br>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
