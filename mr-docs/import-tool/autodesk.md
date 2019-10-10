# Use Autodesk 3ds Max to generate content for use in Microsoft Dynamics 365 mixed reality applications

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
   

 
