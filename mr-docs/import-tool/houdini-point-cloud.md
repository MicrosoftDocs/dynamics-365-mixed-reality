

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



