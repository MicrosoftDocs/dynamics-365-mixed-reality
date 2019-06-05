---
author: BryceHo
description: How to use Dynamics 365 Import Tool (Preview) to prepare 3D models for Dynamics 365 mixed-reality applications
ms.author: BryceHo
ms.date: 04/26/2019
ms.service: crm-online
ms.topic: article
title: Use Dynamics 365 Import Tool (Preview) to prepare 3D models for Dynamics 365 mixed-reality applications
ms.reviewer: v-brycho
---

# Use Dynamics 365 Import Tool (Preview)

> [!div class="mx-imgBorder"]
> ![Import Tool flow](media/import-tool-flow.PNG "Import Tool flow") 

Use [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] to prepare your 3D models to use in [!include[pn-dyn-365](../includes/pn-dyn-365.md)] mixed-reality applications. 

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

5.	Select **Import using this PC**.

    > [!div class="mx-imgBorder"]
    > ![Import using this PC option](media/import-using-pc-option.PNG "Import using this PC option") 

6.	Select **Apply**.

    > [!NOTE]
    > The **Import using this PC** option isn’t available if any of your source models are not in GLB file format.

### Send model to Microsoft option

1.	On your PC, open [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)].

2.	Select **Models** > **PC**, and then select **Add models**.

3.	Go to the folder where your models are saved, and then select the model you want to import.

4.	Select **Open**.
 
5.	Select **Send model to [!include[cc-microsoft](../includes/cc-microsoft.md)]**.

    > [!div class="mx-imgBorder"]
    > ![Send model to Microsoft option](media/send-model-microsoft.PNG "Send model to Microsoft option")

6.	Under **Enter your email address**, enter the email address where [!include[cc-microsoft](../includes/cc-microsoft.md)] can contact you when the model is ready.

7.	Under **Where will you use this model?**, choose the target device. You can only choose one type of target device at this time.

8.	Under **How many models will your scene have?**, select the appropriate option for your scene complexity. 

9.	Select **Apply** to send the model to [!include[cc-microsoft](../includes/cc-microsoft.md)].

    [!include[cc-microsoft](../includes/cc-microsoft.md)] will send you the following email notification to confirm that the model has been sent:
    
    > [!div class="mx-imgBorder"]
    > ![Confirmation email](media/confirmation-email.PNG "Confirmation email") 

    [!include[cc-microsoft](../includes/cc-microsoft.md)] will update you on the progress of the manual optimization through email and will let you know when the model is ready to download.

## What happens to my model when I send it to Microsoft?

When you send your model to [!include[cc-microsoft](../includes/cc-microsoft.md)], it’s uploaded to a secure location. [!include[cc-microsoft](../includes/cc-microsoft.md)] prepares the model using a combination of automated and manual steps. [!include[cc-microsoft](../includes/cc-microsoft.md)] provides a download link when the model is ready. After you download it, your model is deleted from the secure storage area.  

> [!div class="mx-imgBorder"]
> ![Model preparation](media/what-happens.PNG "Model preparation") 

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

### See also
[Overview of Dynamics 365 Import Tool (Preview)](index.md)<br>
[Convert 3D models](convert-models.md)<br>
[Optimize 3D models](optimize-models.md)<br>
[Best practices for converting and optimizing models](best-practices.md)



