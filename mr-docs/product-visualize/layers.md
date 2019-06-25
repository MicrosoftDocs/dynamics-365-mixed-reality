---
author: erhong
description: How to toggle the visibility of layers on a 3D model in Dynamics 365 Product Visualize 
ms.author: erhong
ms.date: 06/18/2019
ms.service: crm-online
ms.topic: article
title: How to toggle the visibility of layers on a 3D model in Dynamics 365 Product Visualize 
ms.reviewer: 
---

# Toggle visibility of layers on a 3D model in Dynamics 365 Product Visualize 

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

## What is a layer? 

A single 3D model consists of one or more layers which can be thought of as categorized objects often grouped by function or location. 

Layers are created in model design software tools such as CAD and can be built in a nested or flattened format. 

## Introduction to the Layers tool

In Dynamics 365 Product Visualize, the Layers tool allows you to toggle the visibility for any existing layer(s) in a 3D model. 

After a model is placed in the scene, you can enter the Layers tool by tapping on the toolbar button on the right side labeled Layers. 

The Layers tool presents a list of the placed 3D model's layers where each row can be selected to toggle the visibility of that layer. 

A layer that contains one or more other layers acts as a folder that can be expanded or collapsed by tapping on the [+] or [-] button respectively. 

By default, all layers in the model are visible. 

## Icon Legend

Each layer can be selected by pressing on the checkbox placed to the right of each layer. 

* ![Unselected](media/unselected.PNG "Unselected") 
* ![Selected](media/selected.PNG "Selected")

Additionally, each layer has an indicator of whether it is a folder or individual layer placed to the left of each layer. 

* ![Expandable Folder](media/expandable-folder.PNG "Expandable Folder with no children layers visible")
* ![Collapsible Folder](media/collapsible-folder.PNG "Collapsible Folder with children layers visible")
* ![Individual Invisible Layer](media/individual-layer-visibility.PNG "(1) Individual Invisible Layer")
* ![Individual Visible Layer](media/individual-layer-visibility.PNG "(2) Individual Visible Layer")


## Toggle a layer's visibility off 

1. After placing a model, select **Layers** on the right side of the screen. 

![Enter Layers Tool](media/layers-tool.PNG "Enter Layers")

2. Tap on the right checkbox of the desired layer(s) you would like to toggle the visibility of. The layers you select will be visibily outlined in white. 

* ![Layer Selected](media/selected.PNG "Select Layers")

3. Tap the **Hide** button to turn the visibility of the selected layer(s) off 

![Hide Layers](media/hide-layer.PNG "Hide Layer")

## Show or Hide all layers 

1. After placing a model, select **Layers** on the right side of the screen. 

![Enter Layers Tool](media/layers-tool.PNG "Enter Layers")

2. Tap on the right checkbox on the layers toolbar to select all layers belonging to the placed model. 

![All Layers Selection](media/layer-select-all.PNG "Select All Layers")

3. Do one of the following: 

- To show all layers, tap on **Show**

- To hide all layers, tap on **Hide** 

![Layer Toggle](media/layer-toggle.PNG "Toggle Layers")

