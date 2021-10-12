---
author: Mamaylya
description: Get oriented with the Microsoft Dynamics 365 Guides HoloLens app, and learn how to place holograms, add styles, and more.
ms.author: mamaylya
ms.date: 09/07/2021
ms.topic: article
title: Place holograms in the Dynamics 365 Guides HoloLens app
ms.reviewer: v-brycho
---

# Get oriented with the Dynamics 365 Guides HoloLens app (for authors)

If you're a Microsoft Dynamics 365 Guides author, after you anchor your guide in the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] [!include[pn-hololens](../includes/pn-hololens.md)] app, you'll see the Step card page. The Step card is the hub of everything that you do with your guide. It's also what your operators see when they use the guide. The Step card follows the operators around to keep the instructions where they need them as they move around their workspace.

You and your operators can move through a guide by gazing at the **Next** and **Back** buttons. If you select the **Back** button, it returns you to the most-recently-visited step (similar to a web browser **Back** button). You can also use gestures such as air tap. 

![Moving through a guide.](media/navigate-example.PNG "Moving through a guide")

> [!TIP]
> When you switch between the PC app and the HoloLens app, select **Refresh** to make sure that you have the latest version of the guide.

## Step card page overview

The following illustration shows the different user interface elements of the HoloLens app Step card page.

![HoloLens buttons.](media/step-card-orientation-2.PNG "HoloLens buttons")

Here's what each button or UI element is used for.

| Number | UI element | Name | Purpose |
|---|---|---|---|
| 1 | ![Save button.](media/save-button.png "Save button") | Save | Save the guide. |
| 2 | ![Undo button.](media/undo-button.png "Undo button") | Undo | Undo the last change. You can undo up to 100 changes. |
| 3 | ![Redo button.](media/redo-button.png "Redo button") | Redo | Redo the last change. You can redo up to 100 changes. |
| 4 | ![Home button.](media/home-button.PNG "Home button") | Home | Select a different guide. |
| 5 | ![Follow Mode button](media/follow-button.PNG "Follow Mode button") | Follow mode | Have the Step card follow you, or lock it to a location.<p>[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] includes a feature that is called **Follow** mode. Wherever you look, the Step card follows your gaze. Therefore, you never have to worry where your instructions are. When you turn off **Follow** mode, the Step card stays where it is. You can move the Step card wherever you want at any time. Just grab it by using the navigation bar.</p> |
| 6 | ![Anchor button](media/anchor-button.PNG "Anchor button") | Anchor | Re-anchor (realign) your guide.<p>[!include[pn-hololens](../includes/pn-hololens.md)] can sometimes lose tracking. To fix this issue, you must re-anchor the guide by gazing at the anchor again.</p> |
| 7 | ![Settings button.](media/settings-button.PNG "Settings button") | Settings | Access the following setting:<ul><li>**Build number**. See the build that you're using.</li></ul> |
| 8 | ![Profile button.](media/profile-button.PNG "Profile button") | Profile | Sign in and out. |
| 9 | ![Outline button.](media/outline-button.png "Outline button") | Outline | Go to the **Outline** page.<p>You can use the **Outline** page to quickly move around your guide.</p> |
| 10 | ![Step counter.](media/step-progress.PNG "Step progress") | Step counter | See what step you're on in the task. |
| 11 | ![Task name.](media/task-name-hololens-app.PNG "Task name") | Task name | The name of the task you're on. |
| 12 | ![Gem button for dragging a dotted line.](media/gem.png "Gem button for dragging a dotted line") | Gem | By dragging the gem, you can create a dotted line to draw attention to a focus area. |
| 13 | (See the green rectangular area in the illustration.) | Bin | See the 3D parts (models) that can be added for the step. 3D parts include 3D objects from the 3D toolkit and any 3D models (computer-aided design \[CAD\] drawings) that you import to mimic 3D parts in your operator's real-world environment. |

> [!NOTE]
> Changes are automatically saved in the cloud as you author in [!include[pn-hololens](../includes/pn-hololens.md)]. Just be sure to select **Refresh** when you go back to the computer, to help guarantee that you have the latest version of the guide.

## Test the flow of your guide

After you're oriented on [!include[pn-hololens](../includes/pn-hololens.md)], we recommend that you go through your whole guide in **Operate** mode to see how it flows. As you step through your guide, make a note of things that you want to change in the PC app. For example, you might have to move some steps around, add tasks or steps, or add more supporting assets. In general, it's best to make these changes in the PC app before you start to place holograms, tethers, and styles.







    


## Change animation options

If your 3D model has animations, you can select a specific animation to play back. You can also configure playback options (speed, direction, and looping options). 

1. Select the 3D model.

2. On the **Edit** menu, select **Animation**.

    ![Animation command on the Edit menu](media/edit-animations1.PNG "Animation command on the Edit menu")
    
    You'll see the following **Animation** dialog box.

    ![Animation dialog box](media/animation-dialog.PNG "Animation dialog box")

3. In the **Animation** dialog box, select from the following options.

    |Option|Description|
    |----------------|---------------------------------------------------------------------|
    |**Animate**|Enable or disable the animation. You might want to use this option if an animation interferes with your ability to place a model in space. You can turn it off, and then turn it back on again. If disabled, the first or last frame of the animation is shown, depending on whether **Direction** is set to **Forward** or **Backward**.|
    |**Takes**|Select a specific animation to play from a 3D model that contains multiple animations.|
    |**Playback**|- If **Loop** is selected, the animation is repeated until the operator leaves the step.<br><br>- If **Once** is selected, the animation is played one time and then stops.<br><br>- If **Ping Pong** is selected, the animation repeats back and forth in each direction. |
    |**Direction**|- If **Forward** is selected, the animation runs from the first frame to the last frame of the animation as defined in the 3D model.<br><br>- If **Backward** is selected, the animation runs from the last frame to the first frame.|
    |**Speed**|Set the relative speed of the animation. For example, if the speed is set to 2.0x, the animation plays at twice the speed as defined in the model. |
    
> [!NOTE]
> For information on working with multiple animations in a single 3D model in 3DS Max, see [Use multiple animation clips in a 3DS Max model](https://doc.babylonjs.com/extensions/Exporters/3DSMax_to_glTF#single-animation-clip).
    
[!INCLUDE[footer-include](../includes/footer-banner.md)]
