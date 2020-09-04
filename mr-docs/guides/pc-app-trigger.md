---
author: Mamaylya
description: Learn how to create a trigger in the Dynamics 365 Guides PC app to automatically advance the operator to the next step based on detection of their hands in HoloLens 2.
ms.author: mamaylya
ms.date: 08/25/2020
ms.service: crm-online
ms.topic: article
title: Create a trigger for step navigation in the Dynamics 365 Guides PC app
ms.reviewer: v-brycho
---

# Create a trigger for step navigation in the Dynamics 365 Guides PC app

If you’re using HoloLens 2 with Microsoft Dynamics 365 Guides, you can create a trigger that automatically advances an operator to the next step based on detection of their 
hand(s). This provides a very natural way for operators to complete a task. You place the triggers in the real world where the work takes place. The operator doesn’t have to 
disrupt the flow of their work by gazing at a button on the instruction card after completing each step. 

When an operator activates a trigger, they see a **Next Step** or **Previous Step** visual cue wherever they’re gazing to let them know that they’ve completed the step. They also receive audio feedback for extra reinforcement.

> [!NOTE]
> You can create a trigger with a HoloLens 1 device, but you can’t test a trigger on HoloLens 1, and operators on HoloLens 1 won’t be able to use the trigger since 
triggers require HoloLens 2 hand detection.

## Two types of triggers

There are two types of triggers:

- **Visible triggers.** Dynamics 365 Guides comes with pre-configured **Next** and **Back** buttons that you can place in the real world. Operators select a visible trigger with their hand(s) to move forward or backward.  

    ![Example of visible trigger](media/trigger-visible.PNG "Example of visible trigger")
 
    > [!TIP]
    > You can add a dotted line to a visible trigger to tie it to a specific place in the real world.

- **Invisible triggers.** An invisible trigger automatically advances an operator to the next step when the trigger is activated. Operators don’t see any evidence of the trigger until they activate it, at which time they’ll see a light green box. 

    ![Example of invisible trigger](media/trigger-invisible.PNG "Example of invisible trigger")
 
This reduces clutter for the operator and helps them focus on the task at hand.

## When is a trigger activated?

You can set up the trigger to activate when the operator's hand enters the trigger area or when it exits the trigger area, as described in the procedures below. 

## Create a trigger 

You create a trigger in the same way that you create any other hologram in the PC app. 

> [!NOTE]
> You can also [create a trigger directly in the HoloLens app](HoloLens-app-trigger.md).

1. In the PC app, select the **3D toolkit** tab.

2. Open the **Triggers** section, and then drag the type of trigger (**Back**, **Invisible**, or **Next**) you want to the bin.

    ![Triggers section in 3D toolkit](media/triggers-category-pc-app.PNG "Triggers section in 3D toolkit")

## Configure the trigger 

After creating your trigger, you need to configure it. You can configure it on the default step (how to define?) or on a question step if you're creating a non-linear (branching) guide. [Learn more about creating a branching guide](pc-app-branching.md). 

### Configure the trigger on a default step

1. Select the trigger in the bin. This opens the **Properties** tab on the right side of the screen that provides a preview of the trigger and the trigger properties. [Learn more about the Properties pane](addlinkhere.md)

    SCREEN SHOT GOES HERE

2. In the **Properties** tab, do the following:

    a. In the **Activation** field, select one of the following:
    
      - **On Hand Enter** to activate the trigger as soon as the operator places their hand in the trigger area.
      
      - **On Hand Exit** to delay the trigger activation until the operator has removed their hand from the trigger area.
      
    b. In the **Action** field, select one of the following:
    
      - **Back** to take the operator back to the previous step in the guide.
      
      - **Next** to take the operator to the next step in the guide.
      
      - **Navigate** if you want to take the operator to a specific step in the guide. After selecting **Navigate**, you can select the exact step to go to in the **Destination** list. Using the **Navigate** option enables you to have the operator skip multiple tasks or steps for different scenarios. 
 
## Configure a trigger on a question step (for branching guides)

Configuring a trigger on a question step allows operators to navigate a guide through the responses included in the question step.  Use Response 1, Use Response 2, and Use Response 3. These correspond to the question responses set in the step editor [link to branching responses documentation page?]. 

1. Select the trigger in the bin to open the **Properties** tab. 

2. In the **Properties** tab, do the following:

    a. In the **Activation** field, select one of the following:
    
      - **On Hand Enter** to activate the trigger as soon as the operator places their hand in the trigger area.
      
      - **On Hand Exit** to delay the trigger activation until the operator has removed their hand from the trigger area.
      
    b. In the **Action** field, select **Use Response 1** to configure the trigger to navigate to the destination set for Response 1. For example, if the first response’s destination is set to **Task 3**, configuring the trigger to **Use Response 1** means the trigger will navigate to **Task 3** when activated. If you update the response’s destination, the trigger will also be updated.
    
    c. Set any other **Use Response** values to correspond with the responses in the question card.

## Place the trigger

After adding the trigger in the PC app, [place and test it in the HoloLens app](hololens-app-trigger.md).

## What's next?

[Place and test a trigger in the HoloLens app](hololens-app-trigger.md)
 
