---
title: View 3D models without using your device's camera with Dynamics 365 Product Visualize
description: Learn how to View 3D models without using your device's camera.
author: sbmjais
ms.author: shjais
manager: shujoshi
ms.date: 05/28/2020
ms.service: crm-online
ms.topic: article
ms.reviewer:
---

# View 3D models without using your device's camera
<!--Shubham, I'm afraid I had a hard time understanding this article, so please excuse if my suggested edits miss the mark. Firstly, the phrase "camera and augmented reality" was confusing to me. If I'm correctly interpreting what I've read about augmented reality (which we don't define in the Product Visualize doc set, by the way; maybe we should?), a person uses their camera to create a physical "place" to put a virtual model on, and this blending of real and virtual is "augmented reality." Second, the emphasis in the title seems a bit off: it's not as interesting that you're "viewing a model without using your camera," it's that you can use a blank background or any neat photo you want. But I'm not your typical reader, so maybe being able to bypass the camera is actually more interesting than the creative possibilities of a creating a custom background for 3D models?-->
The default behavior for viewing 3D models in Dynamics 365 Product Visualize is to use your device's camera to create a physical background for the model in an augmented reality (AR) experience. When you enable the **Show AR mode toggle button** feature, you can turn off this default AR behavior, and instead place your model on a gray background or use a background image from your Photos library. When you turn AR mode back on, you can use your device's camera to place the 3D model as usual.

> [!NOTE]
> Viewing 3D models without using your device's camera is a preview feature. Preview features are experimental features that provide access to the latest innovations that the Dynamics 365 Product Visualize team is working on.

## Enable AR mode

1. Tap **Main** ![Main menu](media/hamburger-icon.png "Main menu"), and then tap **Preview features**.

    > [!div class=mx-imgBorder]
    > ![Preview features](media/preview-features.png "Preview features")

2. In the **Feature Settings** screen, set **Show AR mode toggle button** to **On**.<!--The Writing Style Guide would have this be "turn on the **Show AR mode toggle button** toggle," but I suggest using "setting" here. Not only to avoid "**toggle...** toggle", but to avoid a bit of confusion later when you talk about the **AR** toggle.-->

    > [!div class=mx-imgBorder]
    > ![AR mode feature](media/ar-mode-feature.png "AR mode feature")

## Turn AR mode on and off

After you enable **Show AR mode toggle button**, AR mode is turned off by default. Your 3D models will be placed on a gray background that you can customize if you want by using a photo from your Photos library. As you place your model, the **AR** toggle is displayed at the top of the screen. To turn AR mode back on, tap the **AR** toggle. 

> [!div class=mx-imgBorder]
> ![Model placed on a gray background, with AR mode off](media/ar-off.png "Model placed on a gray background, with AR mode off")

When you turn on the AR mode, you can use your device's camera and augmented reality to place a 3D model.

> [!div class=mx-imgBorder]
> ![Model placed on a captured background, with AR mode on](media/ar-on.png "Model placed on a captured background, with AR mode on")

More information: [Place and manipulate 3D models](manipulate-models.md)

## Add or replace the background image

You can choose to keep the models on a gray background or add a background image by selecting an image from your Photos library.

**To add a background image**

1. Tap the background image ![Add background](media/add-background-icon.png "Add background") icon in the upper-left corner of the screen.

2. Select an image from your Photos library.

**To replace the background image**

1. Tap the background image ![Add background](media/add-background-icon.png "Add background") icon in the upper-left corner of the screen.

2. In the options<!--Is it named "Options"? If so, should be bold, here and below.--> dialog box, tap **Replace**.

**To remove the background image**

1. Tap the background image ![Add background](media/add-background-icon.png "Add background") icon in the upper-left corner of the screen.

2. In the options dialog box, tap **Remove**.

### See also

[Install, open, and sign in to the app](sign-in.md)<br>
[Place and manipulate 3D models](manipulate-models.md)<br>
[Add a note to a 3D model](add-note.md)<br>
[Show or hide layers in a 3D model](layers.md)<br>
[Explore sample 3D models](explore-samples.md)<br>
[View 3D models stored on your device](browse-models.md)<br>
[Add your own 3D model to an existing Dynamics 365 Sales product](add-model.md)<br>
[Download 3D models to use offline](download-models.md)<br>
[Enable product dimensions](product-dimensions.md)