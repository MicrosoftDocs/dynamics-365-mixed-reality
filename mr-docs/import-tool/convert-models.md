---
author: JBrentJ
description: Everything you need to know about converting 3D models to use with Dynamics 365 Import Tool (Preview)
ms.author: v-jerja
ms.date: 10/29/2019
ms.service: crm-online
ms.topic: article
title: Convert your 3D (CAD) models to use with Dynamics 365 Import Tool (Preview)
ms.reviewer: v-brycho
---

# Convert your 3D (CAD) models

To use your 3D models with [!include[pn-dyn-365](../includes/pn-dyn-365.md)] mixed-reality applications, you need to convert them to a file format that supports real-time rasterization. The type of file you convert to depends on the option you choose in the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)].

![Convert flow highlighted](media/convert-flow.png "Convert flow highlighted") 


## Options and file types for Dynamics 365 Import Tool (Preview) 

The [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] provides two options for preparing your 3D models: 

![Import Tool options](media/import-tool-options.PNG "Import Tool options") 

The following table describes the two options and the file formats supported for each.


|Option|Description|Supported file formats|
|------------|-----------------------------------------------------------------|-----------------------------|
|Import using this PC|Use this option if you want to import self-authored models without any optimization.|GLB, GLTF, FBX, OBJ, STL, PLY |
|Send model to [!include[cc-microsoft](../includes/cc-microsoft.md)]|Use this option if you need Microsoft’s assistance optimizing and converting your 3D model. [!include[cc-microsoft](../includes/cc-microsoft.md)] uses a combination of automation and manual steps to prepare the files. |FBX, OBJ, JT, STP, and SKP|

## Tools for exporting CAD models

CAD models can be exported directly to glTF format or into intermediate formats that can be subsequently processed into glTF files. If your content-creation application does not have a glTF exporter, we recommend exporting to [FBX](https://aka.ms/FBXfileformat), [OBJ](https://en.wikipedia.org/wiki/Wavefront_.obj_file), [STL](https://en.wikipedia.org/wiki/STL_(file_format)), or [PLY](https://en.wikipedia.org/wiki/PLY_(file_format)), if available. If these formats are not available, there are third-party applications that can import many different file formats and export them as one of these supported file formats. 

Your use of third-party applications is subject to terms between you and the third party. [!include[cc-microsoft](../includes/cc-microsoft.md)] does not endorse any particular third-party application and assumes no responsibility or liability for any third-party application you elect to use.

|Content-creation package|Description|
|-----------------------------------------------|---------------------------------------------------------------|
[Blender.org Blender](https://aka.ms/Blender_2.8)|Native import/export for Blender 2.8 or later|
[Autodesk 3DS Max](https://aka.ms/BabylonJS_Max2Babylon_Installation)|Babylon.JS plug-in for Max 2015 or later|
[Autodesk Maya](https://aka.ms/BabylonJS_Maya2Babylon_Installation)|Babylon.JS plug-in for Maya 2018 or later|
[Trimble SketchUp](https://aka.ms/SketchUp_glTF_Export)|Separate extensions for [import](https://aka.ms/Sketchupimport) and [export](https://aka.ms/sketchupexport)|
|[Allegorithmic Substance Painter](https://aka.ms/SubstancePainter_glTF_Exporter)|Native exporter|
|[SideFX Houdini](https://aka.ms/Houdini_glTF_Exporter)|Native import/export|
|[Maxon Cinema 4D](https://www.maxon.net/products/cinema-4d/overview/)|Native export plug-in|

In situations where a CAD application doesn’t have an export option for FBX, OBJ, GLB, PLY, STL, or glTF, you can export an intermediate file, such as [JT](https://aka.ms/Jtfileformat) or [STEP](https://aka.ms/STEPfileformat), and then process that file to create a glTF file. 

### See also
[Overview of Dynamics 365 Import Tool (Preview)](index.md)<br>
[Optimize 3D models](optimize-models.md)<br>
[Best practices for converting and optimizing models](best-practices.md)<br>
[Use Dynamics 365 Import Tool (Preview)](import-tool.md)






