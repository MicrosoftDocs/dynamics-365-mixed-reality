
# Tutorial 1: Using Blender to prepare 3D models for use in Microsoft Dynamics 365 Mixed Reality applications

This tutorial provides step-by-step instructions that show you how to:

- Reduce the polygon count of a 3D model so that it matches the performance needs specific to the [performance targets for Dynamics 
365 mixed reality applications](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/optimize-models#performance-targets).

- Combine the 3D model’s multiple materials (colors) into a single texture that can be applied to the model.

- Export the optimized 3D model as a [GLB](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/#gltf-and-glb-file-formats) file that can be used in Dynamics 365 mixed reality applications.

The combination of reducing polygons and turning multiple materials into a single texture can transform a complex 3D model that 
is resource intensive, into a highly performant 3D model that performs well in mixed reality applications.

> [!NOTE]
> This document is created strictly for informative purposes to demonstrate how Blender works with Microsoft Dynamics 365 Mixed Reality 
at Work applications. Your use of third-party applications is subject to terms between you and the third party.  
The Microsoft Corporation is not affiliated with, is not a partner to, and does not endorse or sponsor Blender or any of 
Blender’s products. [There are several other content-creation applications that can be used to prepare your 3D models](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/convert-models#tools-for-exporting-cad-models).

## What is Blender?

[Blender](https://www.blender.org/) is a free and open source 3D creation suite. It supports the entirety of the 3D pipeline: modeling, rigging, animation, simulation, rendering, compositing and motion tracking, and video editing and game creation. 

If Blender is the software that you decide to use to prepare your assets, review Blender’s website and download the most current stable version for Windows. Currently this is [Blender v 2.8](https://www.blender.org/download/releases/2-80/).

## Use Blender 2.8 to prepare a 3D model for Mixed Reality

In this part of the tutorial we’ll take an OBJ and optimize it through decimation and texture baking to prepare it for use in Dynamics 365 mixed reality applications.

The overall steps we’ll cover for optimizing in Blender include:

1.	Import the model into Blender.

2.	Decimate the model.

3.	UV wrap the model.

4.	Assign materials.

5.	Bake the textures.

6.	Export the model.

### Import the model into Blender

1.	Open Blender 2.8. A new scene will automatically be created.

2.	Right-click the cube and delete it.

    SCREENSHOT GOES HERE: blender-delete-cube

3.	Go to **File > Import > Wavefront (.obj)** to import your OBJ. 

4.	In the **Import OBJ** screen:

    a. Make sure to clear the **Object** and **Group** check boxes and select the **Image Search** check box.

      SCREENSHOT GOES HERE: blender-clear-checkboxes
        
    b. Select **Import OBJ** on the right side of the screen. This will import the 3D model as one item and search in the sub folder for any materials.

      SCREENSHOT GOES HERE: blender-import-obj
      
      > [!TIP]
      > If your 3D model is extremely large or small, hard to see, and possibly off screen, you can use the middle mouse wheel to zoom the camera in or out until it’s visible.
      
      SCREENSHOT GOES HERE: blender-zoom-camera
      
      > [!TIP]
      > If your 3D model appears grey, select the **Look Dev** shading option SCREENSHOT of button goes here: blender-look-dev  to show the colors.
      
      SCREENSHOT GOES HERE: blender-look-dev-full-screen
      
      Now you can see your 3D model with the imported materials.
      
      At the bottom right of the screen, you can see your **Tris** count (number of polygons). [If this number falls in line with the target resolution](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/optimize-models#performance-targets), you can skip the decimation step and go directly to the **UV Unwrapping** section of this tutorial. If not, continue to the next section and decimate the 3d model.
      
      SCREENSHOT GOES HERE: blender-tris-count
      
### Decimate the model

To reach application-specific performance goals, we need to decimate the model. Decimation is the process of recomputing the surface polygons of the model to create a similar shape with fewer polygons. There is a reduction in visual fidelity when doing this, but also an increase in performance. The example images below shows a high fidelity model that can be used when you are viewing one or two 3D models at a time on HoloLens, and a low-quality 3D used model used when you are viewing Ten or more models at a time on HoloLens.

SCREENSHOT GOES HERE: blender-decimation

To decimate a model:

1.	Select your 3D model and go to the **Modifiers** menu SCREEN SHOT: blender-wrench-tool  on the right hand tool column.

2.	On the **Modifiers** menu, in the **Add Modifier** drop-down list, select **Decimate**.

SCREENSHOT GOES HERE: blender-add-modifier-decimate

3.	With your model selected, change the **Ratio** value to a number between 0.0-1.0. This will determine the percentage of polygons (triangles) that are removed. For example, a value of 0.5 reduces the original polygon count to 50%. You’ll see the **Tris** value in the bottom right of the Blender window decrease as you change the ratio. When the number reaches a value that matches your performance goal and looks good, select **Apply**.

SCREENSHOT GOES HERE: blender-ratio

### UV unwrapping

A good way to visualize UV unwrapping is to imagine cutting out every surface of your 3d model and placing those surfaces flat on a piece of paper. The U and V dimensions represent the vertical and horizontal axes of this piece of paper in the same way that X, Y, and Z represent the three-dimensional axes of a 3d model. The advantage of unwrapping the UVs is to allow us to paint the flattened pieces with the material colors of the 3d model. This painted paper is called a texture, and it’s later wrapped back on top of the 3d model, giving it the illusion of being made from different colored pieces, when it’s actually one item with a colorful texture wrapped around it. This process is called texture baking, which we’ll go into later. You may skip this step if your model has only one color. 

> [!TIP]
> Enter **Edit Mode** by selecting the mode dropdown in the upper left corner, or press the **Tab** key. Pressing **Tab** while already in **Edit Mode** will bring you back into **Object Mode**. 

SCREENSHOT GOES HERE: blender-object-mode

To start the process:

1.	Select the model, hover the mouse over the main menu, press **Tab** to enter **Edit Mode**, press **“a”** to select all, and then select **Smart UV Project** from the **UV** drop-down menu.

    SCREENSHOT GOES HERE: blender-UV

2.	Keep the default settings for the properties, and then select **OK**.

    SCREENSHOT GOES HERE: blender-default-settings
    
3.	Make sure that you’re in **Edit Mode** (tab), and that the entire model is still selected (a-key). You can tell the entire model is selected because it will be orange. 

4.	Select the **UV Editor** menu (or press Shift+F10).
  
    SCREENSHOT GOES HERE: blender-UV-editor
    
5.	On the **UV** tab, select **Pack Islands**.

    SCREENSHOT GOES HERE: blender-pack-islands
    
    The outlined pieces are reorganized to represent the surface of the model as efficiently as possible. After packing the islands, the UVs will look like this:
    
    SCREENSHOT GOES HERE: blender-pack-islands-after
    
6.	For our next step, we’ll need a duplicate of our mesh.  This will be the mesh that our texture gets “baked” to in a later section.
    a.	To make a copy of the 3d model:
        i.	Click the model with the left mouse button to select it
        ii.	Right-click the 3D model to open the menu
        iii.	Select “Duplicate Objects”
        iv.	Press “Space Bar”

    SCREENSHOT GOES HERE: blender-duplicate-object
    
    
