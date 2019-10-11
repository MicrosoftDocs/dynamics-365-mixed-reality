---
author: JBrentJ
description: Describes, in tutorial format, how to use Autodesk 3ds Max to generate content for use in Dynamics 365 mixed reality applications
ms.author: v-jerja
ms.date: 10/21/2019
ms.service: crm-online
ms.topic: article
title: Use Autodesk 3ds Max to generate content for use in Dynamics 365 mixed reality applications
ms.reviewer: v-brycho
---

# Use Autodesk 3ds Max to generate content for use in Dynamics 365 mixed reality applications

When preparing CAD files for mixed reality, there are numerous performance and quality roadblocks that prevent a smooth transition 
from CAD to real-time. 3ds Max is a digital content creation suite that has a unique ability to bridge parametric models and real-time 
polygon modeling. This topic demonstrates a workflow that utilizes 3ds Max’s conversion and optimization abilities to prepare 3D CAD 
models for use in mixed reality.  
 
> [!IMPORTANT]
> This document is created strictly for informative purposes to demonstrate how Autodesk 3ds Max works with Microsoft Dynamics 365 
Mixed Reality at Work applications. The Microsoft Corporation is not affiliated with, is not a partner to, and does not endorse or 
sponsor Autodesk or any of Autodesk’s products. 

## What is Autodesk 3ds Max

Autodesk 3ds Max is 3d modeling and rendering software for design visualization, games, and animation. Read more 
about [Autodesk](https://www.autodesk.com/products/3ds-max/overview). 

## Import your file into 3ds Max

1. Open a new scene in 3ds Max, and then on the **File** menu, select **Import>Import** to import your 3D model. 
 
   SCREEN SHOT GOES HERE: 3ds-max-file-import
 
2. Check the import options to ensure the scene is imported as expected. Import settings might differ depending on the type of file you 
import. You can usually keep the default values with the following exceptions:
   
    - Set **Hierarchy Mode** to **Flatten**
    
    - Se **Mesh Resolution** somewhere between -6 and -10. If your model imports sideways, re-import it with the Up axis set to Y – Up. 

   SCREEN SHOT GOES HERE: 3ds-max-import-settings   
   
## Optimize your 3D models 

If the polygon count is too high ([see Performance targets](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/optimize-models#performance-targets)), 
the model won’t perform well in mixed reality applications. You can optimize the 3D model to reduce the polygon count so the model 
performs better. To see the polygon count, first set up the viewport to show polygon statistics. 

### Show polygon statistics 
 
1. To view the number of polygons in your scene, select **+** in the upper-left corner of any viewport window to open the 
**Configure Viewports** options.  
 
   SCREEN SHOT GOES HERE: 3ds-max-plus-sign
 
   SCREEN SHOT GOES HERE: 3ds-max-configure-viewports
 
 
2. On the **Viewport Configuration** menu, go to the **Statistics** tab. In the Setup submenu, select the **Polygon Count** check box, 
and select the **Total + Selection** radial button. In the **Application** submenu, select the **Show Statistics in Active View** 
check box.  
 
   SCREEN SHOT GOES HERE: 3ds-max-viewport-settings
 
   You can now see the total poly count of your model, and the total poly count of any objects that you have selected. 
 
   SCREEN SHOT GOES HERE: 3ds-max-total-poly-count
   
### Add an Edit Poly modifier 

- Select all parts of your 3D model and apply the **Edit Poly** modifier. Adding an edit poly modifier helps eliminate shading issues that occur during the modification. 
 
   SCREEN SHOT GOES HERE: 3ds-max-edit-poly-modifier
    
### Select high poly objects

The best way to reduce the size of your model while maintaining visual fidelity is to find the objects with the highest poly count, 
and reduce them the most. Objects such as screws and grills can have thousands of polygons that are rarely seen.  

1. Go to **Select from Scene**. 
 
   SCREEN SHOT GOES HERE: 3ds-max-select-from-scene
 
2. Go to **Customize>Configure Columns**. 
 
   SCREEN SHOT GOES HERE: 3ds-max-configure-columns
 
3. Drag **Faces** next to **name** to activate the column. 
 
   SCREEN SHOT GOES HERE: 3ds-max-drag-faces
 
4. Select the **Faces** tab a few times so that your objects are now sorted from highest face count to lowest. 

   >[!TIP]
   > You can also search at the top of this menu. If your model has lots of fillets, try searching for those. Fillets use lots of polygons and can be reduced without affecting the overall fidelity of the model. 
 
5. Select the objects with the highest face counts, and then select **OK**.   
 
   SCREEN SHOT GOES HERE: 3ds-max-face-counts
 
   You now have the highest poly objects selected. For the example model, 136K of the 195K polygons exist in 6 objects. The next section in this topic shows how to reduce the poly count of these objects. 
   
   SCREEN SHOT GOES HERE: 3ds-max-selected-objects
   
### Reduce poly count 

1. Go to the **Modifier List** panel located on the right side of the viewport, and then select the **Modifier List** drop-down.  

   SCREEN SHOT GOES HERE: 3ds-max-modifier-list   
 
2. Select **ProOptimize** from the list.   

   SCREEN SHOT GOES HERE: 3ds-max-prooptimize
  
3. Select **Calculate** to unlock the **Optimization Level** value adjustments. Try different values for **Vertex %** that range from 10 - 30% until you find the highest level of reduction that still maintains a visual fidelity that meets your standards. 
 
4. Go to **Edit -> Select Invert** and add a **Pro Optimizer** to the rest of your model. Follow the same steps as you did before, but don't go as low as 10 - 30%. Reduce these other objects until you reach a polygon count that matches the recommended [Performance targets](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/optimize-models#performance-targets) for your specific use case and still provides good visual fidelity. 
 
   SCREEN SHOT GOES HERE: 3ds-max-select-invert
   
   > [!TIP]
   > You can be as granular with what you reduce as you like. If there are specific parts that need higher fidelity, select them and raise the percentage value to meet your needs. Try different techniques until you find one that works best for you. 
   
## Work with curved surfaces 

When curved surfaces are present on 3D models, they might appear faceted. You can soften the appearance of these surfaces by using **Smooth**.  
 
1. On the **Edit** menu, select **Select All** to select all 3D models in the scene.  
 
   SCREEN SHOT GOES HERE: 3ds-max-select-all
   
2. In the **Modifier List** panel, select **Smooth** from the drop-down.  

   SCREEN SHOT GOES HERE: 3ds-max-smooth 
 
3. Select the **Auto Smooth** check box, and then adjust the **Threshold** value until the faceted surfaces appear smooth.  The default threshold is 30.0 which is usually pretty good. 
 
   > [!NOTE]
   > You can also apply the **Smooth** modifier to individual 3D models if they each require a different threshold.  
 
At this point, your model may be optimized enough for use in mixed reality. If you think it will work fine in this form, you can skip to exporting your model as a GLB. If the model is still too complex and has lots of materials, go to the next section on texture baking. 
 
## Set up materials

Not all CAD materials are compatible with real-time applications, so they must be converted first. In this section, we’ll change the materials to a GLB-friendly material type called **Physical Material**. This material is very flexible and is compatible with mixed reality technology.  
 
> [!NOTE]
> If your 3D model has 10 or more materials, performance may be an issue. To fix this, skip to the Texture Baking section.  
 
To set up materials in 3ds Max: 
 
1. On the **Rendering** menu, select **Scene Converter**.   
 
   SCREEN SHOT GOES HERE: 3ds-max-scene-converter 
 
2. In the **Scene Converter** dialog box, expand the **Materials** tab, and then select **Standard Material to Physical Material**. 

   SCREEN SHOT GOES HERE: 3ds-max-standard-to-physical
   
3. Select **Convert Scene**.  
 
## Add or modify existing materials

In cases where you want fine control over materials, this section shows how to apply and change material characteristics, such as color and reflection.  
 
1. On the **Rendering** menu, select **Material Editor>Compact Material Editor**. This provides control over how the materials will look. 
 
   SCREEN SHOT GOES HERE: 3ds-max-compact-material-editor
 
 
2. The **Material Editor** window includes blank material slots that appear as grey spheres. To load a slot for inspection, select the eye dropper icon near the **Global** drop-down, and then select the 3d model to look at.  
 
   SCREEN SHOT GOES HERE: 3ds-max-material-color 
 
   The important parameters to look at are **Base Color** and **Reflections**. **Reflections** is controlled by the **Metalness** and **Roughnes**s values — the surface finish of the material.  
 
   - To apply a material to another 3D model, drag the active material ball on top of the 3D model you want to change.  
 
     SCREEN SHOT GOES HERE: 3ds-max-apply-material 
 
   - To inspect another material, either use the eyedropper again to overwrite the current material slot, or select a new slot to easily switch back and forth between materials.  
   
