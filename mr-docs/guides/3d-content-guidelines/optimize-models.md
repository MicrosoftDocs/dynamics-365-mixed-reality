---
author: keno-msft
description: How to optimize your 3D (CAD) models to use with Dynamics 365 Guides and Microsoft Power Apps
ms.author: keno
ms.date: 05/25/2021
ms.topic: article
title: Optimize your 3D models to use with Dynamics 365 Guides and Power Apps
ms.reviewer: v-bholmes
---

# Optimize your 3D models to use with Dynamics 365 Guides or in mixed-reality components included in apps created with Power Apps

For best rendering and best possible real-time performance, your 3D models need to be converted and might need to be optimized before using with Dynamics 365 Guides or in an app created with Power Apps that includes mixed-reality components. Third-party applications that convert CAD files often have tools that can optimize content as well. 

The following table lists software tools that you can use to convert and/or optimize your CAD files or intermediate files and export them as a supported file format. Your use of third-party applications is subject to terms between you and the third party. [!include[cc-microsoft](../../includes/cc-microsoft.md)] does not endorse any particular third-party application and assumes no responsibility or liability for any third-party application you elect to use.

|Software|Import|Export|Convert/transcode|Optimization|
|---------------------------------|----------------------------------------|--------------------|--------------------|-------------------|
|[PiXYZ Software](https://aka.ms/Pixyz)|STEP, Catia, JT, OBJ, FBX, and [more](https://www.pixyz-software.com/documentations/html/2020.1/studio/SupportedFileFormats.html)|glTF 2.0 and more|Yes|Yes|
|[Maxon Cinema 4D](https://aka.ms/MaxonCinema4D)|SOLIDWORKS, STEP, Catia, JT, and IGES|FBX, OBJ, GLB/glTF 2.0 (beta)|Yes|Yes|
|[Simplygon Studios](https://aka.ms/Simplygonsoftware)|FBX, OBJ|FBX|No|Yes|
|[Unreal Datasmith](https://aka.ms/UnrealDatasmithsoftware)|STEP, Catia, JT, OBJ, FBX, and more|FBX, OBJ|Yes|No|
|[Autodesk Inventor](https://aka.ms/AutodeskInventorSoftware)|STEP, Catia, JT, OBJ, FBX, and more|FBX, OBJ, STL|Yes|Yes|
|[Blender](https://www.blender.org/)|Collada (DAE), FBX, PLY, OBJ, STL, glTF, GLB, and more|FBX, OBJ, glTF 2.0, and more|Yes|Yes|

> [!IMPORTANT]
> Dynamics 365 Guides uses meters as the default scale unit. If your 3D model scale is set to millimeters when you export from your CAD solution, the model will be converted to meters in Dynamics 365 Guides. For example, if your model is 50 millimeters, it will be converted to 50 meters. To ensure size consistency between your CAD solution and Dynamics 365 Guides, make sure to set your model scale unit to meters when you  export. 

<br>
Here are examples of CAD, converted, and optimized 3D models.<br></br>

|CAD|Converted to GLB|Optimized GLB|
|------------------------------------------|----------------------------------------------|----------------------------------------------|
|![CAD illustration](media/CAD.PNG "CAD illustration")|![GLB illustration](media/GLB.PNG "GLB illustration")|![Optimized GLB illustration](media/optimized-GLB.PNG "Optimized GLB illustration")|
|Original CAD file|52,000 triangles|9,000 triangles|

## Performance targets

Dynamics 365 Guides is used on [!include[cc-microsoft](../../includes/cc-microsoft.md)] [!include[pn-hololens](../../includes/pn-hololens.md)]. Power Apps mixed-reality components can be used on any [ARCore-capable device](https://developers.google.com/ar/discover/supported-devices) and [certain Apple iOS devices](https://www.apple.com/augmented-reality/). Regardless of the device used, the goal is to provide the highest possible visual fidelity without adversely affecting performance. 

The following table lists some general conservative targets to aim for when acquiring or authoring 3D models for a range of hardware. When in doubt, target the midrange profile for a balance of fidelity and performance. 

|Device|Low-scene complexity<br>![Low complexity graphic](media/simple.PNG "Low complexity graphic")|Medium-scene complexity<br>![Medium complexity graphic](media/medium.PNG "Medium complexity graphic")|High-scene complexity<br>![High complexity graphic](media/complex.PNG "High complexity graphic")|
|--------------|---------------------------|-----------------------------------|-----------------------------------|
|![HoloLens graphic](media/hololens.PNG "HoloLens graphic")<br>HoloLens|**Objects:**<br>1-3 per scene<br><br>**Triangles:**<br><100,000<br><br>**Materials:**<br>1-2 per object|**Objects:**<br>4-10 per scene<br><br>**Triangles:**<br><30,000<br><br>**Materials:**<br>1-2 per object|**Objects:**<br>10+ per scene<br><br>**Triangles:**<br><10,000<br><br>**Materials:**<br>1-2 per object|
|![Immersive headset graphic](media/immersive-headset.PNG "Immersive headset graphic") <br>Immersive headsets|**Objects:**<br>1-3 per scene<br><br>**Triangles:**<br><15,000,000<br><br>**Materials:**<br>1-2 per object|**Objects:**<br>4-10 per scene<br><br>**Triangles:**<br><500,000<br><br>**Materials:**<br>1-2 per object|**Objects:**<br>10+ per scene<br><br>**Triangles:**<br><150,000<br><br>**Materials:**<br>1-2 per object|
|![Mobile graphic](media/mobile.PNG "Mobile graphic") <br>Mobile|**Objects:**<br>1-3 per scene<br><br>**Triangles:**<br><500,000<br><br>**Materials:**<br>1-2 per object|Not applicable|Not applicable|

> [!NOTE]
> Transparency in materials such as glass in 3D models is not supported.
> 
> Dynamics 365 Guides includes a GTLF loader that does not support alpha transparency in textures. However, you can set a single alpha value for an entire material.

### See also
[Overview of preparing 3D models](index.md)<br>
[Convert 3D models](convert-models.md)<br>
[Best practices for converting and optimizing 3D models](best-practices.md)<br>
[Tutorials for converting and optimizing 3D models](tutorials-overview.md)<br>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
