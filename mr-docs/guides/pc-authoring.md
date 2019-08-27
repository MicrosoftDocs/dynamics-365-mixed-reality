---
author: Mamaylya
description: Everything you need to know about using the PC authoring application to create a guide in Dynamics 365 Guides (Preview).
ms.author: mamaylya
ms.date: 08/27/2019
ms.service: crm-online
ms.topic: article
title: Use the PC authoring application to create a guide in Dynamics 365 Guides (Preview)
ms.reviewer: v-brycho
---

# Use the PC authoring application to create a guide in Dynamics 365 Guides (Preview)

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]
 
Use the PC authoring application in [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides-preview](../includes/pn-dyn-365-guides-preview.md)] to:

- Create a guide

- Choose an anchoring method

- Add tasks and steps

- Write the instructions for your steps

- Assign different types of assets to support those steps. Supporting assets include:

  - 3D parts
  
  - 3D objects, such as objects from the 3D toolkit (arrows and numbers, for example)
  
  - 2D media (images and videos)

## Install, open, and sign in to the PC application
Use these instructions to install the app (if it hasn't already been installed for you) and to sign in.

### Install the app 
1.	On your [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 PC, make sure you have the latest [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 build (10.0.16299 or later).

2.	Go to **Start** ![Start button](media/windows-button.png "Start button") > **[!include[cc-microsoft](../includes/cc-microsoft.md)] Store** ![Store button](media/store-button.png "Store button"), and then search for “[!include[pn-dyn-365-guides-preview](../includes/pn-dyn-365-guides-preview.md)].”

3.  Select **Install** to download and install [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)].

### Sign in to the app
1.	Open the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] application from the **Start** menu on your PC. 

2.	In the **Welcome to Guides** screen, select **Sign in**.

    ![Welcome to Guides](media/welcome-to-guides.PNG "Welcome to Guides")
    
3.	In the **Sign in** dialog box, select **Work or school account**, and then select **Continue**. 

4.	In the **Sign in** screen, enter the user account and password assigned to you by your organization. If you’re the administrator, these are the credentials you created when you signed up for the preview.

    ![Sign-in to the PC app](media/sign-in-pc.PNG "Sign in to the PC app")
 
5.	Select the instance you want to use if there’s more than one instance, and then select **Continue**.

    ![Choose an instance](media/choose-instance-pc.PNG "Choose an instance")

## Create a new guide

1.	Open the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] app.

2.	Select **Create a new guide**.

3.	Enter a name for the guide. If you’re planning to create multiple versions of the guide, you might want to add _v2, _v3, and 
so on as part of the name. 

## Saving: how changes are synced between the PC app and HoloLens app

The PC authoring app and the [!include[pn-hololens](../includes/pn-hololens.md)] app are connected through the cloud, where your [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] files and assets are stored. 
When you author a guide, all changes are saved on both the PC and [!include[pn-hololens](../includes/pn-hololens.md)]. This makes it easy to switch between devices. 
Autosave checks for changes every 4 seconds. 

> [!IMPORTANT]
> For this preview release, there are a few things to be aware of when syncing devices:<br><br>- As a best practice, always select **Refresh** before making edits when you switch between devices. This ensures that you have the latest version of that file from the other device.<br><br>- If the same version of the guide is open on both the PC and [!include[pn-hololens](../includes/pn-hololens.md)], the app automatically refreshes when it detects that you've made a change in the other app. For example, if you have a guide open on [!include[pn-hololens](../includes/pn-hololens.md)] and add a new step in the PC app, the guide automatically refreshes on [!include[pn-hololens](../includes/pn-hololens.md)]. You might notice the refresh process.<br><br>- When you add text to the guide in the PC application, the auto publish feature activates only when you move the cursor outside the text box. If you add text to a step, keep your cursor in the text box, and then make a change on [!include[pn-hololens](../includes/pn-hololens.md)], or you’ll lose the text you created on the PC when 
it updates with the changes from [!include[pn-hololens](../includes/pn-hololens.md)]. This issue will be addressed in our next release. 

## Choose an anchoring method 

After you name your guide, you’ll see the **Outline** page and a prompt to create an anchor.

![Outline page with anchor prompt](media/outline-page.PNG "Outline page with anchor prompt")

- Select **Set your anchor now** to display the **Choose an anchor method** screen.

![Anchoring methods screen](media/choose-anchor-method.PNG "Anchoring methods screen")

### How anchoring works and types of anchors

Anchoring is used to spatially sync your instructions to the real world. When you anchor your guide, your instructions coincide 
with the space they live in and become meaningful. Your content is centered around this anchoring point.

There are two types of anchors:

- With a **printed anchor** (recommended), you attach a printed marker to a physical object in the real world. After creating the guide, 
to anchor the guide in the real world, you gaze at the marker using [!include[pn-hololens](../includes/pn-hololens.md)].

- With a **digital anchor**, you import a 3D representation (such as a CAD model or scanned model), and then lay that representation directly over a physical object in the real world. After creating the guide, to anchor it in the real world, 
you use a gesture.

**It’s extremely important to ensure that anchoring is correct and as precise as possible.** If anchoring is not correct, your 
instructions can cause operator confusion and potentially costly damage. For example, an operator could drill a hole in the wrong 
place or assemble the wrong part. 

Printed anchors provide more accuracy. You might want or need to use a digital anchor, however, for any of the 
following reasons:

- It might not be feasible to attach a printed anchor because the authoring is done in a location different than where the parts are located.

- It might not be feasible to attach a printed anchor due to moving parts.

- You can’t guarantee that the placement of the printed anchor will be the same every time.

- A part is too small to attach a printed anchor to.

### Anchor your guide by using a printed anchor

Using a printed anchor involves three basic steps:

1.	Print out a marker.

2.	Attach the marker to a physical object in the real world.

3.	Gaze at the marker to anchor the guide.

To print the marker:

1.  In the **Choose an anchor method** screen, in the **Printed Anchor** section, choose **Select**.

    ![Anchoring methods screen](media/choose-anchor-method.PNG "Anchoring methods screen")

2.  In the **Print and place the anchor** screen, select **Save to print** to save the marker.pdf file to your PC.

    ![Print and place the anchor screen](media/print-anchor.PNG "Print and place the anchor screen")

3.	Open the marker.pdf file on your PC in Adobe Acrobat Reader.

4.	On the **File** menu, select **Print**.

5.	Under **Page Sizing & Handling**, select the **Actual size** option.

    ![Print a marker](media/print-marker.PNG "Print a marker")

4.	Print the last page of the document on matte stock (glossy materials can affect scanning). 

5.	After printing, make sure the marker spacing matches the measurements shown in the following illustration:

    ![Marker spacing](media/marker-spacing.PNG "Marker spacing")
 
> [!NOTE]
> If the marker spacing is not within +/- 0.1 mm, select the **Custom Scale** option in the **Print** dialog box, and then change the 
percentage to compensate for the size discrepancy. For example, if you print the marker, and the result is 49 mm, you need to 
change the scale to 100.4% to get 49.196 mm, which would be within tolerance.<br>You might also need to adjust the hardware offset in Hololens 1 devices to ensure accurate placement of 3D content. [Learn more about adjusting for hardware offset](https://docs.microsoft.com/dynamics365/mixed-reality/guides/known-issues#uploading-new-3d-models-with-names-matching-any-of-the-pre-packaged-models-in-the-3d-toolkit-will-overwrite-the-files-in-the-3d-toolkit).

#### Best practices for printed anchors

Keep the following in mind when working with printed anchors:

- **Size.** Make sure that your printed anchor is the exact size indicated in this document. Incorrect anchor size causes guide misalignment. 

  - Some applications and printers might change the size of the image.
  
  - If the printed anchor is larger than indicated, [!include[pn-hololens](../includes/pn-hololens.md)] interprets the scale difference in distance. This causes the anchor to be identified as closer than it really is. 
  
  - Printing from the .pdf file (as described earlier in this topic) is the best way to ensure that the anchor is not resized. 
  
- **Location.** Place the anchor in a location on the physical object in a location that’s easy to access and out of the way.

  - Anchor placement should ideally be central to the steps being done.
  
  - Content placed farther away from the anchor will be less accurate.
  
  - Place the anchor where operators can quickly rescan to realign at any time.
  
  - Take a photo or video to document the anchor placement, and add it to the guide instructions to increase operator confidence. To capture a photo or video from [!include[pn-hololens](../includes/pn-hololens.md)], see [Mixed reality capture](https://docs.microsoft.com/windows/mixed-reality/mixed-reality-capture).
  
- **Scanning angle.** Make sure you’re facing the anchor straight on at the correct distance when gazing at it. 

  - Scanning from an angle can cause misalignment.
  
  - Ideal scanning range is from 60 to 80 cm.

#### How HoloLens establishes anchor position, scale, and orientation

When scanning, the forward-facing camera on [!include[pn-hololens](../includes/pn-hololens.md)] is used to measure the horizontal and vertical distances on the anchor. 
This information is combined with the actual anchor values stored internally in the application (49.2 mm and 32.8 mm, as indicated 
in the preceding illustration) to establish the anchor's precise position, scale, and orientation in space.

### Align your guide by using a digital anchor

Digital anchoring involves two basic steps:

1.	Using the PC authoring app, import a 3D representation of a physical object. This could be a CAD model used to create the physical object or a scanned model after fabrication. If you don't have a 3D representation, you can skip this step and use the preset 3D model included in [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)].

2.	Using [!include[pn-hololens](../includes/pn-hololens.md)] Author mode, place the 3D digital representation directly over a physical part.

To import a 3D representation: 

1.	Open the PC authoring app.

2.	On the right side of the screen, select the **Import** command. 

3.	In the **Open** dialog box, select the 3D representation that you want to use, and then select **Open**.

    This adds the 3D representation to the **3D parts** section of the library.
    
4.	In the library, select **3D parts**, and then drag your 3D representation to the digital anchor box. If you don't want to select a digital anchor at this time, select **Next**. The guide will be created with a preset 3D model that looks like this:

    ![Preset anchor](media/digital-anchor.PNG "Preset anchor")
   
> [!NOTE]
> It’s a good practice to take a photo or video of the base physical object and location and upload the photo or video to the 
**digital anchor** reference box. To capture a photo or video from [!include[pn-hololens](../includes/pn-hololens.md)], see [Mixed reality capture](https://docs.microsoft.com/windows/mixed-reality/mixed-reality-capture). You might also want to customize the instructions in the **Operator instructions** box to provide more specific directions.

When you switch to [!include[pn-hololens](../includes/pn-hololens.md)] authoring, you'll use a gesture to place the 3D representation directly over the physical object in your work environment.

#### Best practices for digital anchors

- **Size.** Select a digital anchor that’s not too small or too big. 

  - Medium-size digital objects are best. Very small or very large holograms are difficult to manipulate. 
  
  - Shoebox size or slightly larger is ideal.
  
- **Placement.** Choose a digital anchor that’s as close to the center of the work being done as possible. The farther you place digital content away from the digital anchor, the less accurate it becomes.

- **Shape.** Select a digital anchor that has a non-uniform or uncommon shape. Unusual shapes are easiest to align to.

  - Avoid objects that are mirrored. This can cause 180-degree misalignment.
  
  - Pick shapes that have clear edges and corners to help orient your content properly.
  
- **Recognizable.** Select a digital anchor that’s obvious, easily recognizable, and easy for the operator to find. Make sure that they can access the object without any obstructions.

- **Alignment direction.** Always align the digital anchor to your physical object from the same direction. This maximizes repeatability for operators.

  - Placement from different perspectives can cause misalignment.
  
  - Always look at it from multiple angles to ensure the digital anchor is aligned to the physical object.

### Ensure accuracy of anchors (alignment)
Independent from the method used for anchoring, these additional factors can impact the accuracy of the alignment and/or user perception of the alignment:

- **Interpupillary distance (IPD) setting.** The IPD is the distance between the center of the user’s pupils. It’s crucial to set the appropriate IPD to enable [!include[pn-hololens](../includes/pn-hololens.md)] to adapt its display because different users might have different IPDs. An incorrect IPD setting can result in a wrong perception of holograms in space as well as instability of holograms. [Use the HoloLens Calibration app to calibrate your IPD](https://docs.microsoft.com/en-us/windows/mixed-reality/calibration). 

- **Pre-scanning the environment.** [!include[pn-hololens](../includes/pn-hololens.md)] actively scans its environment for visible features  to create maps of its surroundings. This happens whenever the device is turned on and a user is signed in. It’s independent of whether you’re in the [!include[pn-hololens](../includes/pn-hololens.md)] shell or running apps. [!include[pn-hololens](../includes/pn-hololens.md)] constantly improves the accuracy of these maps as it scans the environment from different viewpoints and stores them on the device. Holograms are placed in relation to these maps. The more accurate the map, the more accurate the hologram placement.
Before using [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] on a [!include[pn-hololens](../includes/pn-hololens.md)] that’s unfamiliar with its environment, the user should put on the [!include[pn-hololens](../includes/pn-hololens.md)], sign into the device, and walk around the space where hologram instructions are placed or will be placed. This can be done while the user is in the [!include[pn-hololens](../includes/pn-hololens.md)] shell, but we recommend the user hide the **Start** menu to see the space as they walk around. Walking at a leisurely pace while slowly looking up and down will give the device the opportunity to find features and construct accurate maps. This is called "pre-scanning" because it’s done before you run [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. You only need to do this once for each environment because [!include[pn-hololens](../includes/pn-hololens.md)] stores the maps it created on the device and remembers the spaces it has scanned.

   Very dark or very bright environments, or environments that include very reflective surfaces (mirrors), dark surfaces, or featureless surfaces, cause a negative impact on [!include[pn-hololens](../includes/pn-hololens.md)]’s capability to recognize the space, which will impact hologram position and stability.

- **Impact of device positioning.** [!include[pn-hololens](../includes/pn-hololens.md)] uses a novel display technology to project images in the user’s field of view, which creates holograms. The way a user wears a device on their head has a huge impact on the perceived position of the holograms. 

   The best way to understand this is to adjust the device positioning while aligning holograms to their physical counterparts in [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. Observe how the alignment of holograms is affected when you shift the device left and right, up and down, and when you slide the display forward and backward. Users should wear the device in a consistent way and understand that subtle shifts in device positioning might not feel different but can lead to significant changes to perceived hologram locations.

## Structure your guide in the Outline page

After you choose an anchoring method, you see the **Outline** page. This is where you create the framework for your guide by adding as many tasks and steps as you need. *Tasks* are groups of steps. *Steps* are the short, discrete work items that operators do to complete the task. Steps are the central building blocks in [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)].

When you open the **Outline** page for the first time, you'll see that a single task and step are already created for you. 

![Create a task and step](media/task-name.PNG "Create a task and step")
  
To get started, enter a task name, and then start typing the instructions for the first step in the box. When you need to add a new step, select **Add step**. When you’re ready to add another task, select **Add task**. It’s that simple!

In reality, you’ll probably create most of your steps from inside the Step card (see the next section), but the **Outline** page provides a great way to map out your guide at the start, or to get an overall picture of the guide after you’ve added all your tasks and steps. You can also restructure your guide from the **Outline** page by dragging tasks and steps.

In addition to tasks and steps, the **Outline** page shows:

- Customizable operator instructions.

- A special step called a Completion step that lets operators know when they’ve reached the end of the guide. The Completion step includes default text that you can customize as you see fit.

  ![Outline page](media/completion-step.PNG "Outline page")
 
> [!NOTE]
> Whenever you start working on a guide, be sure to select **Refresh** to ensure you have the latest version. 

### Best practices for the Outline page

- To provide overall context, add an Overview task at the start of the guide. This task would include just one step that describes what the guide is about. This is also a good place to list all the tasks that the guide covers. 

- Add a step at the beginning and end of each task to let the operator know when they’re starting something new or ending a task, and to make the operator feel successful when they complete a task.

- Don’t be afraid to add lots of steps, but remember to keep them short for best effect. 

- Consider adding steps that show individual tips and tricks. 

- Remember to refresh your guide when moving between PC and [!include[pn-hololens](../includes/pn-hololens.md)], and be sure to move the cursor outside the text box when writing steps to activate AutoSave. 

Here’s the **Outline** page from the Example Guide to show what a completed **Outline** page looks like:

![Finished Outline page from Example guide](media/finished-outline-page.PNG "Finished Outline page from Example guide")
  
## Create steps and assign assets in the Step card page

You can create steps on the **Outline** page, but you’ll probably create most of your steps from the WYSIWYG Step card page.  

In the Step card page, you write your instructional text and assign supporting assets for that step, like 3D content or media (image or video). 

### Open the Step card page and add instructions

1. Double-click any step on the **Outline** page. 

2. Enter your instructional text in the black rectangle in the middle of the Step card screen.

### Add 3D content or media to support a step 

1. On the right side of the screen, select the label for the type of item you want to add (**3D parts**, **Images**, **Videos**, or **3D toolkit**).

2. Drag the object to the appropriate box below the instructional text. For example, to add an image or video, drag the image or video to the **Image or video** box. To add a 3D part or an object from the 3D toolkit, drag it to one of the **3D parts** boxes. 

   ![Create a step with the Step card](media/drag-object.PNG "Create a step with the step card")

   > [!NOTE]
   > The collection of boxes below the instructional text is called the “bin.”
  
When you view your guide on [!include[pn-hololens](../includes/pn-hololens.md)] in Author mode, you’ll see all the assets that you associated with the steps, and you can place the assets in their relevant spaces in the real world. For example, if you assign a pointer to a step in the PC application, you’ll align that pointer to the thing you want to point to in [!include[pn-hololens](../includes/pn-hololens.md)] authoring. What you see in the Step card page is very similar to what you see on [!include[pn-hololens](../includes/pn-hololens.md)]. 

### Best practices for the Step card page

- It’s easy to add another step from the Step card page. Just select **Add new step** in the lower-right corner of the page. No need to go back to the **Outline** page. 

- Don’t be afraid to add lots of steps, but keep the text short. Instruction text is limited to 280 characters per step to help keep the text short.

- Try to stick to one type of asset (image, video, or 3D object) per step. Too much media or 3D content can be overwhelming to the operator and too time-consuming to absorb. Think about what type of content gets the point across best.

- Write your guide in casual human language for best results. Don’t use technical jargon that people don’t know or understand.

- Use descriptive words like “locate,” “find,” “get,” “go to”, “pick up,” “put down,” “insert,” “attach,” and “remove.”

- Adding a **NOTE** step is useful for quality checks. This type of step can come before or after another step. Just make sure to put it in the right spot.

- Add a **WARNING** step for things that could be dangerous or cause a quality issue. When you move to Author mode on [!include[pn-hololens](../includes/pn-hololens.md)], you can add a style to reinforce the warning.

- Adding numbered small steps inside a step can sometimes help, but don’t be afraid to create separate steps for easier reading.

- When you’re done writing a step, be sure to move the cursor outside of the text box to activate AutoSave. 

### Import your own custom 3D objects to add to the 3D parts list<a name="import"></a>

You can import your own custom 3D objects to add to the **3D parts** list, and then assign parts to a step. 

To import your own 3D objects:

1.	Select the **Import** command in the upper-right corner of the Step card screen. 

2.	Locate the 3D object you want to import, and then select **Open**.

    ![Import custom 3D part](media/import-object.PNG "Import custom 3D part")
    
> [!NOTE]
> [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] supports glTF, GLB, and FBX file formats. You can use a combination of third-party tools and the [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] to prepare your 3D (CAD) models, or you can use the Import Tool’s concierge service to have [!include[cc-microsoft](../includes/cc-microsoft.md)] convert and optimize the models for you. For more information on the Import Tool, see these topics:<br>- [Import Tool overview](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/index)<br>- [Optimize your 3D models](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/optimize-models)<br>- [Best practices for 3D models](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/best-practices)<br>- [Use Dynamics 365 Import Tool](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/import-tool)

### Add 3D objects from the 3D toolkit to support your steps

[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] comes with a library of predefined 3D objects included in the 3D toolkit that are optimized to work perfectly with [!include[pn-hololens](../includes/pn-hololens.md)]. Use objects from the 3D toolkit like any other asset to support your steps and get your point across. Having a ready-made library makes it easy to get started if your company doesn’t have any 3D content.

![Add object from 3D toolkit](media/3d-toolkit.PNG "Add object from 3D toolkit")
 
The 3D toolkit includes markers, arrows, generic tools, hands, numbers, symbols, and zones. Here’s what the models look like:

![List of objects in 3D toolkit](media/3D-toolkit-objects.PNG "List of objects in 3D toolkit")

You add a 3D object from the 3D toolkit in the Step card page, and then place it in [!include[pn-hololens](../includes/pn-hololens.md)] Author mode. You can use the same object (instance) as many times as you like in a step.

> [!NOTE]
> You can also add 3D objects from the 3D toolkit in [!include[pn-hololens](../includes/pn-hololens.md)] authoring. You don't have to add them on the PC if you prefer to do it in [!include[pn-hololens](../includes/pn-hololens.md)] authoring.

To add an object from the 3D toolkit:

1. Select the **3D toolkit** tab.

2.	Select the appropriate category of objects.
    
3.	Drag the object you want from the list to a **3D parts** box below the Step card.

    ![Drag object from 3D toolkit](media/3d-part.PNG "Drag object from 3D toolkit")
 
### Best practices for 3D toolkit

- Use pointers to communicate simple spatial information like position, direction, and translation.

- Use the arrow when you want the operator to insert a part into something stationary (hand tightening a bolt into a tapped hole, for example). 

- Use one of the hand poses when you want the operator to use their hand in a specific way to influence or manipulate something. There are various poses for specific interactions such as Pull, Push, Pinch, Grab, and others. Combine these standards with arrows and/or icons to add additional meaning.

- Adjust the size of the pointer, but never go below 1 cm. Otherwise, it can cause errors.

## Keyboard shortcuts

You can use any of the following keyboard shortcuts in the PC application:

|Keyboard shortcut|Action|
|---------|-------------------------------------------------|
|Ctrl + S|Save the current guide|
|Ctrl + C|Copy|
|Ctrl + V|Paste|
|Ctrl + X|Cut|
|Ctrl + A|Select All|
|Ctrl + Z|Undo the last change to the guide|
|Ctrl + Y|Redo the last change to the guide|
|Ctrl + F4|Close the current window|
|Win + Down|Minimize the current window|
|Win + Up|Maximize the current window|

## What's next?
After you create your guide, select an anchoring method, and create your tasks and steps, you’re ready to [test things out on HoloLens in a real-world environment, and place your holograms](hololens-authoring.md).

> [!IMPORTANT]
> When switching between PC and [!include[pn-hololens](../includes/pn-hololens.md)], be sure to select **Refresh** when starting work on a device to ensure that you have the latest version of the guide. 

Don’t worry if your guide isn’t perfect before switching to [!include[pn-hololens](../includes/pn-hololens.md)] authoring. You can always go back to the PC application to edit and restructure your guide. In fact, we’ve found it’s generally a good idea to do a quick test of the flow on [!include[pn-hololens](../includes/pn-hololens.md)], and then go back to the PC application to make changes before placing all your holograms in [!include[pn-hololens](../includes/pn-hololens.md)].

> [!TIP]
> If you’re creating multiple versions of the same guide, you might want to use the **Save a Copy** command on the **File** menu. This is great for guides that are similar but have a few different steps. You don’t have to start from scratch!

### See also

[Overview of authoring a guide](authoring-overview.md)<br>
[Test your guide and place holograms in the HoloLens app](hololens-authoring.md)<br>
 
