---
author: BryceHo
description: Tutorial that shows how to use Unreal Datasmith, Blender, and the Dynamics 365 Import Tool (Preview) to prepare 3D models for Dynamics 365 mixed reality applications.
ms.author: BryceHo
ms.date: 04/18/2019
ms.service: crm-online
ms.topic: article
title: Use Unreal Datasmith, Blender, and the Dynamics 365 Import Tool (Preview) to prepare 3D models for Dynamics 365 mixed reality applications
ms.reviewer: v-brycho
---

# Tutorial 1: Unreal Datasmith, Blender, and Dynamics 365 Import Tool

This tutorial provides step-by-step instructions that show you how to:

- Convert (transcode) a CAD 3D model into a polygonal 3D model.

- Decimate the polygonal 3D model so that it has polygon counts that match the performance needs specific to the targeted Dynamics 365 mixed reality application.

- Combine the 3D model materials (colors) into a texture that can be baked into the model. This step eliminates the multitude of draw calls necessary to render individual materials.

- Export the optimized 3D model as a glTF/GLB file that can be used in Dynamics 365 mixed reality applications.

The combination of transcoding, decimation, and texture baking converts a CAD file into a highly performant polygonal 3D model that can be used in Dynamics 365 mixed reality applications. 

In this tutorial, we’ll show you how to use:

1.	[Epic Games Unreal Engine Datasmith](https://aka.ms/UnrealDatasmithOverview) to convert the 3D model to an OBJ file.

2.	[Blender 2.8 Beta](https://aka.ms/blender2.8) to optimize and convert the OBJ file to a GLB file.

3.	[The Dynamics 365 Import tool](import-tool.md) to prepare the model for HoloLens.

## What is Datasmith?

Datasmith is a tool inside the Unreal Engine that converts native CAD 3D models into exportable OBJ and FBX 3D models. 
At the end of the Datasmith part of the tutorial, you’ll find links to additional tutorials from Unreal that can assist you in more advanced optimization techniques and how to fix issues you may encounter when importing your CAD 3D models into Datasmith.

## What is Blender?

Blender is a content creation platform that optimizes models by decimating the polygon count and baking materials into textures. In the Blender part of the tutorial, we’ll take the OBJ file that was converted from native CAD format with Datasmith, optimize it through decimation and texture baking, and finally convert it to a GLB file to meet the requirements for Dynamics 365 mixed reality applications.

## Convert the CAD model with Datasmith

In this part of the tutorial, we’ll convert a native CAD file into an OBJ file.

Here are the overall steps:

1.	Set up a new project and scene.

2.	Import the model into the project.

3.	Reorient the model (if needed).

4.	Export the model as an OBJ file.

Datasmith can import multiple file formats, including several native CAD formats. For a list of all supported formats, [see supported file formats for Datasmith](https://aka.ms/UnrealDatasmithsoftware).

### Set up a new project and scene

1.	Select **Launch Unreal Engine** from the Epic Games Welcome page.

    ![Launch Unreal Engine](media/splash.PNG "Launch Unreal Engine")
    
 2.	Select **New Project**, and then select the **Blank** button.
 
    ![New Project](media/new-project.PNG "New Project")
    
    This will open a blank scene that we’ll replace with an empty level.
    
    ![Blank scene](media/blank-scene.PNG "Blank scene") (MISSING THIS SCREEN SHOT)
    
 3.	On the **File** menu, select **New Level**.
    
    ![New level](media/new-level.PNG "New level")
    
 4. Select **Empty Level**.
    
    ![Empty level](media/empty-level.PNG "Empty level")
    
### Import the model into the project

1.	In the **Import Datasmith** drop-down list at the top of the screen, select **Import CAD**.
    
    ![Import CAD](media/import-cad.PNG "Import CAD")
    
2.	Import your model using one of the [approved file formats](https://aka.ms/UnrealDatasmithsoftware). 

    > [!NOTE]
    > Using the beta file formats (.dwg, .wire, .gltf, and Autodesk Revit plug-in) may give you unwanted results.

    file-formats SCREENSHOT GOES HERE
    

3.	In the **Datasmith Import Options** screen, use the default settings.

    import-options SCREENSHOT GOES HERE
    
### Reorient the model (if needed)

Unreal uses Z as the up direction for its coordinates.

If your model is imported with the wrong vertices up:

1.	Select the parent object for the 3D model in the World Outliner.

2.	Use the **Transform** tab to change the rotation. 

    transform-tab SCREENSHOT GOES HERE
    
    Changing the X rotation on the **Transform** tab to -90 usually fixes this problem.
    
### Export the model as an OBJ file

1.	On the **File** menu, select **Export All**.

    export-all SCREENSHOT GOES HERE

2.	Create a new folder, enter a file name, in the **Save as type** list, select **Object File (.obj)**, and then select **Save**.

    save-as-type SCREENSHOT GOES HERE

3.	When prompted whether you’d like to export the materials as images, select **Yes**. This will allow Blender to assign the correct materials when you import it.

    export-materials-as-images SCREENSHOT GOES HERE
    
### More info on Datasmith

Use these links to learn about more advanced optimizations you can do with Datasmith:

- [Mesh cleanup of CAD 3D model](https://aka.ms/ModifyStaticMesh)

- [Defeaturing a CAD 3D model](https://aka.ms/DatasmithDefeaturing)

- [Removing fully occluded meshes](https://aka.ms/DatasmithJacketing)

- [Considerations when importing native CAD 3D models with Datasmith](https://aka.ms/DatasmithGuideCAD)

## Use Blender to optimize the model

In this part of the tutorial we’ll take the OBJ file that was converted from native CAD format with Datasmith and optimize it through decimation and texture baking to meet the requirements for Dynamics 365 mixed reality applications.

The overall steps for optimizing with Blender include:

1.	Import the model into Blender.

2.	Decimate the model.

3.	UV wrap the model.

4.	Assign materials.

5.	Bake the textures.

6.	Export the model.

### Import the model into Blender

1.	Open Blender 2.8. A new scene will automatically be created.

2.	Right-click the cube and delete it.

    delete-cube SCREENSHOT GOES HERE
    
3.	Go to **File** > **Import** > **Wavefront (.obj)** to import the OBJ file that you exported from Datasmith.

    import-obj SCREENSHOT GOES HERE
    
4. In the **Import** screen:
   
   a. Make sure to clear the **Object** and **Group** check boxes and select the **Image search** check box.
   
      check-boxes SCREENSHOT GOES HERE
      
   b. Select **Import OBJ** on the right side of the screen. This will import the 3D model as one item and search in the sub folder for the materials that we exported in Datasmith.
   
      import-object-2 SCREEN SHOT GOES HERE
      
      > [!TIP]
      > If your 3D model is extremely large and hard to see, you can use the middle mouse wheel to scroll until it’s visible.
      
      large-model SCREENSHOT GOES HERE
      
      > [!TIP]
      > If your 3D model appears grey, select the **Look Dev** shading option to show the colors.
      
      look-dev-shading SCREENSHOT GOES HERE      
      
      Now you can see your 3D model with the imported materials:
      
      At the bottom right of the screen, you can see your Tris count (percentage of polygons removed). [If this number falls in line with your object's desired resolution](optimize-models), you can skip the decimation step and go directly to the UV Unwrapping section. If not, continue to the next section to decimate the 3D model. 
      
      tris-count SCREENSHOT GOES HERE
      
### Decimate the model

To reach application-specific goals, we need to decimate the model.  Decimation is the process of recomputing the surface polygons of the model to create a similar shape with less polygons. There is a reduction in visual fidelity when doing this, but also an increase in performance. The example images below show the difference between a high-quality model used for low scene complexity on HoloLens, and a low-quality model used for high scene complexity.

|High-poly 3D model|Low poly 3D model|
|---------------------------------------------------------------------|----------------------------------------------------------------|
|52000-triangles Screenshot goes here|9000-triangles Screenshot goes here|
|52,000 trialngs|9000 triangles|

To decimate a model:

1.	On the **Modifiers** menu, in the **Add Modifier** drop-down list, select **Decimate**.

    decimate-model SCREENSHOT GOES HERE
    
2.	With your model selected, change the **Ratio** value to a number between 0.0-1.0. This will determine the percentage of polygons (Tris) that are removed. For example, a value of 0.5 reduces the original polygon count to 50%. You’ll see the **Tris** value in the bottom right decrease as you change the ratio. 

3.	When the number reaches a value that falls in line with the Dynamics 365 mixed reality application requirements, select **Apply**.

### UV unwrapping

A good way to visualize UV unwrapping, is to imagine cutting out every surface of your 3D model and placing those surfaces flat on a piece of paper. The U and V represent the vertical and horizontal axes of this piece of paper in the same way that X, Y, Z represent the three-dimensional axes of the 3D model. The advantage of unwrapping the UV is it allows us to paint the flattened pieces with the material colors of the 3D model. This painted paper is called a texture, and it’s later wrapped back on top of the 3D model, giving it the illusion of being made of different colored pieces, when it’s actually one item with a colorful texture wrapped around it. This process is called texture baking, which we’ll go into later.

To start the process:

1.	Select the model, hover the mouse over the main menu, press Tab to enter Edit mode, press “a” to select all, and then select **Smart UV Project** from the **UV** drop-down menu.

    uv-dropdown SCREEN SHOT GOES HERE
    
2.	Keep the default settings for the properties, and then select **OK**.

    uv-settings SCREEN SHOT GOES HERE
    
3.	Make sure that you’re in Edit mode, and that the entire model is still selected (press Tab to enter/exit Edit mode and then press “a” to select all). You can tell that the entire model is selected because it will be orange. 

4.	Select the **UV Editor** menu (or press Shift+F10).

    uv-editor-menu SCREEN SHOT GOES HERE
    
5.	On the **UV** tab, select **Pack Islands**.

    pack-islands SCREEN SHOT GOES HERE
    
    The outlined pieces are reorganized to represent the surface of the model as efficiently as possible. After packing the islands, it will look like this:
    
    pack-islands-2 SCREEN SHOT GOES HERE
    
6.	To bake the texture that we’ll create later, we need a duplicate of the 3D model that only has one material on it. To make a copy of the 3D model, under **Scene Collection**, select the model by selecting the orange triangle icon to the left of the model name, press Shift+D, and then press Spacebar. This will place a duplicate at the exact location of the original object.

    orange-triangle SCREEN SHOT GOES HERE
    
    > [!TIP]
    > If you don’t want to use keyboard shortcuts, click the model with the left mouse button to select it, right-click the model to open the menu, select **Duplicate Objects**, and then press Spacebar.
    
    duplicate-objects SCREEN SHOT GOES HERE
    
### Prepare materials for texture baking

1.	Select the second model, and then go to the materials panel by selecting the **Materials** tab in the menu on the bottom right.

    materials-menu SCREEN SHOT GOES HERE
    

2.	Delete all the materials for the duplicate 3D model by selecting the minus sign to the right of the materials, or if you have a lot of materials, you can use a Python command to delete them all at once:
    
    a.	Open the Python Console (accessible through the icon at the bottom left of the screen or by pressing Shift+F4).
    
        python-console SCREEN SHOT GOES HERE
    
    b.	Use the following Python command to delete all the materials at once:
Bpy.context.active_object.data.materials.clear()

        python-command SCREEN SHOT GOES HERE

3.	To hide the original 3D model and show just the duplicate, select the eye to the right of its name. Notice that there are no materials on the duplicate. 

    hide-original SCREEN SHOT GOES HERE, MISSING SCREEN SHOT
    
4.	Select the plus sign to add a new material to the duplicate.

    plus-sign SCREEN SHOT GOES HERE
    
5.	Select **New** to add a new material to the material slot.

    new-material SCREEN SHOT GOES HERE
    
6.	Hover your mouse over the viewport, press Tab to enter Edit mode, press "a" to select all, and then select **Assign** from the **Materials** tab material-tab-button SCREEEN SHOT GOES HERE.

    assign-button SCREEN SHOT GOES HERE

7.	Select the icon to the left of **Object Mode** to go to the **Image Editor**.

    image-editor SCREEN SHOT GOES HERE
    
8.	Create a new image (select **Add** > **Image** > **New**) that’s 1024 x 1024.

    create-new-image SCREEN SHOT GOES HERE
    
9.	Save the new image as **My_Texture** or similar name that’s easy to remember. Don’t change any other options.

    my-texture SCREEN SHOT GOES HERE

10.	Select the icon to the left of **View** to go to the **Shader Editor**. 

    shader-editor SCREEN SHOT GOES HERE
    
11.	With your original 3D model selected, select **Add** > **Texture** > **Image Texture**. Left click to place the image texture node in the window.

    add-texture SCREEN SHOT GOES HERE
    

12.	Drag the yellow node link (the yellow dot) labeled **Color** in the image texture window to the **Base Color** yellow node on the **Principled BSDF** node to connect it.   

    connect-yellow-node SCREEN SHOT GOES HERE
    
13.	In the drop-down menu on the image texture node, find the image you just created and select it.  

    select-image SCREEN SHOT GOES HERE
    
14.	Select the 3D viewport icon at the top left to go to the 3D viewport menu.

    3D-viewport-icon SCREEN SHOT GOES HERE
    





      



### See also
[Overview of Dynamics 365 Import Tool (Preview)](index.md)<br>
[Convert 3D models](convert-models.md)<br>
[Optimize 3D models](optimize-models.md)<br>
[Best practices for converting and optimizing 3D models](best-practices.md)<br>
[Use the Import Tool](import-tool.md)
