

# Use Agisoft Metashape to create 3D models for use in Microsoft Dynamics 365 mixed-reality applications

This tutorial will walk you through the process of using Agisoft’s Metashape photogrammetry software to create a 3D model that can be 
used on Microsoft Dynamics 365 Mixed Reality applications.

This document is created strictly for informative purposes to demonstrate how Agisoft Metashape works with Microsoft Dynamics 365 
Mixed Reality applications.  The Microsoft Corporation is not affiliated with, is not a partner to, and does not endorse or sponsor 
Agisoft or any of Agisoft’s products.

## What is Agisoft Metashape?

Agisoft Metashape is a stand-alone software product that performs photogrammetric processing of digital images and generates 3D spatial 
data to be used in GIS applications, cultural heritage documentation, and visual effects production as well as for indirect measurements 
of objects of various scales. -Agisoft Metashape

## Photography tips

The following tips will help you take quality photos for photogrammetry:

- If possible, take photos in a location where the lighting will remain consistent and does not cast shadows stark shadows

- If there are shadows cast, try to keep your own shadow out of the picture

- Avoid having moving objects in the background while taking photos

- If the camera you are using has HDR, turn this feature off and do not adjust the exposure of your photographs while you are capturing 
images

- Take pictures about 1 meter apart while circling the object

- If it is possible, maintain a perpendicular location to the model while you are taking photos

- If the subject is large, move in a lateral motion from one end of the object to the other changing the height with each pass until 
you feel that you have captured all of surfaces of the object

## Set preferences

While the majority of Metashape’s preferences can be left at their default values, there are a few alterations that should be made before getting started.

1. First navigate to the preferences panel by selecting **Tools > Preferences**.

SCREEN SHOT GOES HERE
  
2. Click through the **General**, **GPU**, and **Advanced** tabs at the top to confirm that the following options are selected.  

SCREEN SHOT GOES HERE
 
3. On the **General** tab, check the “Write log to file” option under the “miscellaneous “ tab and choose a location and file name you would like to use for your log.  Click **Apply** and navigate to the **GPU** tab.

SCREEN SHOT GOES HERE
 
4. On the **GPU** tab, check any GPUs that you have available for processing.  If you only have one GPU available, check “Use CPU when performing GPU accelerated processing”, otherwise leave it unchecked.  Click **Apply** and navigate to the **Advanced** tab.

SCREEN SHOT GOES HERE
 
Start with these settings from the “advanced” tab.  If the camera you are using to take the photos has extensive meta data about the location, orientation, etc. then you may wish to experiment with the options in the Import / Export section.  Click **OK** to apply and close the preferences pane.

## Import photos

Now that our environment preferences are set up, we can begin adding the photos that will be used to construct our 3D model.

To do this, navigate to **Workflow** > **Add Photos** and select the photos that you would like to import.

SCREEN SHOT GOES HERE
 
## Mask photos

When determining what aspects of your photographs you would like to turn into a 3D model it can be helpful to mask the 3D object.  You may find it beneficial to do this in pictures from different angles.  While it is not necessary to mask your object in every single photo, the more photographs you mask, the more accurate the final result will be.

1.	To add a mask, double-click an image to open it and choose a selection tool such as the “intelligent scissors” and outline the subject you wish to turn into a 3D model.

SCREEN SHOT GOES HERE
 
2.	Once you have your model outlined, press the **Add Selection** button to create the mask.

SCREEN SHOT GOES HERE
 
Repeat this step from multiple angles to get a higher quality output.

SCREEN SHOT GOES HERE


 

