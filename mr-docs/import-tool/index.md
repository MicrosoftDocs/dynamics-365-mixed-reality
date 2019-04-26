---
author: BryceHo
description: Overview of converting and optimizing 3D models to use with Dynamics 365 Import Tool (Preview).  
ms.author: BryceHo
ms.date: 04/24/2019
ms.service: crm-online
ms.topic: overview
title: Overview of converting and optimizing 3D models to use with Dynamics 365 Import Tool (Preview).
ms.reviewer: v-brycho
---

# Overview of Dynamics 365 Import Tool (Preview)

If you’re using Microsoft Dynamics 365 mixed-reality applications, you might want to import your own 3D models ([CAD](https://en.wikipedia.org/wiki/Computer-aided_design) models) into the applications. This guide shows you how to prepare your 3D models for use with Dynamics 365 mixed-reality applications using a combination of third-party tools and Dynamics 365 Import Tool (Preview).

## glTF and GLB file formats
All geometry in Dynamics 365 mixed-reality applications uses the Khronos Group glTF file format. This royalty-free specification minimizes both the size of 3D models and the run-time processing needed to unpack and use those models. The GLB format is the binary version of .glTF version 2.0, which can include textures.

<!--note from editor: I removed the TM bug from "glTF" because we typicvally don't include them.  Guidance from CELA website: "Bug and footnote third party trademarks ONLY when Microsoft is contractually obligated to do so." Do you know if this is a case where MS is obligated by contract?     -->

> [!TIP] 
> The Khronos Group provides a robust overview of best practices: [Art Pipeline for glTF](https://aka.ms/glTFbestpractices).

## Parametric geometry vs. polygonal geometry

Modeling tools in most CAD applications use sets of adjustable mathematical parameters to define parametric solids. Parametric solids and surfaces provide highly accurate detail that can be used to carry out engineering simulations and manufacturing processes. glTF and real-time rendering applications require models to be represented as a triangulated polygon surface.

> [!div class="mx-imgBorder"]
> ![Parametric vs. polygonal geometry](media/compare-geometry.PNG "Parametric vs. polygonal geometry") 

*Model visualized in Autodesk Inventor and Microsoft 3D Viewer*

A.	Parametric 3D model ready for simulation and manufacturing<br>
B.	Polygonal surface 3D model ready for real-time rendering

## Overall process for preparing 3D models

Preparing CAD content for Dynamics 365 mixed-reality applications involves three main steps: 

1.	**Convert 3D models** from their original geometric definition into one that supports real-time rasterization. This converts the models from parametric geometry into polygonal geometry. 

2.	**Optimize the converted 3D models** to ensure the best possible performance in real-time applications.

3.	**Use the Import Tool** to prepare the models for Dynamics 365 mixed-reality applications. 

The following illustration shows a more detailed view of this process.

> [!div class="mx-imgBorder"]
> ![Overall flow](media/overall-flow.PNG "Overall flow") 

**A.**	Create 3D models using the CAD software of your choice.<br>
**B.**	Convert CAD files to one of these file formats: FBX, OBJ, JT, STP, or SKP.<br>
**C.**	Optimize your 3D model and convert it to GLB.<br>
**D.**	Use the Import Tool to prepare content for Microsoft HoloLens, immersive headsets, or mobile devices.<br>
**E.**	3D models are ready to be imported into Dynamics 365 mixed-reality applications.

### See also
[Convert 3D models](convert-models.md)<br>
[Optimize 3D models](optimize-models.md)<br>
[Best practices for converting and optimizing 3D models](best-practices.md)<br>
[Use the Import Tool](import-tool.md)



