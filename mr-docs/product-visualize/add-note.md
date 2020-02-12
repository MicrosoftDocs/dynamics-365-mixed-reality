---
author: mamithan
description: How to add a note (including text and drawings) to a 3D model in Dynamics 365 Product Visualize
ms.author: mamithan
ms.date: 01/29/2020
ms.service: crm-online
ms.topic: article
title: Add a note to your 3D model in Dynamics 365 Product Visualize
ms.reviewer: v-brycho
---

# Add a note to a 3D model in Dynamics 365 Product Visualize

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

You can capture notes while giving product demonstration, and add text or draw on the notes. You can also attach notes on specific points on a 3D model. For example, when you're in the field with a customer, you can capture any required product changes directly on the model. Any notes you create are saved in Common Data Service.

To review notes attached to a model, tap any spatial anchor on the model. Anchors on the front of the model appear as blue circles with white outlines. Anchors on the back appear as blurred circles with transparent outlines. For a model and note that's off the screen, a "note bubble" points in the direction of the model and note. See the table below for information about how these notes appear.

You can also browse through your notes by swiping the notes at the bottom of the screen. The corresponding spatial anchor is activated on the model as you swipe.

The following table shows how notes appear on the model, depending on where the note is located.

|Note on front of the model|Note on back of the model|Note and model off the screen|
|-------------------------------------|-------------------------------------------|-----------------------------------------|
|![Note on front of model](media/front-note.PNG "Note on front of the model")|![Note on back of model](media/back-note.PNG "Note on back of the model")|![Note and model off the screen](media/off-screen-note.PNG "Note and model off the screen")|

## Add a note

1.	Place the model as described in [Place and manipulate 3D models](manipulate-models.md), and then tap **Notes** on the right side of the screen.

    > [!div class=mx-imgBorder]
    > ![Notes button](media/notes-button.png "Notes button")

2. Tap **Add**.

    > [!div class=mx-imgBorder]
    > ![Tap Add Note](media/add-note.png "Tap Add Note")

3. To add a photo, tap **Attach image**.

    > [!div class=mx-imgBorder]
    > ![Tap Attach image](media/attach-image.png "Tap Attach image")
 
    a. Tap **Photo** to take a photo of the model, or tap **Camera Roll** if you want to use a photo already stored on your device.

    > [!div class=mx-imgBorder]
    > ![Tap Photo](media/camera-roll.png "Tap Capture")

    b. To draw on the screen, select a color and start drawing. For example, draw an arrow to call out a particular part of the model. Tap **Next**.

      > [!div class=mx-imgBorder]
      > ![Draw or add text](media/draw-add-text.png "Draw or add text")

      The captured image is displayed in the place of **Attach image** button. If you're not happy with the photo, tap **Remove** to remove the photo and then capture the photo again.

      > [!div class=mx-imgBorder]
      > ![Draw or add text](media/note-image-added.png "Draw or add text")
         
4. To add a message, tap **Type a message here**, and add the text.

    > [!div class=mx-imgBorder]
    > ![Tap Attach image](media/note-text.png "Tap Attach image")

5. To attach the note at a specific point in your model, tap **Pin to model**.

    > [!div class=mx-imgBorder]
    > ![Tap Pin to model](media/pin-to-model.png "Tap Pin to model")

    a. Tap the model where you want to attach the note, and then tap **Next**.
 
      > [!div class=mx-imgBorder]
      > ![Tap on the model](media/tap-on-product.png "Tap on the model")

      The note is attached at the tapped location on the model. If you want to remove the pin from the model, tap **Remove pin**.

      > [!div class=mx-imgBorder]
      > ![Remove pinned note](media/pin-added.png "Remove pinned note")

6. Tap **Finish**.
      

## View the notes attached to a model

1.	After placing the model, tap **Notes** on the right side of the screen.

2.	Tap a blue dot to open a specific note, or swipe right or left in the notes browser at the bottom of the screen to go forward or backward between notes.

    > [!NOTE]
    > If you want to see a larger view of the notes, which is useful if you can't see all the text in the notes card, tap the expand arrow in the upper-right corner of the notes card or flick up. Then you can use the scroll bar in the notes card to move through the text.
    
     ![Expand notes button](media/expand-notes.PNG "Expand notes button")
     
## Delete a note

1.	Tap **Notes** on the right side of the screen.

    > [!div class=mx-imgBorder]
    > ![Notes button](media/notes-button.png "Notes button")

2.	Navigate to the note you want to export, and tap the **Overflow** menu in the upper-right corner of the notes card.

    > [!div class=mx-imgBorder]
    > ![Navigate to the note](media/note-1.png "Navigate to the note")

3.	In the **Options** dialog box, tap **Delete Note**.

    > [!div class=mx-imgBorder]
    > ![Delete a note](media/delete-note.png "Delete a note")

4. Tap **Delete** in the confirmation dialog box.
  
## Export a note

You can export your notes to share them with other apps on your device that support the iOS sharing function. The notes image and text are exported without any special formatting.

To export a note:

1.	Tap **Notes** on the right side of the screen.

    > [!div class=mx-imgBorder]
    > ![Notes button](media/notes-button.png "Notes button")

2.	Navigate to the note you want to export, and tap the **Overflow** menu in the upper-right corner of the notes card.

    > [!div class=mx-imgBorder]
    > ![Navigate to the note](media/note.png "Navigate to the note")

3.	In the **Options** dialog box, tap **Export Note**.

    > [!div class=mx-imgBorder]
    > ![Export note](media/export-note.png "Export note")

4. Tap the required option for exporting the note.

    > [!div class=mx-imgBorder]
    > ![Export options](media/export-options.png "Export options")

## Change how your notes are shared with other apps

By default, your notes are saved to the SharePoint account associated with your Dynamics 365 Sales account. By default, Dynamics 365 Product Visualize also sends your notes to your Dynamics 365 Sales timeline and any connected Microsoft Teams channel.

To turn off sharing with the Dynamics 365 Sales timeline or Teams channels:

1. Tap the Main menu button ![Main menu](media/hamburger-icon.png "Main menu button"), and then select the account you're signed in to.  

2. Under **Note Output Options**, move the sliders to the off position for the options you want to turn off.

   ![Note Output Options](media/note-output-options.PNG "Note Output Options")

### See also

[Install, open, and sign in to the app](sign-in.md)<br>
[Place and manipulate 3D models](manipulate-models.md)<br>
[Show or hide layers in a 3D model](layers.md)<br>
[Explore sample 3D models](explore-samples.md)<br>
[View 3D models stored on your device](browse-models.md)<br>
[Add your own 3D model to an existing Dynamics 365 Sales product](add-model.md)<br>
[Download 3D models to use offline](download-models.md)
