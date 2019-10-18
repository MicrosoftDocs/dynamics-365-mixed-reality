

# Prepare Dassault SolidWorks 3D models for use in Dynamics 365 mixed reality applications

There are several ways that you can optimize 3D models for mixed reality inside of Dassault Systèmes SolidWorks. This tutorial provides you with easy-to-follow procedures for using each of these methods. Some of the procedures are redundant, so you may not need to use them all. Experiment with each procedure and decide what suits your use case best. 
 
Sections of this tutorial are for 2019 and later only, and assume you’ve successfully installed the SolidWorks XR Exporter onto your local machine.  
 
> [!IMPORTANT]
> This document is created strictly for informative purposes to demonstrate how Dassault Systèmes SolidWorks works with Microsoft Dynamics 365 mixed reality applications. Your use of third-party applications is subject to terms between you and the third party. The Microsoft Corporation is not affiliated with, is not a partner to, and does not endorse or sponsor Dassault or any of Dassault Systèmes' products. [There are several other content-creation applications that can be used to prepare your 3D models](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/convert-models#tools-for-exporting-cad-models). 

## What is Dassault Systèmes SolidWorks? 
 
SolidWorks 2019 provides the breadth of tools to tackle the most complex problems, and the depth to finish critical detail work. New features help you improve your product development process to get innovative products into production faster.  [Read more about SolidWorks](https://www.solidworks.com/). 
 
## Optimize 3D models in SolidWorks 

The features in this tutorial have been identified as ways to optimize 3D models for use in mixed reality applications. Depending on how complex your model is, you may be able to just export it as a GLB file or you may need to use a combination of several features. 
 
## Remove features with the Simplify tool 

If your 3D model is extremely complex and you're having performance issues, you can optimize it with the Simplify tool.  The Simplify tool provides a wide range of options for simplifying your models to different levels, including internal part removal, small part removal, defeaturing and more. [Learn more about using the Simplify tool](https://help.solidworks.com/2018/English/SolidWorks/sldworks/t_simplifying_parts.htm). 

To remove features with the Simplify tool:

1. Access the Simplify tool, select **Tools > Find/Modify > Simplify**. 

   SCREEN SHOT GOES HERE: solidworks-simplify-tool
 
2. Choose from the following options: 

   - **Features**. Decide which features you want to search for. Select fillets, chamfers, and holes as these features create lots of polygons when transcoded.
   
   - **Feature Parameter or Volume Based.**  When you select the **Feature Parameter** option, SolidWorks selects objects whose parameters (such as “Fillet Radius”) are smaller than the simplification factor. When you select the **Volume Based** option, SolidWorks selects objects if the feature volume is less than the volume of a part times the value in the **Simplification factor** field. Either method works fine. Selecting the **Volume Based** option and entering a value of 0.1 for the **Simplification factor** field will give you a great first pass. If you don’t find many objects, increase the **Simplification factor** value and try again. Select **Find Now** to see the results. 
 
      SCREEN SHOT GOES HERE: solidworks-simplify-features

3. Select the **All** check box, and then select **Suppress**. 

    SCREEN SHOT GOES HERE: solidworks-suppress
 
   The features you select are removed from your model. If you discover that features of your model were removed that you wish to keep, you can undo the process. Clear the **All** check box, and then select just the items you want to remove. 

## Remove small parts with the Defeature tool

The Defeature tool provides another optimization option. You can use this tool for both part removal and for creating a silhouette of your model.  

1. To access this tool, select **Tools > Defeature**. 
 
    SCREEN SHOT GOES HERE: solidworks-defeature
 
2. Select to either simplify your geometry or create a silhouette. 

    SCREEN SHOT GOES HERE: solidworks-geometry-or-silhouette

### Simplify geometry

1. Select the Simplify Geometry icon, and then select the Next arrow. 
 
    SCREEN SHOT GOES HERE: solidworks-simplify-geometry
    
2. Select the **Internal components** check box.  

3. Select the **Small components** check box, and enter a percentage to use.  We suggest starting with 1%. This will often remove nuts, bolts, and washers from an assembly while leaving the more visually important components. You can increase this percentage if you need to remove more. Select the next arrow when you're ready.

    SCREEN SHOT GOES HERE: solidworks-components
    
4. Select the Next arrow again to skip adding motion to the assemblies.  

    SCREEN SHOT GOES HERE: solidworks-motion
    
5. If you want to retain the detail for specific geometry areas, select them. Otherwise, they'll be optimized. You can also select the check boxes under **Auto-Select** to retain all holes or holes of a specific size. Select the Next button when you're done.

    SCREEN SHOT GOES HERE: solidworks-autoselect
    
6. The tool "defeatures" the model. If there's anything that was missed that you would like to remove, select it in the following screen. When you're done, select the Next button. 

    SCREEN SHOT GOES HERE: solidworks-select-additional-features
    
7. If the optimized model meets your needs, select **Save as a new document**, and then select the green arrow. 

    SCREEN SHOT GOES HERE: solidworks-save
 
8. Name your model, and then select **Save**. The model is saved as a single SolidWorks part file. 

### Create a silhouette

Another option for optimizing your model is the Silhouette tool. This tool is useful when you just need to understand the basic shape of a complex model.  

1. To access the tool, select **Tools > Defeature**.

    SCREEN SHOT GOES HERE: solidworks-defeature
    
2. Select **Sillhouette**. 

    SCREEN SHOT GOES HERE: solidworks-silhouette
 
3. Highlight the entire model (or portions of the model if you only want to modify certain parts), select an option under  **Simplification Method**, and then select **Add Group**. For this example, we selected the **Tight Fit Outline** option, but feel free to experiment with other options.
 
    SCREEN SHOT GOES HERE: solidworks-tight-fit-outline
 
4. You'll see a preview window that shows what your silhouetted model will look like. When you have it the way want, select the Next button.  
 
    SCREEN SHOT GOES HERE: solidworks-preview-window
 
5. Select **Save as a new document**, and then select the green check mark to save your model. 
 
    SCREEN SHOT GOES HERE: solidworks-save-silhouette

