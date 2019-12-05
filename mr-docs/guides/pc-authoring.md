---
author: Mamaylya
description: Everything you need to know about using the PC authoring application to create a guide in Dynamics 365 Guides.
ms.author: mamaylya
ms.date: 12/09/2019
ms.service: crm-online
ms.topic: article
title: Use the PC authoring application to create a guide in Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Author in the PC application for Dynamics 365 Guides

Watch videos on:

- [Dynamics 365 Guides overview](https://aka.ms/guidesoverview)
- [PC authoring](https://aka.ms/pcauthor)
- [HoloLens authoring](https://aka.ms/hololensauthor)

Use the PC authoring application in [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] to:

- Create a guide

- Choose an anchoring method

- Add tasks and steps

- Write the instructions for your steps

- Assign different types of content to support those steps. Supporting content includes:

  - 3D parts
  
  - 3D objects, such as objects from the 3D toolkit (arrows and numbers, for example)
  
  - 2D media (images and videos)
  
![PC authoring](media/pc-authoring.PNG "PC authoring")


## Install, open, and sign in to the PC application
Use these instructions to install the app (if it hasn't already been installed for you) and to sign in.

### Install the app 
1.	On your [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 PC, make sure you have the latest [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 build (10.0.16299 or later).

2.	Go to **Start** ![Start button](media/windows-button.png "Start button") > **[!include[cc-microsoft](../includes/cc-microsoft.md)] Store** ![Store button](media/store-button.png "Store button"), and then search for “[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)].”

3.  Select **Install** to download and install [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)].

### Sign in to the app
1.	Open the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] application from the **Start** menu on your PC. 

2.	In the **Welcome to Guides** screen, select **Sign in**.

    ![Welcome to Guides](media/welcome.PNG "Welcome to Guides")
    
3.	In the **Sign in** dialog box, select **Work or school account**, and then select **Continue**. 

4.	In the **Sign in** screen, enter the user account and password assigned to you by your organization. 

    ![Sign-in to the PC app](media/sign-in-pc.PNG "Sign in to the PC app")
 
5.	Select the instance you want to use if there’s more than one instance, and then select **Continue**.

    ![Choose an instance](media/choose-instance-pc.PNG "Choose an instance")

## Create a new guide

1.	Open the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] app.

2.	Select **Create new guide**.

     ![Create new guide](media/create-guide.PNG "Create new guide")

3.	Enter a name for the guide, and then select **Create**. If you’re planning to create multiple versions of the guide, you might want to add _v2, _v3, and so on as part of the name. 

     ![Name the guide](media/name-guide.PNG "Name the guide")
     
>[!NOTE]
>When you create a guide using the PC app, a JSON data file is automatically created in Common Data Service. This file is for internal use only. We don't recommend building functionality on top of this file because it may change over time. 

## Saving: how changes are synced between the PC app and HoloLens app

The PC authoring app and the [!include[pn-hololens](../includes/pn-hololens.md)] app are connected through the cloud, where your [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] files and content are stored. 
When you author a guide, all changes are saved on both the PC and [!include[pn-hololens](../includes/pn-hololens.md)]. This makes it easy to switch between devices. 
Autosave checks for changes every 4 seconds. You must be online to use [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]

> [!NOTE]
> When you switch from one device to the other, it's best to close the guide to make sure you don't lose any work. 

## Choose an anchoring method for your guide

The next step is to choose an anchoring method for your guide. Anchoring is a crucial step in creating a guide. It's how you tie your holograms to your real-world environment. If you don't anchor your guide properly, your holograms will be misaligned, and your operators will be confused and can even cause damage to machinery or parts. [Learn more about anchoring and how to create an anchor](anchor.md).

## Structure your guide in the Outline page

After you choose an anchoring method, you see the **Outline** page. This is where you create the framework for your guide by adding as many tasks and steps as you need. *Tasks* are groups of steps. *Steps* are the short, discrete work items that operators do to complete the task. Steps are the central building blocks in [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)].

When you open the **Outline** page for the first time, you'll see that a single task and step are already created for you. 

![Create a task and step](media/create-task-2.PNG "Create a task and step")
  
To get started, enter a task name, and then start typing the instructions for the first step in the box. When you need to add a new step, select **Add step**. When you’re ready to add another task, select **Add task**. It’s that simple!

In reality, you’ll probably create most of your steps from inside the Step card (see the next section), but the **Outline** page provides a great way to map out your guide at the start, or to get an overall picture of the guide after you’ve added all your tasks and steps. You can also restructure your guide from the **Outline** page by dragging tasks and steps.

In addition to tasks and steps, the **Outline** page shows:

- Customizable operator instructions.

- A special step called a Completion step that lets operators know when they’ve reached the end of the guide. The Completion step includes default text that you can customize as you see fit.

  ![Completion step](media/completion-step.PNG "Completion step")
 
### Best practices for the Outline page

- To provide overall context, add an Overview task at the start of the guide. This task would include just one step that describes what the guide is about. This is also a good place to list all the tasks that the guide covers. 

- Add a step at the beginning and end of each task to let the operator know when they’re starting something new or ending a task, and to make the operator feel successful when they complete a task.

- Don’t be afraid to add lots of steps, but remember to keep them short for best effect. 

- Consider adding steps that show individual tips and tricks. 

- When you move from the PC app to the HoloLens app, you'll be prompted to refresh. It's a good idea to close the guide you're working on when you switch devices. 

Here’s an example of a filled-out **Outline** page:

![Filled-out Outline page from Pylon wiring guide](media/finished-outline-page.png "Filled-out Outline page from Pylon wiring guide")
  
## Create steps and assign content in the Step card page

You can create steps on the **Outline** page, but you’ll probably create most of your steps from the WYSIWYG Step card page. The instructions you create on the Step card page match what the operator will see on [!include[pn-hololens](../includes/pn-hololens.md)].

In the Step card page, you write your instructional text and assign supporting content for that step, like 3D content or media (image or video). 

### Open the Step card page and add instructions

1. Select any step on the **Outline** page, or select **Step** in the left navigation. 

   ![Step command in left navigation](media/left-nav-step.PNG "Step command in left navigation")

2. Enter your instructional text in the rectangle in the middle of the Step card screen.

### Add 3D content or media to support a step 

1. On the right side of the screen, select the label for the type of item you want to add (**3D parts**, **Images**, **Videos**, or **3D toolkit**).

2. Drag the object to the appropriate box below the instructional text. For example, to add an image or video, drag the image or video to the **Image or video** box. To add a 3D part or an object from the 3D toolkit, drag it to one of the **3D parts** boxes. 

   ![Create a step with the Step card](media/drag-object.PNG "Create a step with the step card")

   > [!NOTE]
   > The collection of boxes below the instructional text is called the “bin.”
  
When you view your guide on [!include[pn-hololens](../includes/pn-hololens.md)] in Author mode, you’ll see all the content that you associated with the steps, and you can place the content in the relevant spaces in the real world. For example, if you assign a pointer to a step in the PC application, you’ll align that pointer to the thing you want to point to in [!include[pn-hololens](../includes/pn-hololens.md)] authoring in the real world. What you see in the Step card page is very similar to what you see on [!include[pn-hololens](../includes/pn-hololens.md)]. 

### Best practices for the Step card page

- It’s easy to add another step from the Step card page. Just select **Add new step** in the top right corner of the page. No need to go back to the **Outline** page. 

  ![Add new step button](media/add-new-step-button.PNG "Add new step button")

- Don’t be afraid to add lots of steps, but keep the text short. Instruction text is limited to 280 characters per step to help keep the text short.

- Try to stick to one type of content (image, video, or 3D object) per step. Too much media or 3D content can be overwhelming to the operator and too time-consuming to absorb. Think about what type of content gets the point across best.

- Write your guide in casual human language for best results. Don’t use technical jargon that people don’t know or understand.

- Use descriptive words like “locate,” “find,” “get,” “go to”, “pick up,” “put down,” “insert,” “attach,” and “remove.”

- Adding a **NOTE** step is useful for quality checks. This type of step can come before or after another step. Just make sure to put it in the right spot.

- Add a **WARNING** step for things that could be dangerous or cause a quality issue. When you move to Author mode on [!include[pn-hololens](../includes/pn-hololens.md)], you can add a style to reinforce the warning.

- Adding numbered small steps inside a step can sometimes help, but don’t be afraid to create separate steps for easier reading.

- When you’re done writing a step, be sure to move the cursor outside of the text box to activate AutoSave. 

### Import your own custom 3D objects<a name="import"></a>

You can import your own custom 3D objects to add to the **3D parts** library, and then assign parts to a step. 

To import your own 3D objects:

1.	Select the **Import** command in the upper-right corner of the Step card screen. 

2.	Locate the 3D object you want to import, and then select **Open**.

    ![Import custom 3D part](media/import-object.PNG "Import custom 3D part")
    
> [!NOTE]
> [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] supports glTF, GLB, FBX, STL, and PLY file formats. You can use a combination of third-party tools and the [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] to prepare your 3D (CAD) models, or you can use the Import Tool’s concierge service to have [!include[cc-microsoft](../includes/cc-microsoft.md)] convert and optimize the models for you. For more information about the Import Tool, see these topics:<br>- [Import Tool overview](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/index)<br>- [Optimize your 3D models](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/optimize-models)<br>- [Best practices for 3D models](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/best-practices)<br>- [Use Dynamics 365 Import Tool](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/import-tool)

### Add 3D objects from the 3D toolkit to support your steps

[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] comes with a library of predefined 3D objects included in the 3D toolkit that are optimized to work perfectly with [!include[pn-hololens](../includes/pn-hololens.md)]. Use objects from the 3D toolkit like any other content to support your steps and get your point across. Having a ready-made library makes it easy to get started if your company doesn’t have any 3D content.
 
The 3D toolkit includes markers, arrows, generic tools, hands, numbers, symbols, and zones. Here’s what the models look like:

![List of objects in 3D toolkit](media/3D-toolkit-objects.png "List of objects in 3D toolkit")

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
|Ctrl + Left, Right|Move to previous or next task or step, depending on what's selected|
|Ctrl + Up, Down|Move to above or below task or step, depending on what's selected|
|Win + Down|Minimize the current window|
|Win + Up|Maximize the current window|

> [!NOTE]
> Microsoft will continue to add support for screen readers, high contrast, and keyboard usability.

## Opt out of sending telemetry data to Microsoft

For privacy reasons, you can turn off the ability to send telemetry data to Microsoft. Microsoft uses this data to improve the product. Opting out prevents Microsoft from collecting any activity data.

To turn telemetry data off for the PC application:

1.  On the **File** menu, select **About**.

2. In the **About** dialog box, turn the **Send usage data** slider to off.

    ![Send usage data setting](media/send-usage-data-pc.PNG "Send usage data setting")
    
> [!NOTE]
> This option applies only to the device on which it's set. If you use [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] on more than one device, you need to modify the setting on those other devices. To turn this setting off for HoloLens, see [Author in the HoloLens application](hololens-authoring.md). Database administrators can also prevent usage data from showing in Power BI dashboards for Guides Analytics. For more information, see [Opting out of storing Dynamics 365 Guides events data in Common Data Service](data-opt-out.md).

## What's next?
After you create your guide on the PC, select an anchoring method, and create your tasks and steps, you’re ready to [test things out on HoloLens in a real-world environment, and place your holograms](hololens-authoring.md).

> [!IMPORTANT]
> When switching between PC and [!include[pn-hololens](../includes/pn-hololens.md)], be sure to select **Refresh** when starting work on a device to ensure that you have the latest version of the guide. 

Don’t worry if your guide isn’t perfect before switching to [!include[pn-hololens](../includes/pn-hololens.md)] authoring. You can always go back to the PC application to edit and restructure your guide. In fact, we’ve found it’s generally a good idea to do a quick test of the flow on [!include[pn-hololens](../includes/pn-hololens.md)], and then go back to the PC application to make changes before placing all your holograms in [!include[pn-hololens](../includes/pn-hololens.md)].

> [!TIP]
> If you’re creating multiple versions of the same guide, you might want to use the **Save a Copy** command on the **File** menu. This is great for guides that are similar but have a few different steps. You don’t have to start from scratch!

### See also

[Overview of authoring a guide](authoring-overview.md)<br>
[Choose an anchoring method for your guide](anchor.md)<br>
[Author in the HoloLens app](hololens-authoring.md)<br>
 
