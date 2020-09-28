

## Use PiXYZ Studio to prepare 3D models for use in Dynamics 365 mixed-reality apps

This tutorial outlines a general process for using PiXYZ software to convert Computer-Aided Design (CAD) based parametric assets into polygon-based .GLB files that perform 
well in Dynamics 365 mixed-reality apps (see [Optimize your 3D models](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/optimize-models#performance-targets) for information about performance targets). Keep in mind that every asset and use case ise different, 
so you may need to adjust the process accordingly. 

> [!IMPORTANT]
> This document is created strictly for informative purposes to demonstrate how PiXYZ Studio works with Dynamics 365 mixed-reality apps. Your use of third-party applications 
is subject to terms between you and the third party. Microsoft Corporation is not affiliated with, is not a partner to, and does not endorse or sponsor PiXYZ or any of 
PiXYZ’s products. There are [other content-creation apps](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/convert-models#tools-for-exporting-cad-models) you can use to prepare your 3D models.

## What is PiXYZ Studio?

[PiXYZ Studio](https://www.pixyz-software.com/studio/) helps companies and 3D users re-use their CAD data for any visualization scenario.

## Import a CAD asset into PiXYZ Studio

1. Open PiXYZ Studio, and then on the top-left side of the toolbar, select **Wizard** to start the Import wizard.

    SCREEN SHOT GOES HERE
 
2. In the **Import Wizard** dialog box, use the settings shown above to create a high-quality tessellation as a starting point.

3. **Execute**.

## Scene cleanup

Start by manually removing all parts and assemblies that are not required for the mixed-reality app.

1. In the Viewer or the Product Structure (Tree), select **Occurrences**.

2. Press Delete on the keyboard to delete the selection from the scene.

> [!NOTE]
> Tools in the **Selection** menu such as **Select Instances**, **Select Similar** and **Select By Max Size** can be very useful for quickly selecting multiple occurrences to delete.

After removing all the unnecessary parts and assemblies, you can use the following commands to clean up left over occurrences, materials, textures, and lines:

•	**Scene** > **Delete Empty Occurrences**

•	**Materials** > **Clean Unused Materials**

•	**Materials** > **Clean Unused Textures**

•	**Mesh** > **Delete Lines**

> [!NOTE]
> If lines are important for your scenario, you can use **Mesh** > **Create Textures From Lines** on co-planar lines to bake a textured polygon to use in mixed-reality apps. See the [PiXYZ documentation](https://www.pixyz-software.com/documentations/html/2020.1/studio/api/Algo.lineToTexture.html) for more information.

## Remove features

If there are holes in any of the parts or assemblies that aren’t required for your scenario, you can remove them for potentially large polygon savings.

1. Select the parts and assemblies that have the holes you want to remove.

    > [!NOTE] 
    > If you don’t make a selection, PiXYZ runs the **Remove Holes** command on the entire scene.

2. Select **Optimize Mesh** > **Remove Holes**.

3. In the **Remove Holes** window, select the types of holes you want to remove:

    - **Through Holes:** Holes that go through a surface and come out the other side.

    - **Blind Holes:** Holes that go into a surface but stop part way through.

    - **Surfacic Holes:** Holes that are cut into a surface but don’t have any depth.
    
    SCREEN SHOT GOES HERE
 
4. Enter a number (in millimeters) for the **Max Diameter** field. Holes with a diameter below this value that match the types you set will be removed.

5. Optionally, select the **Fill With Material** check box to select a material to fill holes that are removed to leave the appearance of a hole while still saving polygons.



