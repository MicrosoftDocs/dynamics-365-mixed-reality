---
title: File sharing
author: xonatia
description: Send and receive files between technicians and experts
ms.author: xolee
ms.date: 04/01/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Share files between technicians and experts to improve collaboration

Remote Assist for mobile provides technicians and remote collaborators with document sharing capabilities. Sharing documents promotes seamless collaboration during a call by adding more context and information, such as visual aids and schematics, to the technicians’ environment. This facilitates technicians having richer conversations with remote collaborators and, ultimately, solve their problems quickly and efficiently.  
 
Both the technician and remote collaborators can send **any** file type to each other. This includes .jpg, .png, .tiff, .mp4, .pdf, .docx, .xlsx, .txt, and .apk files. They can upload files and images from their local device or OneDrive. In order for technicians to open and access these different file types, they will need the corresponding app that supports the file type.  

If you're a Dynamics 365 Field Service customer, the files shared during your Remote Assist for mobile call can be linked to your work order, learn more [here](https://docs.microsoft.com/en-us/dynamics365/mixed-reality/remote-assist/mobile-app/fs-integration).

## How it works
### Sending files 
1. The technician must select the **text chat** to start sharing files to the remote collaborator. 

2. In the text chat, the technician is presented with the **Attachment** and **Image** icons. 
![Icons](./media/filesicons.PNG "Icons")

3. If the technician selects the **Attachment** icon, an option of files from the technician's local device will be displayed. 
> [!Note]
> For iOS, the technician is presented with the Files app directly. On Android, it can either be a File chooser or a Menu to choose which app to use as a file chooser.

4. The technician selects the files to send to the remote collaborator. The technician can select up to 5 images at a time. The technician will see the uploading progress until it's ready to be sent. 
![Upload](./media/filesprogress.PNG "Upload")

5. If the technician selects the **Image** icon, the technician gets the option to choose to **select images** from the mobile device's Photo Gallery or Files apps. 
> [!Note] 
> For iOS, the technician is presented with the Photos app directly. On Android, it can either be a Photo Gallery or a Menu to choose which app to use as your picture chooser.

6. If all of the files are not successfully uploaded in the chat, the technician can select the **Arrow** and retry downloading the unsuccessful files or remove any files. 
![Retry](./media/files_fail.PNG "Retry")

7. Select **send**.

8. The file link or image preview is sent to the collaborator through OneDrive, which sets the permission to share the file with the remote collaborator. Afterwards, the remote collaborator on Teams receives a link to the document in OneDrive in the Microsoft Teams text chat. The remote collaborator has full access to the document. 
![Preview](./media/files_view.PNG "Preview")

### Receiving files 
1. In the text chat, the technician selects the file's link or image preview to open it and view larger and they are automatically downloaded to the device's Downloads folder. 
2. If the file is an image, the image now takes up the technician's device screen. 
3. If the file is not an image and if the technician has an app that can open this file type, the technician can view the file in the app. The user now has full access to the file. 
4. If the file is not an image and if the technician does not have an app that can open this file type, the technician cannot view the file. We still ask the user how to open this file.  
5. If there are any issues while downloading or opening the file, there is a pop-up notification stating the issue

