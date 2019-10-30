---
author: JBrentJ
description: How to use Dynamics 365 Import Tool (Preview) to prepare 3D models for Dynamics 365 mixed-reality applications
ms.author: v-jerja
ms.date: 10/29/2019
ms.service: crm-online
ms.topic: article
title: Use Dynamics 365 Import Tool (Preview) to prepare 3D models for Dynamics 365 mixed-reality applications
ms.reviewer: v-brycho
---

# Use Dynamics 365 Import Tool (Preview)

Use [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] to prepare your 3D models to use in [!include[pn-dyn-365](../includes/pn-dyn-365.md)] mixed-reality applications. 

> [!div class="mx-imgBorder"]
> ![Import Tool flow](media/import-tool-flow.png "Import Tool flow") 

## Two options for preparing 3D models

[!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] provides two options for preparing your 3D models: 

> [!div class="mx-imgBorder"]
> ![Import Tool options](media/import-tool-options.PNG "Import Tool options") 
 
If you choose the **Import using this PC** option, you’ll need to prepare your models yourself using the instructions in these topics:

- [Convert your 3D models](convert-models.md)
- [Optimize your 3D models](optimize-models.md)
- [Best practices for 3D models](best-practices.md)

If you choose the **Send model to [!include[cc-microsoft](../includes/cc-microsoft.md)]** option, [!include[cc-microsoft](../includes/cc-microsoft.md)] converts and optimizes your model for you and will provide a download link when the model is ready.

### Import using this PC option

1.	On your PC, open [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)].

2.	Select **Models** > **PC**, and then select **Add models**.

3.	Go to the folder where your models are saved, and then select the models you want to import (up to 25 at a time).

4.	Select **Open**.

5.	In the **Prepare Model** dialog box, under **How would you like to prepare the model?**, select **Import using this PC**.

    > [!div class="mx-imgBorder"]
    > ![Import using this PC option](media/import-using-pc-option.PNG "Import using this PC option") 

6.	Select **Apply**.

#### If you encounter file access errors when importing files

3D models sometimes reference other files in your file system, such as textures and materials files. Your imported 3D model might not look correct if Dynamics 365 Import Tool (Preview) can’t access these files, in which case, you might see this error dialog box:

> [!div class="mx-imgBorder"]
> ![File access errors dialog box](media/file-access-errors.PNG "File access errors dialog box") 

There are two primary reasons why Dynamics 365 Import Tool (Preview) might not have access to these files:

- **No permissions**. For the safety and security of your files, Windows 10 does not allow all Windows Store applications full access to the files in your system. To allow Dynamics 365 Import Tool (Preview) access to your files, select **Grant permissions**, go to the folder(s) that contains the files, and then select the folder(s). This grants access to all files in the folder. Alternatively, you can move your 3D models and all their referenced files to the **3D Objects** folder.

- **Missing files**. Dynamics 365 Import Tool (Preview) expects the files to appear in the exact file paths listed in the dialog box. If files are not there, they will be marked as missing. Move the missing files to locations indicated in the dialog box, or update the original 3D model.

### Send model to Microsoft option

1.	On your PC, open [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)].

2.	Select **Models** > **PC**, and then select **Add models**.

3.	Go to the folder where your models are saved, and then select the model you want to import.

4.	Select **Open**.
 
5.	In the **Prepare Model** dialog box, under **How would you like to prepare the model?**, select **Send model to [!include[cc-microsoft](../includes/cc-microsoft.md)]**.

    > [!div class="mx-imgBorder"]
    > ![Send model to Microsoft option](media/send-model-microsoft-a.png "Send model to Microsoft option")

6.	Under **Enter your email address**, enter the email address where [!include[cc-microsoft](../includes/cc-microsoft.md)] can contact you when the model is ready.

7. Select **Next**.     

8.	Under **Where will you use this model?**, choose the target device. You can only choose one type of target device at this time.

    > [!div class="mx-imgBorder"]
    > ![Send model to Microsoft option, second page](media/send-model-microsoft-2.png "Send model to Microsoft option")

9.	Under **How many models will your scene have?**, select the appropriate option for your scene complexity. 

10. In the **What's most important to you about your model** box, provide instructions for Microsoft. For example, specify which is most important to you—visual accuracy or performance.

11.	Select **Apply** to send the model to [!include[cc-microsoft](../includes/cc-microsoft.md)].

    [!include[cc-microsoft](../includes/cc-microsoft.md)] sends you the following email notification to confirm that the model has been sent:
    
    > [!div class="mx-imgBorder"]
    > ![Confirmation email](media/confirmation-email.PNG "Confirmation email") 

    [!include[cc-microsoft](../includes/cc-microsoft.md)] updates you on the progress of the manual optimization through email and lets you know when the model is ready to download.

## What happens to my model when I send it to Microsoft?

When you send your model to [!include[cc-microsoft](../includes/cc-microsoft.md)], it’s uploaded to a secure location. [!include[cc-microsoft](../includes/cc-microsoft.md)] prepares the model using a combination of automated and manual steps. [!include[cc-microsoft](../includes/cc-microsoft.md)] provides a download link when the model is ready. After you download it, your model is deleted from the secure storage area.  

> [!div class="mx-imgBorder"]
> ![Model preparation](media/what-happens.png "Model preparation") 

## Download a model after it's been converted and optimized by Microsoft

1.	Open the [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)].

2.	Right-click the model that was submitted for manual processing, and then select **Download from [!include[cc-microsoft](../includes/cc-microsoft.md)]**.

    > [!div class="mx-imgBorder"]
    > ![Download model](media/download-model.PNG "Download model") 

## Locate your converted assets

Files created with [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] are stored locally. To find the files on your local drive:

1.	Open [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)].

2.	Right-click a model, and then select **Open file location**.

    > [!div class="mx-imgBorder"]
    > ![Locate model](media/locate-model.PNG "Locate model")

## Provide feedback on the quality of processed 3D models

You can provide feedback on the quality of processed 3D models if you're not satisfied.

1.	Select the **Models** or **All** tab, and then select the model you want to provide feedback on.

2.	At the bottom of the **Properties** tab, under **How does the model look?**, select **Looks good** or **Looks broken** to record your feedback.

    > [!div class="mx-imgBorder"]
    > ![Provide feedback](media/feedback.PNG "Provide feedback") 

    > [!NOTE] 
    > You can't update feedback after you submit it.

## Do I need to be connected to Wi-Fi to use Dynamics 365 Import Tool (Preview)?

[!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] requires users to be signed in with their Active Directory account to access the application. Users need to be connected to Wi-Fi the very first time the application is launched. After the first launch, they need to be connected to Wi-Fi once every 30 days so that the application can validate that the user has a valid Active Directory account for continued use of the application.

In addition to the above, Wi-Fi connectivity requirements depend on the method that users choose to import models:

- **Import using this PC**. When users choose this option to import models, a Wi-Fi connection is not required.

- **Send my model to [!include[cc-microsoft](../includes/cc-microsoft.md)]**. When users choose this option to import models, a Wi-Fi connection is required. To understand how your models are processed by [!include[cc-microsoft](../includes/cc-microsoft.md)], see [What happens to my model when I send it to Microsoft?](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/import-tool#what-happens-to-my-model-when-i-send-it-to-microsoft). 

### See also
[Overview of Dynamics 365 Import Tool (Preview)](index.md)<br>
[Convert 3D models](convert-models.md)<br>
[Optimize 3D models](optimize-models.md)<br>
[Best practices for converting and optimizing models](best-practices.md)<br>
[Tutorials for converting and optimizing 3D models](tutorials-overview.md)<br>



