

# Use SideFx Houdini to prepare 3D models for use in Dynamics 365 mixed reality applications

This tutorial provides step-by-step instructions that will show you how to:

- Optimize a 3D model by reducing the polygon count so that it matches [performance targets for Dynamics 365 mixed 
reality applications](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/optimize-models#performance-targets).  

- Add the correct material to a 3D model. 

- Export an optimized 3d model as a .GLB file that can be used in Dynamics 365 mixed reality applications. 

- Create a processing pipeline template for quickly optimizing other 3D models in the future. 

>[!IMPORTANT]
> This document is created strictly for informative purposes to demonstrate how SideFX Houdini works with Microsoft 
Dynamics 365 Mixed Reality at Work applications.  Your use of third-party applications is subject to terms between you 
and the third party.  The Microsoft Corporation is not affiliated with, is not a partner to, and does not endorse or sponsor 
SideFX or any of SideFX’s products.  There are several other content-creation applications that can be used to prepare your 3D models.

## What is Houdini? 

Houdini is a 3D procedural content creation tool. It has a non-destructive node-based tool system that can be used to design process pipelines. 

## Import a 3D model into Houdini

1. Open Houdini 17.5. 

   SCREEN SHOT GOES HERE: houdini-new scene

   A new scene will automatically be created.   
 
2. Right-click in the bottom right window pane to open the **TAB** menu (or press TAB).    

3. In the **TAB** menu, go to **Import > File**. Select to place this in the Geometry pane. 

   SCREEN SHOT GOES HERE: houdini-import-file
 
4. Double-click the center of the “file1” icon or press ‘I’ to drill down to the file selection part of this node. Select the “open floating file chooser” button and choose the file you want to import. 

   SCREEN SHOT GOES HERE: houdini-file-chooser
 
5. A file browser will pop up. Browse to the location of the file you need to import, select the file requiring reduction, and then select **Accept**.  

   SCREEN SHOT GOES HERE: houdini-select-file 
 
   You can now see your model in the viewport. 
   
   SCREEN SHOT GOES HERE: houdini-viewport
   
   
