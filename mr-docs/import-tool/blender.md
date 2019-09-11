
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
      
