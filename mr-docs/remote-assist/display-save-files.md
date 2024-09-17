---
author: prashantyvr
description: Learn how to share and save files in Microsoft Dynamics 365 Remote Assist on HoloLens. 
ms.author: prashan
ms.date: 06/14/2024
ms.topic: article
title: Share and save files in Dynamics 365 Remote Assist on HoloLens
ms.reviewer: v-wendysmith
---

# View service-related documentation and save shared files

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

During your repair or inspection, you might want to refer to an image or PDF related to the asset or procedure you're completing.
For example, you can place a wiring diagram in the space next to the asset you're working on. During a video call, a remote collaborator can share a reference to help you better understand what an asset should look like after you've successfully repaired it.

> [!NOTE]
> Dynamics 365 Remote Assist follows Teams policies for sharing files. If your Teams policies are configured to prevent file sharing, users won't be able to share files with each other. Files can't be shared if an external user is on the call or if a user is not a member of a Teams channel in a channel meeting. For more information, see:
> - [Use guest access and external access to collaborate with people outside your organization](/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access)
> - [Native chat experience for external (federated) users in Microsoft Teams](/microsoftteams/native-chat-for-external-users)

If you're in a video call, any call participant can annotate the file, just as they would annotate any physical object.

> [!NOTE]
> You can share an image file by attaching it from the Mixed Reality toolbar. You can't paste a bitmap image into the body of a chat message. If you do that, it will be pasted as [Image Image]. 

## Prepare your workspace with files from OneDrive

Files are accessible at any time in Dynamics 365 Remote Assist. You don't need to be in a call to access your files from OneDrive and place them in your workspace. To display a OneDrive file, select the **Files tab**, or say “Remote Assist, Files" and select the file. The file pops up as a new slate in your space. If you are on a video call, remote collaborators are able to see the image or PDF file as long as you’re looking at it. Supported files include:

- .jpg
- .bmp 
- .png
- .tif or .tiff 
- .pdf
- still .gif 

At this time, a link to the OneDrive file isn't sent in the Teams chat if you open a file during a call.

## Save a file shared by a remote collaborator to OneDrive

When a Teams user shares a file from OneDrive or from their device during a video call, it appears as a new slate in your space. A link to the file is shared in the chat. Even after the call ends, you can find the link in your Teams chat. 

You might also want to save the file to your OneDrive for future reference. For example, the Teams user might send a PDF of a schematic you can use in future repairs, so you want to save it to your OneDrive and share the OneDrive file with others. 

To save the file to OneDrive, select the OneDrive icon (as seen here: ![OneDrive.](media/RAHL_OneDrive.png)) in the top right of the slate. The OneDrive file is then automatically saved to a folder called **HoloLens Received Files**.

>[!Note]
>The top right corner of the PDF displays the page number you’re currently on as well as the total number of pages. You can use the **Previous** and **Next** arrows to navigate pages. To navigate to a specific page, select the current page number. A numeric keyboard will pop out. Select the page number you want to navigate to.

## Save a file shared by a remote collaborator to your work order

Field Service organizations often want to capture tribal knowledge and relevant contextual information from technicians, inspectors, and remote collaborators. Contextual information includes the schematics and reference images that call participants share. These files can be used for training and building a knowledge base for faster problem resolution and first-time fix rate. 

If you made a Dynamics 365 Remote Assist call in the context of a Field Service booking, you can post the files shared during the call to the work order that the booking is associated with. When the call ends, a list of files that you and any remote collaborator shared appear.

![Screenshot showing Dynamics 365 Remote Assist in the HoloLens, with a prompt to post files to work order.](media/RAHL_PostToWorkOrderPrompt.png)
 
Select **Post All** to save the files and **Call Log** to the work order. The **Call Log** includes the names of the call participants and the call duration.

Specifically, two new notes are created and attached to the work order. One note includes call log info, and the other note includes a plain text link to each file. 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
