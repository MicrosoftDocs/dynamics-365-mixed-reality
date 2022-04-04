---
title: Voice commands and gestures for Dynamics 365 Remote Assist on HoloLens
author: amaraanigbo
description: Learn about voice commands and gestures for Microsoft Dynamics 365 Remote Assist on HoloLens.
ms.author: soanigbo
ms.date: 04/04/2022
ms.topic: article
ms.reviewer: v-bholmes
---

# Voice commands and gestures for Dynamics 365 Remote Assist on HoloLens

You can navigate Dynamics 365 Remote Assist on HoloLens and HoloLens 2 using voice commands and gaze instead of gestures. Some voice commands are contextual, so they only work in particular areas of the user interface. For example, “Start inking” only works if the **Draw** tool is already active. You can also gaze at any button and say “Select.”

At this time, voice commands and speech recognition are [available in specific languages for Hololens](./faq-hololens.md).

When you’re in a call, a good way to learn the features of Dynamics 365 Remote Assist is to say, “Remote Assist” without saying a follow-up command. The app displays what it believes you said by showing a check mark and “Remote assist.” Then the app displays the name of each button. After a few seconds, the labels automatically disappear. 

When you’re outside a call (for example, before you’ve picked up, or when you’re looking at a list of contacts but have not called anyone), you can also say “Remote Assist” to remind yourself of the voice command for each button you see. The labels will pop up for a few seconds, and then disappear. However, you won't receive confirmation of your voice command. 

## Voice commands

The table below provides the full list of voice commands that you can use with Dynamics 365 Remote Assist on HoloLens. 

To use a voice command, say “Remote Assist”, and then say one of the voice commands. For example, say "Remote Assist, Move" to enter Move mode for a window. You can also gaze at any button and say “Remote Assist, Select” to select that button.

|Voice command|Description |
| ------------- | -----|
|**General**| | 
|Remote Assist|If you say “Remote Assist” without following it with a command, displays labels with the name of each button. After a few seconds, the labels automatically disappear.| 
|Start listening|Put Dynamics 365 Remote Assist into state expecting a list of commands to follow.|
|Stop listening|Remove Dynamics 365 Remote Assist from state expecting a list of commands to follow.|
|Next|Go to next page.|
|Cancel|Close a dialog box without taking any action.|
|Undo|Undo the previous action.|
|**Call management**  | | 
|Call|Call a contact.|
|Launch call|Launch a call from the calling confirmation dialog box.|
|Search|Display the **Search** box to search for a contact.|
|Retry|Retry searching the **Contacts** list.|
|Video|Answer an incoming call with video.|
|Audio|Answer an incoming call with audio only.|
|Hang up|End a call (including ending a ringing outgoing call).|
|Mute|Mute an audio call.|
|Unmute|Unmute an audio call.|
|Record call |Start video recording.|
|Stop recording|Stop video recording. |
|Camera| Selects the camera/capture tool.|
|Start video|Turn on the video for a call.|
|Stop video|Stop the video for a call.|
|Turn on snapshot|Turn on Snapshot mode for a call in low-bandwidth mode.|
|Turn off snapshot|Turn off Snapshot mode for a call in low-bandwidth mode.|
|Take a snapshot|Take a snapshot when the Snapshot dialog box appears for low-bandwidth mode.|
|Join meeting|Join a Microsoft Teams meeting.|
|Open participants|Open the participants list.|
|Invite|Confirm inviting a participant to join a call.|
|Close participants|Close the participants list.|
|Next meeting|Show the next meeting notification.|
|Previous meeting|Show the previous meeting notification.|
|Narrator on|Turn the narrator on to have HoloLens announce the name of an incoming caller.|
|Narrator off|Turn off the narrator.|
|Dictation|Turn on dictation for text input in a chat.|
|**Window management**  | | 
|Select slate| Select the window you're currently gazing at so you can move or resize it.|
|Move|Select the **Move** tool to move a window.|
|Accept|Accept the placement of a moved window.|
|There|Accept movement of the slate, and lock it to this location.|
|Place here|Place the slate at specific location.|
|Cancel|Cancel placement of a moved window.|
|Reset|Reset the window to the previous placement.|
|Scale|Select the **Scale** tool to resize a window (PDF document, for example). It does not resize an annotation or ink.|
|Scale off|Turn off the **Scale** tool.|
|Bigger|When the **Scale** tool is active, make the current window bigger.|
|Smaller|When the **Scale** tool is active, make the current window smaller.|
|Close|Close the open window.|
|Pin|Pin a window in your space so it doesn’t follow you as you move around in your environment.|
|Unpin|Unpin a window so it follows you as you move around in your environment.|
|Follow me|Set the panels to follow the user.|
|Dock|Dock the text chat during a call.|
|Undock|Undock the text chat during a call.|
|Open chat|Open the **Text Chat** window (attached to the video feed).|
|Close chat|Close the **Text Chat** window.|
|**Annotations**    | | 
|Arrow|Select the **Arrow** tool to create a holographic arrow. Use arrows to point to parts of your environment. |
|Arrow off|Turn off the **Arrow** tool.|
|Arrow|Place an arrow at the current gaze cursor location.|
|Ink|Select the **Draw** tool to draw on the walls and surfaces of your environment.|
|Ink off|Turn off the **Draw** tool.|
|Start inking| Start adding ink.  |   
|Stop inking| Stop adding ink.  |  
|Colors|Open color picker to determine color of the arrow or ink, and then say blue, gray, green, red, or yellow.|
|Undo| Undo the previous action. |
|Erase all |Remove all annotations that you placed in the environment.|
|Toggle hand rays| Turn hand rays on or off. <br><br>Note that turning hand rays off disables far-field interactions. Turning hand rays back on re-enables far-field interactions. Activating any tools that require far-field interactions (inking and arrows, for example) also automatically turns hand rays back on.|
|Hand rays on|Show hand rays.|
|Hand rays off| Hide hand rays. <br><br>Note that turning hand rays off disables far-field interactions. Turning hand rays back on re-enables far-field interactions. Activating any tools that require far-field interactions (inking and arrows, for example) also automatically turns hand rays back on.|
|**Capture photos or videos**||
|Snap, Take picture, Take photo, Capture|Take a photo of the environment.|
|Take photo|	Select the **Take Photo** button.|
|Cancel|	Cancel the photo or video capture.|
|Photo|	Enable the image capture tool.|
|Photo off|	Disable the image capture tool.|
|Retake snapshot|Retake the photo during Snapshot mode.|
|Save to chat|During a call when the Snapshot box is active, save the snapshot to the chat.|
|Record video|Record a video capture of the environment.|
|End recording|Stop the video capture.|
|Video off|Disable the video capture tool.|
|Save to booking	|Save the captured photo to a Dynamics 365 Field Service booking.|
|Save to OneDrive|	Save the captured photo to OneDrive.|
|Dismiss	|Select the **Dismiss** button in the poor connection dialog box.|
|**OneDrive file management**   | | 
|Files|Switch to the **Files** tab to add a file from OneDrive to your environment.|
|Home|When the **Files** tab is open, go to the root OneDrive folder. |
|Up|When the **Files** tab is open, scroll up in the file directory.|
|Back|When the **Files** tab is open, go back.|
|Previous page|Go to the previous page in OneDrive.|
|Next page|Go to the next page in OneDrive.|
|Previous|When viewing a PDF file, go back to the previous page.|
|Next|When viewing a PDF file, go to the next page.|
|Set page|Set the page of the open PDF file.|
|Close|Close OneDrive.|
|**Asset management**||
|New asset|Add a new asset.|
|Rename|Rename an asset.|
|Submit|Submit a new name when renaming an asset.|
|Post, Post all|Post the Field Service items to the work order.|
|Discard, Discard all|Discard the Field Service items at the end of a call.|

## Use the Narrator to announce incoming calls

You can turn on the Narrator if you want to take advantage of voice narration for incoming calls. When you turn on incoming call narration, in addition to displaying the incoming caller's name, the caller's name is announced. You can then say "Remote Assist, Video," "Remote Assist, Audio," or "Remote Assist, Ignore," to respond to the incoming call.

To turn on the Narrator for incoming calls:

- Go to Settings, and then select the **On** button for the Narrator.

 ![Open Narrator.](media/08.00-settings.png "Open Narrator")

## Gestures

The April 2021 release of Dynamics 365 Remote Assist improved gestures on HoloLens 2 to make them more instinctual:

- Improved audio and visual cues make it easier to grab, move, and resize windows, whether you’re directly manipulating windows up close or manipulating them from a distance with hand rays.

- Improvements to the near finger cursor make it easier to grab windows and select buttons. 

[!INCLUDE[footer-include](../includes/footer-banner.md)]
