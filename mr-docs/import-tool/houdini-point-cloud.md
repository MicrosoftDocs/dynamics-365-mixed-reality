

# Use SideFX Houdini to turn point clouds into optimized 3D models for use in Dynamics 365 Mixed Reality applications

This tutorial provides step-by-step instructions that show you how to: 

- Convert a point cloud into a 3D model. 

- Optimize a 3D model by reducing the polygon count so that it matches [performance targets for Dynamics 365 mixed reality applications](optimize-models#performance-targets).

- Export an optimized 3D model as a .GLB file that can be used in Dynamics 365 mixed reality applications.

- Create a processing pipeline template so you can quickly optimize point clouds in the future.

This document is created strictly for information purposes to demonstrate how SideFX Houdini works with Microsoft Dynamics 365 mixed reality applications. Your use of third-party applications is subject to terms between you and the third party. Microsoft Corporation is not affiliated with, is not a partner to, and does not endorse or sponsor SideFX or any of SideFX’s products. There are several other [content-creation applications that you can use to prepare your 3D models](convert-models#tools-for-exporting-cad-models). 

## What is Houdini?

Houdini is a 3D procedural content creation tool. It uses a non-destructive node-based tool system that can be used to design process pipelines and 3D content. 

## Set up your environment

To set up your environment, you need to:

- Install SideFX Labs extension

- Set up AliceVision for Photogrammetry

### Install SideFX Labs extension

SideFX Labs is a testing ground for tools that you can use with SideFX Houdini to help you get up and running quicker with Houdini. This collection of free tools includes tools that are useful for converting point clouds into optimized 3D models. You must use Houdini 18 or later to use SideFX Labs.

SideFX provides a [tutorial video](https://www.sidefx.com/tutorials/sidefx-labs-installation/) that helps you install these tools.

1. To install SideFX Labs, select the plus sign at the top of the screen ![Plus sign](media/houdini-66-plus-sign.png "Plus sign"), select **Shelves**, and then select the **SideFX Labs** check box.

    ![SideFX Labs check box](media/houdini-1-sidefx-check-box.PNG "SideFX Labs check box")
 
2. In the toolbar that appears near the top of the screen, select the **Update Toolset** button to launch the installer.

    ![Update toolset icon](media/houdini-2-update-toolset-icon.PNG "Update toolset icon")

3. Select **Update** to install the tools. 

    ![Update button](media/houdini-3-update-button.PNG "Update button")

    >[!NOTE]
    > SideFX is packaged with Houdini so you don't need an internet connection to install it. If you're connected to the internet, you can update the release later. If you want to install the latest build of SideFX Labs, clear the **Production Builds Only** option.

If the installation is successful, you'll see more tools on the toolbar, and can continue with this tutorial.

### Set up AliceVision for photogrammetry

[AliceVision](https://alicevision.org/) is a photogrammetric computer vision framework developed by Mikros Image that provides 3D reconstruction and camera-tracking algorithms. Learn more [about AliceVision](https://alicevision.org/#about) and the [AliceVision plug-in](https://www.sidefx.com/tutorials/alicevision-plugin/).

To install and setup up the AliceVision plug-in for Houdini, [see the SideFX tutorial](https://www.sidefx.com/tutorials/alicevision-plugin/).

## Import point clouds into SideFX Houdini

Houdini can import point cloud files in the .PLY file format. If your file is in a .PTS file format, you can manually convert it to the .PLY format.

### Convert .PTS files to .PLY

1.  Open your .PTS file in the file editor of your choice, and then add the following header: 

    ************************
    ply<br>
    format ascii 1.0<br>
    element vertex 534993<br>
    property float x<br>
    property float y<br>
    property float z<br>
    property uchar intensity<br>
    property uchar red<br>
    property uchar green<br>
    property uchar blue<br>
    end_header<br>
    ************************

2. In the header, replace the **534993** value next to **element vertex** with the value that appears at the top of your .PTS file here:

   ![Selected number at top of .PTS file](media/houdini-4-pts-file.PNG "Selected number at top of .PTS file")

   This value is the total number of points in your point cloud. 

3. Remove the original value after the header from your file. The following table shows a side-by-side comparison of the files before and after making the modifications. The **element vertex** count is highlighted in red:

   |Top of .PTS file|Top of .PLY file|
   |---------------------------------------------------------------|------------------------------------------------------------------|
   |![Selected number at top of .PTS file](media/houdini-4-pts-file.PNG "Selected number at top of .PTS file")|![Selected number at top of .PLY file](media/houdini-5-ply-file.PNG "Selected number at top of .PLY file")|

4. Save the file with a .PLY extension.

### Import the .PLY file

1.	Open Houdini. A new scene is automatically created. In this procedure, we'll build a chain of nodes to process the point cloud into a 3D model. These nodes will be constructed in the bottom-right window pane.

    ![Node area of window](media/houdini-6-node-area.PNG "Node area of window")

2.	Right-click the bottom-right window pane (or press TAB) to open the **TAB menu**.

3.  On the **TAB Menu**, select **Import > File**, and then click the **Geometry** pane to place the node.

    ![Import File command](media/houdini-7-import-file.PNG "Import File command")
 
3.	Double-click the center of the **file1** icon (or press **I**) to drill down to the file selection part of this node, select the **File Chooser** button, and then choose the file you want to import.

    ![File Chooser button](media/houdini-8-file-chooser.PNG "File Chooser button")

4.	In the file browser that pops up, browse to the location of the file you want to import, select the .PLY point-cloud file, and then select **Accept**. 

    ![Accept button](media/houdini-9-accept-button.PNG "Accept button")
 
    Now you can see the point cloud in the viewport. If you can't see it, try zooming out with the mouse wheel until you can see the entire point-cloud.

    ![Point cloud displayed](media/houdini-10-point-cloud-displayed.PNG "Point cloud displayed")
 
## Prepare the point cloud

### Re-orient the point cloud

Sometimes when you import a point cloud, it will have the wrong orientation. You can fix this by adding a transform node to the node tree.  

1.	To add a transform node, right-click inside the **Geometry** pane to open the **TAB Menu**, and then select **Manipulate > Transform**.

    ![Manipulat > Transform command](media/houdini-11-manipulate-transform.PNG "Manipulate > Transform command")

2.	To link the **transform1** node and the **file1** node, drag the dot on the bottom of the **file1** node to the dot on the top of the **transform1** node. Then click the right side of the **transform1** node. Doing this will turn it blue and set the **View** window to the **transform1** node so you can see your model after it has been re-oriented. 

    ![Transform node](media/houdini-12-transform-node.PNG "Transform node")
 
    >[!TIP]
    >In Houdini, you can select the right side of each node to view the model during that stage of the process. This is helpful if you ever need to go back and look at your 3D model in a previous state and make changes that occurred during that state.
    
3.	To correct the rotation of your model, in the options pane above the node pane, add values to the **Rotate** row. You can often replace the **x** value with **270** to rotate the model to the correct position. If this doesn't work, try different values.

    ![Rotation value](media/houdini-13-rotation-value.PNG "Rotation value")
 
4.	To center your the point cloud over the origin, add an axis align node after the transform node. To place the node, hover your mouse over the **Geometry** pane, press Tab, and then select **Labs** > **Geo** > **Labs Axis Align**.  

    ![Labs > Geo > Labs Axis Align command](media/houdini-14-labs-geo-axis-align.PNG "Labs > Geo > Labs Axis Align command")
 
5.	Connect the output of your **transform1** node to the input of your **axis_align1** node. Leave the default values to set your point cloud on top of the origin point (an ideal place).

    ![Nodes connected](media/houdini-15-nodes-connected.PNG "Nodes connected")

### Clean up the point cloud to remove stray points

If your point cloud has stray points that you want to remove, you can select and delete individual points or groups of points.

1. To start, change the **Geometry select** method to **points** and the **Select** tool to **Lasso Picking**. 

   >[!NOTE]
   >You can use a different method if you prefer.

   ![Points and Lasso Picking selected](media/houdini-16-points-lasso-picking.PNG "Points and Lasso Picking selected")

2. Select the points that you want to delete.

    ![Selected points to delete](media/houdini-17-selected-points.PNG "Selected points to delete")
 
3. Press the **Delete** key. When you do this, a new **blast1** node appears connected to the bottom of the last node you were working with.

    ![Blast node](media/houdini-18-blast-node.PNG "Blast node")
 
4. Continue removing points until you're satisfied with the results. Each deletion adds a new **blast** node that you can view or remove at any time.

    ![Multiple blast nodes](media/houdini-19-multiple-blast-nodes.PNG "Multiple blast nodes")
 
## Convert a point cloud to a mesh

The next step after importing the point cloud is to convert it to a mesh. To do this, you can use the **Particle Fluid Surface** command in the **Tab menu**. 

1. Click the **Geometry** pane, select **Fluid** > **Particle Fluid Surface**, select the node, and add it to the **Geometry** pane. 

   ![Fluid > Particle Fluid Surface command](media/houdini-20-particle-fluid-surface.PNG "Fluid > Particle Fluid Surfacecommand")

2. Connect it to the **transform1** node by dragging the output node to the left input node. Then click on the far-right tab of the **pariclefluidsurface1** node to activate the node in the viewport.
 
   ![Connected nodes](media/houdini-21-connected-nodes.PNG "Connected nodes")
  
    This renders the point cloud as a mesh in the viewport. The **Surfacing** tab is open in the upper-right pane above the **Geometry** tab.

   ![Surfacing tab](media/houdini-22-surfacing-tab.PNG "Surfacing tab")
 
3. If the points in the point cloud have color data connected to them, you can use those color attributes by adding the letters **Cd** to the end of the **Transfer Attributes** text box. When you add this attribute, the color will come through on your mesh.

   ![Cd attribute](media/houdini-23-cd-attribute.PNG "Cd attribute")
 
4. Sometimes you might see holes in the mesh as shown below. To fix this, adjust the **Particle Separation** and **Voxel Scale** sliders. 

   ![Particle Separation and Voxel Scale sliders](media/houdini-24-particle-scale-voxel.PNG "Particle Separation and Voxel Scale sliders")
 
5. To prepare the mesh for decimation (the next step in the process) in the **Output** tab, change the **Convert to** value from **Surface Polygon Soup** to **Surface Polygons**. This will enable you to remesh and decimate the mesh.

   ![Convert to drop-down](media/houdini-25-convert-to.PNG "Convert to drop-down")
 
6. Next add a remesh node to convert the mesh to triangles. This will enable you to decimate the 3D model to a poly count that meets your performance requirements. To do this, right-click the **Geometry** pane, and then select **Polygon** > **Remesh**.

   ![Polygon > Remesh command](media/houdini-26-polygon-remesh.PNG "Polygon > Remesh command")

7. Connect the **remesh1** node to the left input node of the **particlefluidsurface1** node. Click the middle of the **remesh1** node to activate it in the pane above the **Geometry** pane and click the far-right tab to activate the model in the viewport. You should now be able to edit the properties of the remesh and see those edits represented in the viewport.

   ![Connected nodes](media/houdini-27-connected-nodes.PNG "Connected nodes")
 
8. Play with the element sizing controls to get the results you want. You can keep the default **Uniform** option in **edge lengths** or choose **adaptive** and change the **relative density slider** (and other options) to produce the mesh you want.

   ![Element Sizing controls](media/houdini-28-element-sizing.PNG "Element Sizing controls")

## Decimate the 3D model

To reach application-specific goals, we may need to decimate the 3D model.  Decimation is the process of recomputing the surface polygons of the model to create a similar shape with less polygons. There is a reduction in visual fidelity when doing this, but also an increase in performance. The example images below show the difference between a high-quality model used for low scene complexity on HoloLens, and a low-quality model used for high scene complexity.

|High-poly 3D model|	Low-poly 3D model|
|---------------------------------------------------------------|--------------------------------------------------------------|
|![High-poly model](media/houdini-29-high-poly-model.PNG "High-poly model") |![Low-poly-model](media/houdini-30-low-poly-model.PNG "Low-poly model")|
|500,000 triangles|8,000 triangles|

1.	In the Geometry pane on the lower right, tap the Tab key to bring up the tab menu again.  Navigate to **Polygon > PolyReduce** and to select the PolyReduce node.  Place the node in the Geometry pane.

    ![Polygon > PolyReduce command](media/houdini-31-polygon-polyreduce.PNG "Polygon > PolyReduce command")
 
2.	Connect the output from the **remesh** node to the top-left input node of the **polyreduce** node.  Select the **polyreduce** node by clicking in the middle and click the far-right tab to activate the **polyreduce** node in the viewport.  Once you have done this, change the **Reduction Amount** tab’s **Target** dropdown to **Output Polygon Count** and adjust the polygon count to an amount that is within your performance requirements and maintains an acceptable visual fidelity.

    ![Connected nodes](media/houdini-32-connected-nodes.PNG "Connected nodes")
 
Our point-cloud has now been converted to an optimized 3D mesh.  In the next step we will bake a high-resolution texture to the 3D model to recover some of the visual fidelity that existed before decimation.

## Bake a high-resolution texture to our low poly mesh

One downside to reducing the number of polygons that are in a mesh is that much of the detail can be lost.  However, there is a method of capturing the detail that exists on your high-poly 3D model and applying it as a texture layered on top of your low-poly model known as “texture baking”.  Texture baking basically takes a picture of all the surfaces of your high-poly model and stitches those pictures into a quilt that is draped on top of your low-poly model.  Doing this gives you the performance of a low-poly 3D model while maintaining some of the finer details of your high-poly 3D model.  The steps below will walk you through this process.

1.	Add the **Labs AutoUV** node to the scene by right clicking in the geometry pane and navigating to **Labs > UV > Labs Auto UV** and change the method to **UV unwrap**.

    ![Labs AutoUV node](media/houdini-33-labs-autouv-node.PNG "Labs AutoUV node")

2.	Connect the **polyreduce output node** to the **AutoUV input node**.

    ![Connected nodes](media/houdini-34-connected-nodes.PNG "Connected nodes")

3.	Change your Viewport to **Vertical split** by clicking the **Viewport Layout** button and selecting **Two Views Side by Side**.

    ![Two Views Side by Side option](media/houdini-35-two-views-option.PNG "Two Views Side by Side option")
 
4.	In the left ViewPane, set the view to **UV view** by left mouse clicking the drop down and navigating to **Set View > UV viewport**.

    ![Set View > UV viewport command](media/houdini-36-uv-viewport.PNG "Set View > UV viewport command")
 
You will now see your unwrapped UVs in the left pane and your 3D model in the right pane.

    ![Unwrapped UVs displayed](media/houdini-37-unwrapped-uvs.PNG "Unwrapped UVs displayed")

5.	Add the **Labs Maps Baker** node to the geometry pane by navigating to **Labs > Output > Labs Maps Baker (Beta)**.

    ![Labs Maps Baker node](media/houdini-38-labs-maps-baker-node.PNG "Labs Maps Baker node")
 
6.	Connect the **AutoUV output** node to the **LOW Resolution input** node of the **maps baker** node.

    ![Connected nodes](media/houdini-39-connected-nodes.PNG "Connected nodes")

7.	Connect the **particle fluid surface output** node to the **HIGH resolution input** node of the **maps baker node**.

    ![Connected nodes](media/houdini-40-connected-nodes.PNG "Connected nodes")
 
8.	Select the **maps_baker** node and change the preview channel to **diffuse** and **check diffuse** in the **Transfer** section of **Bake options**.

    ![Diffuse options](media/houdini-41-diffuse-options.PNG "Diffuse options")

    >[!TIP]
    >Save your project in a specific folder by clicking the file chooser highlighted in the image above.  When we bake our texture, the .png texture file will be output into a render folder that is created in the root of the saved project.  Saving your project into its own folder will make the baked texture easy to find.

9.	Highlight the **Maps Baker** node and click **Bake** in the options pane.

    ![Bake command](media/houdini-42-bake-command.PNG "Bake comand")
 
10.	Right mouse click in the Geometry pane to access the TAB menu and navigate to **Managers >Material Network** to add a **Material Network** node to your scene.  

    ![Managers > Material Network command](media/houdini-43-managers-material-network.PNG "Managers > Material Network command")

11.	Double click the **matnet** node to open the **VEX Builder** Pane.

    ![Matnet node](media/houdini-44-matnet-node.PNG "Matnet node")
 
12.	Add a Principled Shader material by right mouse clicking in the VEX Builder pane and navigate to **Shaders > Principled Shaders**.

    ![Shaders > Principled Shaders command](media/houdini-45-shaders.PNG "Shaders > Principled Shaders command")
 
13.	In the options pane, navigate to the **Surface** tab and change the **roughness** to **0.6** and **Metallic** to **0.1**.  You can set these values to whatever you like.  We have found these values in conjunction with leaving the other values at their default values to be a good starting point.

     ![Roughness and Metallic values](media/houdini-46-roughness-metallic.PNG "Roughness and Metallic values")

14.	Next navigate to the **Texture** tab and under **Base Color** select the **Use Texture** box.  Now click on the **File Chooser** icon and select the _*_color.png_ texture that we baked out into the render folder earlier. Our principled shader is now ready for use.  There are lots of opportunities in this material network for advanced users to further modify the material, but for this tutorial we will be using this configuration.

    ![Use Texture box and selected texture](media/houdini-47-texture.PNG "Use Texture box and selected texture")

15.	Click the back arrow in the **Vex Builder** pane to navigate back to our **Geometry** Pane.

    ![Back arrow](media/houdini-48-back-arrow.PNG "Back arrow")

16.	Place a **Material** node into the geometry pane by navigating to **Material > Material**.

    ![Material > Material command](media/houdini-49-material.PNG "Material > Material command")

17.	Next, connect the output of your **AutoUV** node to the input of the **Material** node.

    ![Connected nodes](media/houdini-50-connected-nodes.PNG "Connected nodes")

18.	With the **Material** node selected, click the **operator chooser** button and select the **Principled Shader** we just created by navigating to **file1 > matnet1** and selecting the **principledshader1** operator.

    ![Operator chooser button and material file](media/houdini-51-operator-chooser-material.PNG "Operator chooser button and material file")

19.	If you click the right side of the node to activate it in your viewport you will see the texture rendered on top of your low-poly 3D model.  If it looks acceptable, we can move on to exporting the 3D model.
 
    ![Texture on low-poly model](media/houdini-52-texture-low-poly.PNG "Texture on low-poly model")

## Export the model to a GLB file

In this step, we’ll export the model to a GLB file so it can be used with Dynamics 365 mixed reality apps. 

1.	In the Geometry window, right mouse button click to bring up the Tab menu.  Navigate to **Export > ROP GLTF Output**.

    ![Export > ROP GLTF Output command](media/houdini-53-export.PNG "Export > ROP GLTF Output command")

2.	Drag a connection from the **material1 output** node to the **rop_gltf input** node.

    ![Connected nodes](media/houdini-54-connected-nodes.PNG "Connected nodes")
  
3.	In the top pane, change **Export Type** to **GLB**. 

    ![glb selected in Export Type field](media/houdini-55-select-glb.PNG "glb selected in Export Type field")
 
4.	Next to the Output File field, click the **File Chooser** and choose a name and destination for the **GLB**.  Make sure to add “.glb” to the end of your file name.

    ![File Chooser button and Name field](media/houdini-56-file-chooser-name.PNG "File Chooser button and Name field")

5.	Next, click the **Render to Disk** button to finalize the export and to create the **GLB** file.

    ![Render to Disk button](media/houdini-57-render-to-disk.PNG "Render to Disk button")
 
Congratulations! You have officially taken a point-cloud and converted it into a mixed reality ready 3D model.

## Creating a template

An advantage to using Houdini is all of the steps that are used to prepare the 3D model exist in the application, even export to the glTF format.  This node tree can be reused to create more 3D models from point clouds.  While you will have to click bake and maybe adjust a few values to tweak everything to your liking, the majority of the processing is automated and we can rapidly create more 3D models.  

1.	The first thing we will do is replace whatever geometry is currently being used with a default geometry.  This makes our template file lightweight so that it will load quickly when we open it.  To do this, do the following:

    a.	Click on your file icon to activate the geometry file menu in the upper pane.
    
    b.	Once activated, change the “Geometry File” field to say “default.bgeo” and click **Reload Geometry**.
    
    c.	This will refresh the geometry so that it is now a generic cube.
    
    d.	Go ahead and change the file name to something generic like “Template” as well.
    
      ![Refreshed geometry](media/houdini-58-refreshed-geometry.PNG "Refreshed geometry")
 
2.	With our template setup, save your file as something memorable like “Prep_Template.”  To save the file go to **File > Save**.

    ![File > Save command](media/houdini-59-file-save.PNG "File > Save command")

3.	Your Template is now ready.  Close Houdini so that we can perform a complete walkthrough using our template.

### Using the template

1. Now that our template is ready, Launch Houdini and open your template file by going to File > Open, and selecting the template we saved in the previous section.

    ![File > Open command](media/houdini-60-file-open.PNG "File > Open command")
 
2. Click on the center of the geometry file node to switch to the File context menu above, and then click the “Open floating file chooser” button to select your .ply point cloud file.

    ![Selected node and File Chooser button](media/houdini-61-selected-node-file-chooser.PNG "Selected node and File Chooser button")
 
3. Click the “Reload Geometry” button to load your point-cloud into your scene.

    ![Reload Geometry button](media/houdini-62-reload-geometry.PNG "Reload Geometry button")
 
4. Once your point-cloud loads return to the **Maps Baker** node and click **bake** to bake a new texture for your 3D model.

    ![Bake command](media/houdini-63-bake-command.PNG "Bake command")

5. Click the right tab of the **Material** Node to view what your baked model looks like.

    ![Right tab of Material node](media/houdini-64-right-tab-material-node.PNG "Right tab of Material node")

6. If you are satisfied with the 3D model, navigate to the **rop_gltfB** node and export your 3D model by clicking **Render to Disk**.  

    ![Render to Disk command](media/houdini-65-render-to-disk.PNG "Render to Disk command")

7. If you are not satisfied with how your model looks, then try adjusting the options in the **particle fluid surface**, **remesh**, and **polyreduce** nodes.  Once your model looks acceptable, bake your texture again and export your 3D model.

## Viewing your 3D model in mixed reality

Now that you have prepared your 3d models, you can learn more about using the following Microsoft Dynamics 365 experiences to view your 3d model in mixed reality here: 

[Dynamics 365 Product Visualize](https://docs.microsoft.com/dynamics365/mixed-reality/product-visualize/) 

[Dynamics 365 Guides](https://docs.microsoft.com/dynamics365/mixed-reality/guides/) 

[Dynamics 365 Layout](https://docs.microsoft.com/dynamics365/mixed-reality/layout/index) 
 
### More information 
 
Several screenshots in this document were taken from the Houdini software program in order to provide clear instructions on how to use Houdini’s software.  More information about Houdini can be found here: [SideFX](https://www.sidefx.com/tutorials/alicevision-plugin/)
 
The Microsoft Corporation is not responsible for, and expressly disclaims all liability for damages of any kind arising out of the use of Houdini, or reliance on these instructions. This document is created only to provide general information to our customers and does not take into consideration any individualized business plans or specifications. 
 
The use in this document of trademarked names and images is strictly for informative and descriptive purposes, and no commercial claim to their use, or suggestion of sponsorship or endorsement, is made by the Microsoft Corporation. 

