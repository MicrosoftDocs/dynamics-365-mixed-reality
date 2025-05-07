---
author: prashantyvr
ms.author: prashan
description: Learn about supported file formats for 3D objects, images, and videos in Microsoft Dynamics 365 Guides.
ms.date: 02/22/2024
ms.topic: article
title: Supported file formats and limits for 3D objects, images, and videos
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Supported file formats and limits for 3D objects, images, and videos

In Microsoft Dynamics 365 Guides, you can use the PC app to add 3D objects, images, and videos to help operators with steps.

## Support file formats

The PC app supports the following file formats for these types of files.

| Media | Supported formats | Best practice |
|-------|-------------------|---------------|
| 3D objects | FBX, GLB, glTF, STL, PLY | Optimize your 3D objects as much as possible, to help maintain optimal performance on HoloLens. For more information, see [Convert CAD drawings to use as holograms](author-convert-3D-models.md). |
| Images | PNG, JPG, JPEG, BMP, TIF | |
| Video/audio | MP4, MOV, WMV, ASF, AVI M2TS, MKV| Keep your videos less than two minutes long and focused on one step at a time. |

## Step content recommended limits

When authors create guides, each step can have different content associations. Guides measures the totality of all content on a step to estimate performance on HoloLens. If limits are exceeded, HoloLens might exhibit poor performance or be unable to display content on steps. We recommend authors check overall memory usage warnings when authoring on HoloLens.

It is the responsibility of the author to balance content on their steps within available limits.

[!INCLUDE [supported-step-limits](../includes/supported-limits-steps.md)]

## 3D object limits

[!INCLUDE [supported-object-limits](../includes/supported-limits-objects.md)]

## More information on 3D objects, images, and videos 

- The August 10, 2022 release introduced a new setting that improves video transcoding. If the PC app detects a hardware transcoding failure, it automatically uses software transcoding instead. If the software transcoding is successful, the **Use hardware video encoding on this device** setting is automatically updated to switch off hardware video encoding. 

     ![Screenshot of Use hardware video encoding on this device setting.](media/video-transcoding-setting.PNG "Screenshot of Use hardware video encoding on this device setting")

- The supported video format resolution is 854 x 480 H.264 MP4 (commonly called "Advanced Video Recording"). Any other formats are transcoded when imported and might result in a larger file size than the original.

- The file size limit for a video, image, or 3D object is 128 MB. Transcoding might occur when uploading, which might change the size of the file that needs to be stored. This change can cause the upload to fail if the file is too large.

- Dynamics 365 Guides uses meters as the default scale unit. If your 3D object scale is set to millimeters when you export from your CAD solution, the object is converted to meters in Dynamics 365 Guides. For example, if your object is 50 millimeters, it's converted to 50 meters. To ensure size consistency between your CAD solution and Dynamics 365 Guides, make sure to set your object scale unit to meters when you export.  

- Some glTF files might have dependencies in other folders. During upload, if the app doesn't have permissions to those folders, errors can occur, or 3D objects in the gallery might be broken. When you upload glTF objects, make sure that you have permissions to all dependencies, or that all dependencies are in the same folder.

## Next steps

- [Step Editor overview](pc-app-step-editor-overview.md)
- [Add a 3D object from the toolkit](pc-app-add-3D-model.md)
- [Add a 3D part](pc-app-add-3D-part.md)
- [Add an image or video file](pc-app-add-media.md)
- [How to make a great mixed-reality guide](great-guide.md) 
