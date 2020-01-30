

# Use SideFX Houdini to turn point-clouds into optimized 3D models for use in Dynamics 365 Mixed Reality applications

This tutorial provides step-by-step instructions that will show you how to: 

- Convert a point cloud into a 3D model.

- Optimize a 3d model by reducing the polygon count so that it matches [performance targets for Dynamics 365 mixed reality applications](optimize-models#performance-targets).

- Export an optimized 3d model as a .GLB file that can be used in Dynamics 365 mixed reality applications.

- Create a processing pipeline template for quickly optimizing point-clouds in the future.

This document is created strictly for informative purposes to demonstrate how SideFX Houdini works with Microsoft Dynamics 365 mixed reality applications.  Your use of third-party applications is subject to terms between you and the third party.  The Microsoft Corporation is not affiliated with, is not a partner to, and does not endorse or sponsor SideFX or any of SideFX’s products.  There are several other [content-creation applications that can be used to prepare your 3D models](convert-models#tools-for-exporting-cad-models). 

## What is Houdini?

Houdini is a 3D procedural content creation tool.  It uses a non-destructive node-based tool system that can be used to design process pipelines and 3D content. 

## Setting up your environment

### Install SideFX Labs extension

SideFX Labs is a testing ground for tools that can be used with SideFX Houdini aimed to help you get up and running quicker with Houdini knowledge and capabilities .  Within this collection of free tools, you can find some specific ones that are useful for converting point-clouds into optimized 3D models.  You must be using Houdini 18 or later to use SideFX Labs.

SideFX provides a tutorial video that will help you install these tools that can be found here: [SideFX Labs Install](https://www.sidefx.com/tutorials/sidefx-labs-installation/)

1.	To install SideFX Labs, first navigate to the top of the window and select the plus symbol SCREEN SHOT GOES HERE and navigate to **Shelves > SideFX Labs**. Check the box to the left of SideFX Labs.

SCREEN SHOT GOES HERE
 
2.	You will now have a SideFX Labs toolbar that has one icon called **Update toolset**.  Click on this icon to launch the installer.

SCREEN SHOT GOES HERE 

3.	Click update to install the tools.  It is packaged with Houdini and does not require an internet connection to install.  If you are connected to the internet, then you can change the release to a later release.  If you want to check out the latest features, then you can uncheck the “Production Builds Only” option and you will be able to install the absolute latest builds of SideFX Labs.

SCREEN SHOT GOES HERE

You will know that your install was successful if more tools show up in the toolbar. You are now ready to use SideFX Labs tools and can continue with the tutorial.

### Setting up AliceVision for Photogrammetry

There is an existing plugin for Houdini users to leverage AliceVision for photogrammetry, follow [this tutorial from SideFX](https://www.sidefx.com/tutorials/alicevision-plugin/) to correctly install and set up AliceVision.

[AliceVision](https://alicevision.org/) is a Photogrammetric Computer Vision Framework which provides 3D Reconstruction and Camera Tracking algorithms, which can be found on GitHub. It is being developed by the post-production company called **Mikros Image**, about whom you can find more information here: [About AliceVision](https://alicevision.org/#about) – [SideFX](https://www.sidefx.com/tutorials/alicevision-plugin/)

## Importing point-clouds into SideFX Houdini

Houdini can import point-clouds of a file type .ply.  If you do not have a .ply file format, but do have a .pts file format, it is possible to manually convert your file format.

### Manually converting .pts files to .ply files.

You can open your .pts file in a file editor of your choice and add the following heading to your file to convert it from a .pts file to a .ply file.  

************************
ply
format ascii 1.0
element vertex 534993 WHY WAS THIS HIGHLIGHTED IN YELLOW?
property float x
property float y
property float z
property uchar intensity
property uchar red
property uchar green
property uchar blue
end_header
************************
(Note: the element vertex highlighted above in the header is the number that appears at the top of your .pts file.  This is the total number of points in your point cloud and should be placed in the header and removed from the file after the header.)
Below is a side by side view of what the top of your original .pts file and the top of your modified .ply files will look like before and after the heading is added.  The element vertex count is highlighted in red:

|Top of .pts file|Top of .ply file|
|---------------------------------------------------------------|------------------------------------------------------------------|
|SCREEN SHOT GOES HERE|SCREEN SHOT GOES HERE|

*The numbers on the left most of the images indicate respective line number.*

Once you have correctly modified your .pts file, save it with the file extension .ply and you will now be able to import your point-cloud into Houdini.

### Import your .ply file

1.	Open Houdini. A new scene will automatically be created.  We will be building a chain of nodes that process our point cloud into a 3D model.  These nodes will be constructed in the bottom right windowpane highlighted below.

SCREEN SHOT GOES HERE  

2.	Right click in the bottom right windowpane to open the tab menu (you can also just press TAB). In the **TAB menu**, navigate to **Import > File**.  Left click to place this node into the Geometry pane.

SCREEN SHOT GOES HERE
 
3.	Double click the center of the **File1** icon or press **I** to drill down to the file selection part of this node. Click the **File Chooser** button and choose the file you wish to import.

SCREEN SHOT GOES HERE 

4.	A file browser will pop up. Browse to the location of the file you need to import, select your .ply point-cloud file, and then click the **Accept** button. 

SCREEN SHOT GOES HERE
 
5.	You can now see your point-cloud in the viewport.  If you cannot, try zooming out with the mouse wheel until you can see the entire point-cloud.

SCREEN SHOT GOES HERE
 
## Preparing point-clouds

### Re-orienting point-clouds

Sometimes your point-cloud will import in the wrong orientation.  You can easily fix this by adding a transformation node in the node tree on the bottom right of the Houdini window.  

1.	To add a transform node, right-click inside the geometry pane to access the TAB menu and navigate to **Manipulate > Transform**.

SCREEN SHOT GOES HERE

2.	Place the “transform” node below the “file” node, left mouse click and hold the dot on the bottom of the “file” node and drag it to the dot on the top of the “transform” node to link them.  Once you have them linked, left mouse click the right side of the “transform” node.  Doing this will turn it blue and set the View window to the transform node so that you can see your model after it has been transformed. 

SCREEN SHOT GOES HERE
 
>[!TIP]
>Tip: In Houdini, you can Select the right side of each node to view the model during that stage of the process.  This is helpful is you ever need to go back and look at your 3D model in a previous state to make changes that occurred during that state.
3.	Now that you have your transform node set up properly, correct the rotation of your model.  You do this by adding values to the “Rotate” row of value in the options pane above the node pane.  Often you can replace the x value with “270” and the model will rotate to the correct position.  If this does not produce an acceptable result, try with different values.

SCREEN SHOT GOES HERE
 
4.	You should now see your point-cloud oriented correctly.  If you would like to center your point-cloud over the origin, you can add an **axis align** node after your transform node.  To place the node, hover your mouse over the Geometry pane, press tab and navigate to **Labs > Geo  Labs Axis Align**.  

SCREEN SHOT GOES HERE
 
5.	Connect the output of your **transform** node to the input of your axis align node.  Leaving the values at default will set your point-cloud on top of the origin point, an ideal place to have your 3D model.

SCREEN SHOT GOES HERE 

Next, we will clean up the point-cloud.

### Cleaning up point-clouds

If your point-cloud has stray points that you would like to remove, you can select and delete individual or groups of points.

1.	To start, change the “geometry select” method to **points** and the “select” tool to **Lasso Picking**. You can use a different method if you prefer, but for this demo we will be using these settings.

SCREEN SHOT GOES HERE 

2.	Once you have your selection set up, select the points that you wish to delete.

SCREEN SHOT GOES HERE 
 
3.	Press the **Delete** key to remove these points from your point cloud.  When you do this, a new node called “blast” will appear connected to the bottom of the last node you were operating on.

SCREEN SHOT GOES HERE 
 
4.	Continue to remove points until your point-cloud reaches a satisfactory level of cleanliness.  Each deletion will add a new “blast” node that can be viewed or removed at any time.

SCREEN SHOT GOES HERE 
 



