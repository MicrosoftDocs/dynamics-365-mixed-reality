---
author: keno-msft
description: How to optimize your 3D (CAD) models to use with Dynamics 365 Import Tool (Preview).
ms.author: v-jerja
ms.date: 01/08/2020
ms.service: crm-online
ms.topic: article
title: Optimize your 3D models
ms.reviewer: v-brycho
---

# Optimize your 3D models

For best rendering and best possible real-time performance, your 3D models need to be converted and might need to be optimized before using [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)]. Third-party applications that convert CAD files often have tools that can optimize content as well. 

The following table lists software tools that you can use to convert and/or optimize your CAD files or intermediate files and export them as a supported file format. Your use of third-party applications is subject to terms between you and the third party. [!include[cc-microsoft](../includes/cc-microsoft.md)] does not endorse any particular third-party application and assumes no responsibility or liability for any third-party application you elect to use.

|Software|Import|Export|Convert/transcode|Optimization|
|---------------------------------|----------------------------------------|--------------------|--------------------|-------------------|
|[PiXYZ Software](https://aka.ms/Pixyz)|STEP, Catia, JT, OBJ, FBX, and more|glTF 2.0|Yes|Yes|
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

The [!include[pn-dyn-365](../includes/pn-dyn-365.md)] mixed-reality applications can be used on [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-hololens](../includes/pn-hololens.md)], immersive headsets, and mobile devices. The goal is to provide the highest possible visual fidelity without adversely affecting performance. 

The following table lists some general conservative targets to aim for when acquiring or authoring 3D models for a range of hardware. When in doubt, target the midrange profile for a balance of fidelity and performance. 

||Low-scene complexity<br>![Low complexity graphic](media/simple.PNG "Low complexity graphic")|Medium-scene complexity<br>![Medium complexity graphic](media/medium.PNG "Medium complexity graphic")|High-scene complexity<br>![High complexity graphic](media/complex.PNG "High complexity graphic")|
|--------------|---------------------------|-----------------------------------|-----------------------------------|
|![HoloLens graphic](media/hololens.PNG "HoloLens graphic")<br>HoloLens|**Objects:**<br>1-3 per scene<br><br>**Triangles:**<br><100,000<br><br>**Materials:**<br>1-2 per object|**Objects:**<br>4-10 per scene<br><br>**Triangles:**<br><30,000<br><br>**Materials:**<br>1-2 per object|**Objects:**<br>10+ per scene<br><br>**Triangles:**<br><10,000<br><br>**Materials:**<br>1-2 per object|
|![Immersive headset graphic](media/immersive-headset.PNG "Immersive headset graphic") <br>Immersive headsets|**Objects:**<br>1-3 per scene<br><br>**Triangles:**<br><15,000,000<br><br>**Materials:**<br>1-2 per object|**Objects:**<br>4-10 per scene<br><br>**Triangles:**<br><500,000<br><br>**Materials:**<br>1-2 per object|**Objects:**<br>10+ per scene<br><br>**Triangles:**<br><150,000<br><br>**Materials:**<br>1-2 per object|
|![Mobile graphic](media/mobile.PNG "Mobile graphic") <br>Mobile|**Objects:**<br>1-3 per scene<br><br>**Triangles:**<br><500,000<br><br>**Materials:**<br>1-2 per object|Not applicable|Not applicable|

> [!NOTE]
> Transparency in materials such as glass in 3D models is not supported.

### See also
[Overview of Dynamics 365 Import Tool (Preview)](index.md)<br>
[Convert 3D models](convert-models.md)<br>
[Best practices for converting and optimizing 3D models](best-practices.md)<br>
[Use Dynamics 365 Import Tool (Preview)](import-tool.md)
