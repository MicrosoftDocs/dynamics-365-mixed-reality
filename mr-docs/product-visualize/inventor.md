---
author: sbmjais
description: Describes, in tutorial format, how to use Autodesk Inventor to prepare 3D models for use in Dynamics 365 mixed-reality apps
ms.author: shjais
ms.date: 08/13/2020
ms.topic: article
title: Prepare Autodesk Inventor 3D models for use in mixed-reality applications
manager: shujoshi
---

# Prepare Autodesk Inventor 3D models for use in mixed-reality applications

This tutorial shows how to prepare Autodesk Inventor files for use in Dynamics 365 mixed-reality apps.  

> [!IMPORTANT]
> This document is created strictly for informative purposes to demonstrate how Autodesk Inventor works with Dynamics 365 mixed-reality apps. Your use of third-party applications is subject to terms between you and the third party. Microsoft Corporation is not affiliated with, is not a partner to, and does not endorse or sponsor Autodesk or any of Autodesk's products. There are [other content-creation apps](convert-models.md#tools-for-exporting-cad-models) you can use to prepare your 3D models.

## What is Autodesk Inventor?

Autodesk Inventor is professional-grade 3D CAD software for product design and engineering. For more information, [see Autodesk Inventor](https://www.autodesk.com/products/inventor/overview).

## Optimize 3D models for mixed reality

The first step is to remove any unneeded detail from the 3D model. This vastly improves performance and increases the visual quality of the 3D model. Inventor has a tool called **Shrinkwrap** that can assist by removing fillets, chamfers, small parts, holes, and more.

1.	On the **Assemble** tab in Inventor, select **Shrinkwrap**.

    ![Shrinkwrap.](media/inventor-shrinkwrap.PNG "Shrinkwrap")

    From here, there are several optimization options you can choose to help increase the performance of your model in Dynamics 365 mixed-reality apps.

2.	Select the **Remove parts by size** check box, select the mouse arrow, and then select the largest object you're willing to remove, such as a bolt. This will remove all objects (nuts, bolts, washers) that are smaller than the object you selected.

    ![Remove parts by size.](media/inventor-remove-parts.PNG "Remove parts by size")

3.	If there are specific items such as grates or cooling fins that are extremely complex and you don't need to see them, you can use the **Select to Exclude** option to remove them piece by piece.

    ![Select to Exclude option.](media/inventor-select-to-exclude.PNG "Select to Exclude option")

4.	On the **Features** tab, you'll see options to remove some or all features such as holes, fillets, pockets, and chamfers. This works the same as removing parts by size, but for features instead of entire parts. Experiment with these features to gain additional optimizations for your model. The results can be significant.

    ![Features tab.](media/inventor-features-tab.PNG "Features tab")

5.	On the **Create** tab, do the following:

    a.	Choose a part name for the export.

    b.	Use the **Standard.ipt** template.

    c.	Set the new file location.

    d.	Under **Style**, select **Single Composite**.

    e.	Select the **Fill all internal voids** check box.

    f.	Select the **Remove internal parts** check box.

    g.	Select the **Use color override from source component** check box.

    h.	Select **OK**.

      ![Features tab settings.](media/inventor-features-tab-settings.PNG "Features tab settings")

6.	Save your file.

## Export the 3D model

Next, you need to export the model to a usable format that can be read by mixed-reality apps. You need to adjust settings so the lowest-density model is exported.

1.	In the **Save as type** box, select **OBJ files (*.obj)**.

2.	Select the **Options** button.

    ![Options button.](media/inventor-options-button.PNG "Options button")

    This is what the OBJ export settings look like in Inventor:

    ![Save As options.](media/inventor-save-as-options.PNG "Save As options")

    We recommend using the **Brep** ("boundary representation") setting, which produces the lowest poly output for Inventor files. If your model isn't overly complex and you want a higher level of detail, you can use the **Low** setting (see [Performance targets](optimize-models.md#performance-targets)).

## Convert your OBJ file to a GLB file

Dynamics 365 mixed-reality apps use the GLB format for 3D models. You can convert your OBJ file to a GLB file by using a digital content creation (DCC) platform to convert your 3D models into GLB files. Using these software platforms is a manual process, but it gives you more opportunities for optimization. To assist with this process, see the following tutorials:

  - [Blender](blender.md)
  - [Autodesk 3ds Max](3ds-max.md)
  - [SideFX Houdini](houdini.md) 
  - [Agisoft Metashape](agisoft-metashape.md)
  - [Inventor](inventor.md)
  - [ReCap Photo](autodesk-recap-photo.md) 
  - [Dassault Systèmes SOLIDWORKS](solidworks.md)


## View the 3D model in mixed reality

After preparing the 3D model, you can learn more about using the following Dynamics 365 apps to view your 3D model in mixed reality:

[Dynamics 365 Product Visualize](../product-visualize/index.md)<br> 
[Dynamics 365 Guides](../guides/index.md)

### More information

Several screenshots in this document were taken from the Autodesk Inventor software program to provide clear instructions on how to use Autodesk's software.  [Read more about Autodesk Inventor](https://aka.ms/Autodesk_inventor).

Microsoft Corporation is not responsible for, and expressly disclaims all liability for damages of any kind arising out of the use of Autodesk Inventor, or reliance on these instructions. This document is created only to provide general information to our customers and does not take into consideration any individualized business plans or specifications.

The use in this document of trademarked names and images is strictly for informative and descriptive purposes, and no commercial claim to their use, or suggestion of sponsorship or endorsement, is made by Microsoft.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
