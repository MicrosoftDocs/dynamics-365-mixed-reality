---
author: BryceHo
description: Glossary of terms for Dynamics 365 Guides in preview
ms.author: anhaman
ms.date: 04/30/2019
ms.service: crm-online
ms.topic: article
title: Glossary of terms for Dynamics 365 Guides in preview
ms.reviewer: v-brycho
---

# Glossary of terms for Dynamics 365 Guides in preview

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]
 
When you're working with Microsoft Dynamics 365 Guides in preview, you might find this glossary of terms helpful.

## 3D parts
3D content that you assign to a step to support that step. You assign 3D parts in the PC application, and then place the holograms in a real-world environment in HoloLens Author mode.

## 3D toolkit
A library of predefined objects included in Dynamics 365 Guides that use can use to get started right away. For example, there are 3D objects such as pointers and arrows that you can add to a step to support that step.

## Air tap
A gesture that’s equivalent to a “click” with a mouse. For more information on how to do an air tap, see [Gestures to know](authoring-gestures.md).

## Alignment
The process of making sure that a guide “lines up” with associated objects in the real world when used on HoloLens. Alignment is crucial and mandatory for creating any guide. For more information, see the [Authoring guide](pc-authoring.md).

## Asset
Collective term for the complete set of objects that you can add to a step to support that step. Assets include 2D objects (images and videos) and 3D objects (3D parts and objects from the 3D toolkit). 

## Author
The person who creates a guide.

## Calibration
A process in which HoloLens adjusts the hologram display according to a user's interpupillary distance (IPD). The HoloLens device must be calibrated correctly so that the guide aligns properly in the real world. Proper calibration is also necessary to place holographic objects in HoloLens Author mode. HoloLens includes a Calibration app that can be used by authors and operators for this purpose. 

## Digital twin
A 3D representation used for one type of alignment. You place the digital twin, which can be a CAD model or scanned model, directly over its counterpart in the real world, and then use a gesture to align the guide to the digital twin.

## Field of view
The size of the HoloLens display where holograms show up. It’s important to keep the field of view in mind when placing holograms in a real-world environment.

## Fit Box setting
A setting that ensures the HoloLens device fits properly. A proper fit is very important for alignment purposes.

## Gaze
The act of looking at a user interface element with HoloLens. In some cases, you can select an item just by gazing at it. In other cases, you use gaze to target an object and then act on that target with a gesture.

## Gesture
A hand movement that enables an operator to do an action in mixed reality. For more information, see [Gestures to know](authoring-gestures.md).

## Interpupillary distance (IPD)
The distance between a user’s eyes. Different users have different IPDs. To align content correctly, HoloLens needs to be calibrated for each user’s IPD. 

## Marker
A computer-generated visual used for one type of alignment. You gaze at the marker to align the guide with its spatial coordinates.

## Operator
The person who uses a guide to do a set of tasks. 

## Outline page
A page in the PC Authoring application that you use to add tasks and steps. From the Outline page, you can get a sense of the whole guide and restructure tasks by dragging them from one place to another. The Outline page also includes customizable alignment instructions and a special step called the Completion step (also customizable).

## Step
A short, discrete work item that an operator does to complete a task. Tasks are made up of steps. Steps are also the central navigation point in a guide.

## Step card
The fundamental building block in Guides. You add text and supporting assets to a Step card in the PC authoring application, and then place holograms associated with each step in a real-world environment in HoloLens Author mode. The operator works through each step to complete a task or series of tasks. For more information about Step cards, see the [Authoring guide](pc-authoring.md).

## Style
Visual properties that you can add to any 3D object to reinforce what you want the operator to do or know. Examples of styles include Pick up, Place, and Caution.

## Task
A piece of work to be done or undertaken. A task is made up of steps that the operator must follow to complete the task. 

## Tether
A holographic link that ties a step visually to the area where you want the operator to focus. It helps the operator find content or understand what they’re supposed to be looking at in the real world. You can use a tether together with a 3D object, such as a holographic arrow or number. 

### See also

[Overview of authoring a guide](authoring-overview.md)<br>
[Operator's manual](operator-guide.md)<br>
[Analyze your guides](analytics-guide.md)
