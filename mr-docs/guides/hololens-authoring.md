---
author: anhaman
description: Test and place holograms using the HoloLens application in Author mode (Dynamics 365 Guides)
ms.author: anhaman
ms.date: 02/24/2019
ms.service: crm-online
ms.topic: article
title: Test and place holograms using HoloLens Author mode (Dynamics 365 Guides)
ms.reviewer: v-brycho
---

# Test and place holograms using HoloLens Author mode

The second major step in creating a guide in Microsoft Dynamics 365 Guides takes place on the HoloLens application. In HoloLens Authoring mode, you:

1.	Align your guide to a marker or a digital twin, depending on the type of alignment you chose in the PC application.
2.	Test the flow of your guide.
3.	Add holographic tethers to visually tie your steps to physical objects in the real world.
4.	Place your holographic 3D content in their relevant spaces in the real world.
5.	Add styles (optional) to 3D content to add treatments such as a warning or caution.

    ![Test your guide)](media/test-guide.PNG "Test your guide")

## Install the HoloLens app
If you haven’t already installed the HoloLens app on your HoloLens device, you can install it from the Microsoft Store for Consumers.

### Install the HoloLens app.
1.	Make sure you have HoloLens build 10.0.14393.0 or later installed on your HoloLens. Build 10.0.14393.0 is the minimum that supports Guides. We recommend updating to newer versions when available. See [Manage updates to HoloLens](https://docs.microsoft.com/en-us/HoloLens/hololens-updates) for instructions on using Windows Update for Business.
2.	On your HoloLens, use the bloom gesture to open the Home menu, and then open the Microsoft Store app and search for “Guides”.
3.	Select **Install** to download and install the Guides application.

### Sign in to the HoloLens app
If you sign in with a brand new HoloLens device, you’ll be prompted to walk through the Setup wizard. In the Setup wizard, you can sign in with an existing account or create a new one, depending on the version of Windows that you’re running. The Setup wizard will also walk you through steps to calibrate and prepare your HoloLens for use.

#### Calibrate your HoloLens
When placing holograms, it’s crucial to ensure the alignment is as close as possible. You can’t place holograms accurately if your HoloLens isn’t calibrated. Calibration is also recommended to improve the quality of the visuals or to calibrate visuals for a new user. **It’s particularly important for authors to ensure that their IPD is set correctly. Otherwise, all operators using the guide will see misaligned holograms.**

You can use the Calibration app that comes with HoloLens to set your IPD and ensure proper device fit. 

To set your IPD using the Calibration app:
1.	Do the bloom gesture to launch the Start menu.
2.	Air tap on Calibration to begin calibrating your HoloLens.

    ![Calibrate your HoloLens)](media/calibrate-hololens.PNG "Calibrate your HoloLens")

3.	Follow the instructions on your HoloLens.

> [!TIP]
> If you’re sharing a HoloLens device, learn about how you use the Windows Device Portal to avoid having to re-calibrate the HoloLens each time you switch users. 
 
### Open and sign in to HoloLens for the first time
After ensuring that your HoloLens is correctly calibrated, you can open the HoloLens application.
1.	Go to **Apps**.

    ![HoloLens Apps selection)](media/hololens-apps.PNG "HoloLens Apps selection")

2.	Select the down arrow.

    ![HoloLens down arrow highlighted)](media/hololens-down-arrow.PNG "HoloLens down arrow highlighted")

3.	Launch the Guides application.

    ![Launch Guides)](media/launch-guides.PNG "Launch 'Guides")
 
4.	On the welcome screen select Sign in. 
5.	In the **Email and accounts** screen, select **Work or school account**, and then select **Continue**. 
6.	In the Work or school screen, enter the email address sent to you by your organization. If you’re the administrator, use the credentials you created for the Trial subscription. 

    ![Sign in to HoloLens)](media/sign-in-hololens.PNG "Sign in to HoloLens")
 
7.	Select an instance to use if you have more than one instance, and then select **Continue**.
8.	In the **Select Mode** dialog box, gaze at the box to the right of **Author** until the box fills, which selects that item. 

    ![Select Author mode)](media/author-mode.PNG "Select Author mode")

## Align your guide
The first thing you see when you open a guide is the alignment instructions you created in the PC Authoring application. The screen shot below shows the operating instructions created for the Example Guide that comes with Dynamics 365 Guides.

![HoloLens alignment instructions)](media/hololens-alignment.PNG "HoloLens alignment instructions")

If you chose Marker alignment as the alignment method for the guide, the next step is to align the marker hologram with the printed marker you placed in the real-world environment. The marker hologram looks like this:

![Holographic marker image)](media/marker-holograph.PNG "Holographic marker image")
  
After aligning the guide, you’ll see the **Marker found** screen. Select the **Confirm** button to continue. 

![Marker found holograph)](media/marker-found.PNG "Marker found holograph")
   
> [!NOTE]
> If you chose Manual alignment as the alignment method for the guide, you’d align the hologram that matches the digital 3D representation that you placed in your real-world environment.

When you align your guide, the alignment information is stored on your HoloLens so you don’t have to realign the guide every time you open it. You can realign a guide at any time though if you feel the holograms are out of alignment. For more information, read about the **Alignment** button in the next section.

## Get oriented on HoloLens
After you align your guide, you’ll see the Step card. The Step card is the hub of everything you do with your guide and how you navigate in the app. The Step card is also what your operator will see when they use the guide. The Step card tags along with the operator to keep the instructions where they need them as they move around their work space.

Navigate through the guide by gazing at the **Next Step** and **Go Back** arrows. You can also use gestures such as air tap to navigate through a guide. 

At the top of the Step card screen, you’ll see three holographic buttons: **Undo**, **Redo**, and **Save**.

![HoloLens step card screen)](media/hololens-orientation.PNG "HoloLens step card screen")
 
The **Undo** and **Redo** buttons work like **Undo** and **Redo** in any Microsoft Office program. There’s no limit to the number of times you can undo or redo. 

> [!NOTE]
> Changes are automatically saved as you author in HoloLens. Just be sure to select **Refresh** when you go back to the PC to ensure that you have the latest version of the guide.

The Step card also includes several other buttons and UI elements:

![HoloLens buttons)](media/hololens-buttons.PNG "HoloLens buttons")
 
Here’s what each button or UI element is used for:

|Button|Name|Purpose|
|-----|------------|----------------------------------------------------------------------------------------------------------------|
|![Home button)](media/home-button.png "Home button")|Home|Choose a different guide|
|![Profile button)](media/profile-button.png "Profile button")|Profile|Sign in and out|
|![Settings button)](media/settings-button.png "Settings button")|Settings|Access the following settings:</br><br>- **Fit box**. Use to make sure you’re wearing the HoloLens device correctly.</br><br>- **Noise Cancellation**.</br><br>- **Dynamic Volume**. Adjusts the volume dynamically based on noise in the environment. For example, if the environment is very noisy, the volume adjusts upward automatically.</br><br>- **Build number**. Shows the build you’re using.|
|![Alignment button)](media/alignment-button.png "Alignment button")|Alignment|Realign your guide.|HoloLens can sometimes lose tracking. To fix this, you’ll need to realign the guide by gazing at the marker or digital twin again.|
|![Pin button)](media/pin-button.png "Pin button")|Pin|Lock the step card to a location.|Guides includes a feature called “tag-along.” Wherever you look, the Step card follows your gaze so you never have to worry where your instructions are. When you pin the step card, you turn off the tag-along feature. When tag-along is off, you can just grab the card and move it wherever you like.|
|![Outline button)](media/outline-button.png "Outline button")|Outline|Go to the Outline page.|Use the Outline page to quickly navigate around your guide.|
|![Task progress)](media/task-progress.PNG "Task progress")|Task Progress	|Shows where you are in the open task.|
|![Media button)](media/media-button.png "Media button")|Media|This button shows that there’s a video or image attached to a step. The image or video opens automatically when the operator goes to the step. If they want to close the image or video, they can select the button.|

## Test the flow of your guide
Once you’re oriented on HoloLens, we recommend that you go through your whole guide to see how it flows. As you step through your guide, make note of things you want to change in the PC application. For example, you may need to move some steps around, add tasks or steps, or add more supporting assets. It’s generally best to make these changes in the PC application before you start placing holograms, tethers, and styles.

When you’re ready to make the changes in the PC application, **make sure to close the HoloLens app** before re-opening the PC app. Don’t keep both applications open at the same. 

## Place your holograms
You’ve tested the flow of your guide and you’ve made changes in the PC application. Now you’re ready to move to the next stage of the authoring process—you’re ready to place your holograms. 

In this stage of the process, you’ll walk through each step in your guide and place any assets that you associated with that step when you authored it in the PC application. For example, if you added a 3D part to support a step, you’ll place that part over its physical counterpart in the real world. If you added a 3D object from the 3D toolkit (an arrow or a number, for example), you’ll place that object in an appropriate place in the real world to draw the user’s focus. You can place the same 3D part or 3D object as many times as you want.

You don’t need to do anything to place images or videos associated with a step. They automatically appear when the operator goes to the step. They can select the **Media** button to close the image or video.

The 3D assets associated with each step appear below the Step card:

![3D assets below Step card)](media/place-holograms.PNG "3D assets below Step card")
 
To place them in the real world: 
1.	Air tap an empty box under **3D parts**.
2.	Air tap a category in the 3D toolkit (an arrow or hand, for example).

    ![Air tap a category)](media/airtap-category.PNG "Airtap a category")

3.	Air tap the object you want to add.
    This item will be added to your bin.
    
    ![3D object in bin)](media/object-in-bin.PNG "3D object in bin")


### Manipulating holograms
To place a hologram from one of your bins:
1.	Air tap a 3D asset to add it to your real world. It will appear in your world in front of the Step card.
2.	Raise your hand to the ready gesture and gaze at the 3D asset to select it. You can tell if it’s selected if the 3D selection sphere appears around it.
3.	Once the object is selected, air tap + hold anywhere on the selection sphere to pick up the 3D asset.
4.	Do one of the following to move the hologram:
    - To move it larger distances in any direction, move your hand quickly in the direction you want. By default, the hologram will move approximately the same distance your hand moves from the starting point of where you “grabbed” the hologram to where you stop. 
    - To make more precise adjustments, move your hand slowly or keep it stationary to enter precision mode. This slows down the movement speed so you can nudge the hologram where you want it.

>[!Tip]  
> You’ll know you’ve entered precision mode when the selection sphere turns blue.

![Hologram selection sphere)](media/hologram-selection-sphere.PNG "Hologram selection sphere")

 
#### Rotate a hologram
It’s unlikely an asset will be at the correct orientation when you initially place or move it. Use the rotation adjustment knobs to rotate it the way you want.

To rotate a hologram:
- Air tap and hold on a rotation adjustment, and then do one of the following:
  - Use the up/down knob to rotate vertically.
  - Use the left/right knob to rotate horizontally.
  - Use the free-hand knob to rotate in any direction.

>[!Tip]
> Gazing at any of the gizmo knobs will let you know which direction the knob will rotate.

When rotating, it helps to think as if you are physically grabbing the knob and rotating around the object, like a wheel.
The following screen shots show how to use the different rotation knobs:

![Hologram manipulation)](media/hologram-manipulation.PNG "Hologram manipulation")
 
> [!Important]
> To manipulate holograms effectively, make sure that your HoloLens is calibrated properly. 

### Best practices for working with 3D content
- Make sure that the 3D content is not in the way of the operator doing the task. 
- Keep the field of view in mind when placing assets. If you put a hologram behind someone, it will be very hard to find. 
- Use 3D content sparingly and with a clear goal. Too much content can clutter the instructions and make it harder to follow.
- Remember that you can attach a tether to 3D content to make it more discoverable. See the next section to learn about tethers.

## Place tethers
You’ll typically place a tether for each Step card when you place your holograms. A tether visually links a Step card to the area where the operator needs to focus. It helps the operator find the content or understand what they’re supposed to be looking at in the real world. 

![Holographic tether)](media/hographic-tether.PNG "Holographic tether")

To place a tether:
1.	Tap and hold the “tether ball” below the Step card.
2.	Place it in the real-world location that you want.

    ![Place a tether)](media/place-tether.PNG "Place a tether")

### Best practices for tethers
- Tether placement isn’t exact, so if you’re connecting a tether to a 3D object from the 3d toolkit, place the tether in the general area, and then place the 3D object (a number, for example) at the end of the tether. 
- To make a tether appear to be more precise, use a 3D object like a circle or arrow to show exactly where the tether is pointing.

## Add styles for emphasis
Use styles to provide visual cues for extra emphasis. For example, add the Warning style to show caution or the Avoid style to make sure an operator doesn’t do something that could cause harm. As your operators get used to the visual language provided by styles, it will speed up their learning process.

> [!Note]
> At this time, you can’t add styles from the PC application. They exist only in HoloLens. 

To place a style:
1.	Air tap a hologram you’ve already placed in the real world to select it.
2.	Air tap the **Edit Hologram** (. . .) button.

    ![Edit hologram button)](media/edit-hologram-button.PNG "Edit hologram button")

3.	Air tap **Styles**. 

    ![Edit styles)](media/edit-styles.PNG "Edit styles")
 
4.	Select the style you want to use.

    ![List of styles)](media/styles-list.PNG "List of styles")
 
Here’s a list of styles included in Guides and when to use each:

|Style	|Purpose	|How it appears to the operator|
|---------------|-------------------|--------------------------------------------|
|Original|Restore to original appearance	|Default appearance|
|Pick up	|Tell the operator to pick up something	|Outline|
|Place	|Show the operator where to place something	|Dotted line|
|See-through 1	|Show something without obscuring the operator’s view	|Transparent 50%|
|See-through 2	|Layer one thing on top of another so the operator can see through two layers	|More transparent 25%|
|Warning	|Warn about a safety or quality concern	|Yellow and black striped|
|Avoid	|Show areas or things to avoid	|Red flashing|
|X-ray	|Show things that happen inside something	|Outline with transparent inside|
|Metal	|Provide a realistic metal finish for an object	|Metallic|

![All styles)](media/all-styles.PNG "All styles")
 
### Best practices for styles
- Use style to reinforce actions.
- Use styles only for the purpose they were intended. When operators learn the visual language of styles, they’ll know that a particular style means a certain thing, which will speed up the learning process. 

## What's next?

To learn more about Dynamics 365 Guides, here are some helpful links:

- [Use a guide as an operator](operator-guide.md)
- [Analyze your guides to improve efficiences](analytics-guide.md)
- [FAQ](faq.md)

To learn more about Microsoft mixed reality apps and HoloLens, here are some helpful links: 

- [What is mixed reality](https://docs.microsoft.com/en-us/windows/mixed-reality/mixed-reality)?
- [Microsoft Dynamics 365 Layout](https://dynamics.microsoft.com/en-us/mixed-reality/layout/)
- [Microsoft Dynamics 365 Remote Assist](https://dynamics.microsoft.com/en-us/mixed-reality/remote-assist/)
- [Connect to Wi-Fi on HoloLens](https://docs.microsoft.com/en-us/windows/mixed-reality/connecting-to-wi-fi-on-hololens)
- [Calibrate your HoloLens](https://docs.microsoft.com/en-us/windows/mixed-reality/calibration)
- [Using the Windows Device Portal](https://docs.microsoft.com/en-us/windows/mixed-reality/using-the-windows-device-portal)
