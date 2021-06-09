---
title: Share the Guides model-driven app with other users
description: Learn how to share the Guides model-driven app to provide access to other team members.
author:  MattHoag-MS
manager: tfehr
ms.topic: article
ms.date: 06/10/2021
ms.author: v-mhoag
ms.reviewer: v-bholmes
---
<!-- This article could be a redirect to the article below with the term "App" updated to "Guides model-driven app".   A better solution will have to be found to "customize" core power apps support documents to address the specific D365 Guides user experience.  
https://docs.microsoft.com/powerapps/user/assign-or-share-records -->

# Share the Guides model-driven app to provide access

When you create a guide in the PC authoring app, the content is stored in the Microsoft Dataverse. The Guides model-driven app enables you to access and view guide content from the Dataverse quickly. You can also make modifications through the Guides model-driven app. For example, you can [deactivate a guide](admin-deactivate-guide.md), [share content](admin-access-teams.md), or [create a 3D object-collection](workflow-example-2.md).

> [!CAUTION] 
> The Guides model-driven app isn't intended as a replacement for authoring in the PC and HoloLens apps. If you use the model-driven app to create, update, or delete records, you might make Dynamics 365 Guides nonfunctional or prevent users from using the PC or HoloLens apps in the intended way. Currently, guide modification through the model-driven app isn't fully supported and should be reserved for experienced Dynamics 365 developers who are familiar with Microsoft Dataverse.

## Open the Guides model-driven app

1. In the PC authoring app, sign in to the Dynamics 365 instance that includes the guide.

2. Select the **Analyze** tab, and then under **Instance URL**, select **Copy**, and then paste the value into the address bar of a web browser.

    ![Copy the Instance URL value](media/copy-instance-url.jpg "Copy the Instance URL value")

3. Sign in, and then in the left pane of the **Power Apps** screen, select **Guides** to open the Guides model-driven app.

    ![Guides model-driven app example](media/Guides-Hub.png "Guides model-driven app example")

## Limit access to the Guides model-driven app

The Guides model-driven app is a type of app created in Microsoft Power Apps. It's common for organizations to limit users who can access the model-driven app. You can do this by sharing the app with individual users, or by sharing it with one or more Azure Active Directory Groups. For more information, see [Share a model-driven app using Power Apps](https://docs.microsoft.com/powerapps/maker/model-driven-apps/share-model-driven-app) for detailed steps on either option. 
 
