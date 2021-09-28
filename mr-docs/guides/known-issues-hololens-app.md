---
author: Mamaylya
description: Learn about known issues with the Microsoft Dynamics 365 Guides HoloLens app.
ms.author: mamaylya
ms.date: 06/26/2021
ms.topic: article
title: Known issues with the Dynamics 365 Guides HoloLens app
ms.reviewer: v-brycho
---

# Known issues with the Dynamics 365 Guides HoloLens app

## Telemetry data not stored for operators with **Restricted Operator** role in certain cases

Operators with the **Restricted Operator** role that don't have the appendTo privilege can access and operate guides but their session data (telemetry) is not stored for time-tracking purposes.

## The account picker becomes unresponsive if you stay on it for more than 25 seconds during HoloLens sign-in 

On the page where you can select among the different accounts that are saved on [!include[pn-hololens](../includes/pn-hololens.md)], you must select an option within 25 seconds. After 25 seconds, the page becomes unresponsive, and you must restart the app. This issue has been fixed on RS5 but still exists on RS4 if you have that version installed.

## When you place large assets on HoloLens, you might experience minor loading delays

The [!include[pn-hololens](../includes/pn-hololens.md)] app currently loads the guide right after you open it. As you use the guide, the app loads it in the background. If your guide contains large 3D models and media, you might experience loading delays of a few seconds.

## An incorrect profile picture is shown in the app 

If an incorrect profile picture is shown, make sure that you're signed in. Select the profile picture, sign out, and then sign back in by using your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] credentials. Your profile picture should appear correctly.

By using the correct credentials to sign in, you ensure that your work progress is correctly tracked in [!include[pn-dyn-365](../includes/pn-dyn-365.md)].

## The video preview on a step is blurry

The [!include[pn-hololens](../includes/pn-hololens.md)] app converts and resizes videos when they are uploaded, to ensure optimal performance on [!include[pn-hololens](../includes/pn-hololens.md)]. If your video was recorded at a very high resolution, or if it's very large, the transcoding process might degrade its quality. To fix this issue, record and upload a new video, keeping its length and resolution in mind.

As a best practice, video clips should not be too long. We recommend **a maximum of two minutes**. This limit helps operators focus on one meaningful task at a time and keeps them from getting overwhelmed. 

## When the see-through style is applied to a 3D model, it might show gray areas instead of correctly rendering textures 

There are rendering issues for the "see through" style on some 3D models. Some surfaces on these models will look gray. If you experience this issue, use another style. If you **must** use this style and need help with it, contact customer service.

## See also

[Known issues with Dynamics 365 Guides generally](known-issues.md)<br>
[Known issues with the PC app](known-issues-pc-app.md)<br>
[Dynamics 365 Guides FAQ](faq.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
