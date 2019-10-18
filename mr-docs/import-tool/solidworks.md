

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


