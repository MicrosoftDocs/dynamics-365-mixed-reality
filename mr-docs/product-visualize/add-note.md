---
author: mamithan
description: How to add a note (including text and drawings) to a 3D model in Dynamics 365 Product Visualize
ms.author: mamithan
ms.date: 10/30/2019
ms.service: crm-online
ms.topic: article
title: Add a note to your 3D model in Dynamics 365 Product Visualize
ms.reviewer: v-brycho
---

# Add a note to your 3D model in Dynamics 365 Product Visualize

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

You can capture notes on specific points on a 3D model in Microsoft Dynamics 365 Product Visualize, and even add text or draw on the notes. For example, when you’re in the field with a customer, capture any required product changes directly on the model. 

To add a note, you tap the location of the model where you want to add the note, and then take a picture of the model or upload a picture from your photo library to set the context. Then you can draw on the image or add comments. Notes you create are saved in the Common Data Service.

To review notes you have made on your model, you can tap any spatial anchor on the model. Anchors on the front of the model appear as blue circles with white outlines. Anchors on the back appear as blurred circles with transparent outlines. You can also browse through your notes by swiping the notes cards at the bottom of the screen. The corresponding spatial anchor activates on the model as you swipe. 

![Types of notes](media/types-of-notes.PNG "Types of notes")

## Add a note

1.	After placing a model, select **Notes** on the right side of the screen.

    ![Select Notes item](media/select-notes.PNG "Select Notes item")
 
2.	Select **Add**.

    ![Select Add Note](media/add-note.PNG "Select Add Note")
 
3.	Tap the model where you want to place the note. 

    ![Tap the model](media/tap-on-product.PNG "Tap the model")
 
4.	Do one of the following:

    -	To take a picture, select **Capture** on the right side of the screen. The app takes a picture of the model.
    
    -	To use a picture from your camera roll, select **Camera Roll**, and then select the picture you want.
    
        ![Picture choices](media/take-photo.PNG "Picture choices")
   
5.	In the **Create Note** screen:

    a. Do the following: 
    
      - To draw on the screen, select a color and start drawing. For example, draw an arrow to call out a particular part of the model.
    
      - To add text, tap the box at the bottom of the screen, and then enter the text you want.
    
         ![Add text](media/add-text.PNG "Add text")
      
    b. Select **Submit** to add your note.
 
      > [!NOTE]
      > If you’re not happy with the picture, select **Replace** to redo the capture or select a different picture from your camera roll. When you select **Replace**, any text you entered is retained, but any drawings are lost.    

## View the notes attached to a model

1.	After placing the model, select **Notes** on the right side of the screen.

    ![Select Notes item](media/select-notes.PNG "Select Notes item") 

2.	Tap a blue dot to open a specific note, or swipe right or left in the notes browser at the bottom of the screen to go forward or backward between notes.

    > [!NOTE]
    > If you want to see a larger view of the notes, which is useful if you can’t see all the text in the notes card, tap the expand arrow in the upper-right corner of the notes card or flick up. Then you can use the scroll bar in the notes card to scroll the text. 
    
     ![Expand notes button](media/expand-notes.PNG "Expand notes button")
     
## Edit or delete a note

1.	Select **Notes** on the right side of the screen.

2.	Select the **Overflow** menu ![Overflow menu button](media/overflow-button.png "Overflow menu button") in the upper-right corner of the notes card.

3.	In the **Options** dialog box, select **Edit note** or **Delete note**.

     ![Edit or delete a note](media/share-status.PNG "Edit or delete a note")
  
## Change how your notes are shared with other apps

By default, your notes are saved to the SharePoint account associated with your Dynamics 365 Sales account. By default, Dynamics 365 Product Visualize also sends your notes to your Dynamics 365 Sales timeline and any connected Microsoft Teams channel. 

To turn off sharing with the Dynamics 365 Sales timeline or Microsoft Teams channels:

1. Select the Main menu button ![Main menu](media/hamburger-icon.png "Main menu button"), and then select the account you're signed in to.

   ![Edit account settings](media/edit-account-settings.PNG "Edit account settings")

2. Under **Note Output Options**, move the sliders to the off position for the options you want to turn off.
 
## Export a note

You can export your notes to share them with other apps on your device that support the iOS sharing function. The notes image and text are exported without any special formatting.

To export a note:

1.	Select **Notes** on the right side of the screen.

2.	Select the **Overflow** menu ![Overflow menu button](media/overflow-button.png "Overflow menu button") in the upper-right corner of the notes card.

3.	In the **Options** dialog box, select **Export note**.   


### See also

[Install, open, and sign in to the app](sign-in.md)<br>
[Place and manipulate 3D models](manipulate-models.md)<br>
[View layers of your 3D model](layers.md)<br>
[Explore sample 3D models](explore-samples.md)<br>
[View 3D models stored on your device](browse-models.md)
