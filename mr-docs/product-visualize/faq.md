---
author: mamithan
description: Frequently asked questions about Dynamics 365 Product Visualize
ms.author: mamithan
ms.date: 01/17/2020
ms.service: crm-online
ms.topic: article
title: Frequently asked questions about Dynamics 365 Product Visualize
ms.reviewer: v-brycho
---

# FAQ: Dynamics 365 Product Visualize

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

## What are the requirements for running Microsoft Dynamics 365 Product Visualize, and what platforms does it support?

For information about platforms and requirements, check out our [Requirements page](requirements.md).

## What kind of 3D content can I add?

Dynamics 365 Product Visualize supports GLB files only.

## How do I get my content in the right format?

To learn how to format your content, see the following page on the Khronos website: [Art Pipeline for glTF](https://go.microsoft.com/fwlink/p/?linkid=2083000). 

## How does Dynamics 365 Product Visualize connect with Dynamics 365 Sales?

After you sign in with your Azure Active Directory credentials, Dynamics 365 Product Visualize displays organizations associated with your Dynamics 365 Sales account. Opportunities and products associated with your organizations automatically show up in the app, as do 3D models attached to your products.

## Can I use Dynamics 365 Product Visualize to do remote sales?

At this time, Dynamics 365 Product Visualize doesn't support remote capabilities.

## Why is the "Need admin approval" message displayed after signing in?

![Admin Approval](media/admin-approval.PNG "Admin Approval")

This message indicates that your organization requires administrator approval before any new apps can be used to access organizational resources. Talk to your system administrator to get approval to use Dynamics 365 Product Visualize in your organization. In the meantime, you can set up a [free trial version](setup.md).

## Why don't I see my Dynamics 365 instances?
 
Dynamics 365 Product Visualize can connect to instances of Dynamics 365 Sales version 9 or later. It doesn't support on-premises Dynamics 365 solutions or older instances of Dynamics 365 Sales. Make sure your instance meets the [minimum requirements](requirements.md) for using Dynamics 365 Product Visualize. If your instance meets the requirements, make sure you're signed in to the app with the same credentials you use to access Dynamics 365 Sales.

## Why am I getting a message that says my organization isn't set up to use Dynamics 365 Product Visualize?

This message indicates the Dynamics 365 Sales instance you selected doesn't meet the [minimum requirements](requirements.md) for using Dynamics 365 Product Visualize. If you have access to more than one Dynamics Sales instance, make sure you selected the correct one.

## How do I find my opportunities?

Dynamics 365 Product Visualize helps you stay organized by focusing only on the opportunities that are important to you. From the Opportunity Selection view, there are three options for viewing your opportunities:

1. **My Open Opportunities** - Open opportunities where you're listed as the owner.
2. **My Connected Opportunities** - Open opportunities where you've been added to the Sales team.
3. **My Followed Opportunities** - Open opportunities that have been marked as __Followed__.

If an opportunity doesn't show up in the app, go to the Dynamics 365 Sales Hub and ensure that at least one of these criteria is met.

## Why doesn't my model load?

Models with very high polygon counts might take a long time to load, especially over slower connections. If the model doesn't load at all, the GLB file might not be valid. A corrupt or invalid GLB file can appear as if it were loading but it will never actually load. If this happens, restart the app and try again. If, after restarting, the model still fails to load, try re-exporting the GLB from your authoring software and upload it again to SharePoint. If that doesn't work, try loading the model in a different glTF viewer like [BabylonJS Sandbox](https://sandbox.babylonjs.com/).

Larger models might exceed the memory of the mobile device you're using. This is especially true on previous-generation iPhones. To reduce the model's memory requirements, reduce the size of any textures associated with the model and decimate the model to use fewer polygons.

## How far must I stand from the object to see it?

Initially, you must be 3 feet to 4 feet away from the location where you want to place the model. When the model appears and you place it on a surface, the model size should initially be contained within the device's screen. If you scale it up, depending on the model's size, this may require you to move back several feet to see the object in its entirety again.
 
## What is the best way to obtain tracking?

Point the device down so that it is parallel to the desired surface. Hold it there momentarily and then slowly tilt the device up so that it is close to a 45 degree angle to the floor. If tracking is still not achieved, point the device toward the surface again and slowly raise it and lower it while keep parallel to the surface. When tracking is gained, tilt the device up to the desired angle pointing it at the desired placement location on the surface.  
 
## What should I do if I lose tracking during a presentation? 

Initially, you should try pointing the device down so it is parallel to the surface and then slowly tilting it up. If that does not restore tracking, select the hamburger menu (three bars) icon on the top-left of the screen and then select **Opportunities**. Select the opportunity that contains the product and then select the product containing the model you were viewing. You will then need to go through the placement process again with the initial model in the product. After placing the initial model, tap the **Model** button on the right of the screen to open the model menu. From the model menu, find the desired model, and then select it to place it on the selected surface. 
 
## What surfaces and locations are best to track on? 

Low contrast non-reflective surfaces with non-repeating patterns with good lighting are ideal. 
 
## Are there any known problematic tracking locations? 

You will want to avoid something with large high-contrast repeating patterns like a checkerboard pattern with high-contrast light and dark squares. This can cause the device difficulty in establishing an even surface to place the model on. Highly reflective surfaces also can cause unwanted behavior and should be avoided if possible. Areas with little or dim lighting should be avoided as well.    
 
## Can I automatically scale the object to 100%? 

Yes. By double tapping on the model it will expand to its 100% scale. Double tapping on the model again will scale it back to the previous scale it was at. 
 
## How do I switch between objects during a presentation? 

If the desired model is in the current Product:
1. Tap the **Model** button to open the model browser. 
2. Scroll left or right to find the desired model (you can also use search if there are a large number of models in the browser). Tap on the model to load it. 
 
If the desired model is in another Product or Opportunity: 
1. Tap on the hamburger menu (three bars). 
2. Tap on Opportunities and then on the Opportunity with the desired model. 
3. Tap on the Product with the desired model.  
4. Go through the Placement process and place the initial model. 
5. Tap on the Model button to bring up the model browser at the bottom of the screen. 
6. Scroll left or right to find the desired model (you can also use search if there are a large number of models in the browser). Tap on the model to load it. 
 
## How do I export the text and image in my note for email? 

Navigate to the note you want to export. Tap on the overflow menu (three dots) on the note itself. Tap on Export Note on the popup menu. Tap on email and select the app that your email uses.  
 
## How do I download and retain the model locally? 

First you will need to enable the offline mode. Tap on the Hamburger menu (three bars) at the top left of the screen. Tap on Preview features. Tap on the toggle for Offline mode so that it is enabled. 
 
Navigate to your Opportunities and tap on the one that has the Product you want to save. Observe the cloud icon with the down pointing arrow on the lower left corner of each product. Tap on that icon in the Product that has the desired model. This will start a download process changing the icon to a square and loading circle. After every model in the Product has been downloaded a blue circle with a check market will appear. Those models are now on the device. 
 
If you lose network connectivity and want to view the downloaded files restart the app and navigate to the Opportunity and Product as before. The models that were downloaded should appear and be accessible from the Product.  
 
## Will my notes be visible to other users? 

Notes are currently saved to the Opportunity they were made in. If someone with another account also has access to that Opportunity they can see the notes on that model. 
 
## Can I update the Product Notes during a meeting? 

Currently you can only make new notes or delete notes. 
 
In the Note menu tap on the Add Note to make a new one. To delete a note tap on the overflow menu (three dots) on the upper right corner of the note. Tap delete now and confirm.    
 
## If I delete a note, how can I recover it? 

You cannot recover a deleted note in the app. However, the note is saved in Dynamics even if deleted so the text and image can be recovered to be used in the app again. 
 
## Can I walk away from my model and come back later? 

The iOS device uses a camera to orient to the world and placing the device so that the camera is covered, or leaving it idle so that the screen turns off, will likely cause the device to lose its world information and lose where it placed the object. If this happens you will need to redo the placement process for the model. 
 
## How can I ensure success when manipulating my model? 

Be aware of the positioning of the hand holding the device as a stray finger on the screen might cause unintended movement of the model when trying to manipulate it via gestures


### See also

[Requirements for setting up Dynamics 365 Product Visualize](requirements.md)<br>
[Set up Dynamics 365 Product Visualize](setup.md)<br>
[Administrator guide](admin-guide.md)<br>
[User guide](user-guide.md)<br>
