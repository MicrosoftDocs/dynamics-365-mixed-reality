---
title: "Share Guides model-driven app with users and groups using security roles to limit access to Dynamics 365 Guides | MicrosoftDocs"
description: How to share Guides model-driven app
author:  MattHoag-MS
manager: anhaman
ms.service: crm-online
ms.component: pa-user
ms.topic: conceptual
ms.date: 03/10/2021
ms.author: v-mhoag
ms.custom: ""
ms.reviewer: ""
ms.assetid: 
search.audienceType: 
  - enduser
search.app: 
  - Guides
  - PowerApps
  - D365CE
---
<!-- This article could be a redirect to the article below with the term "App" updated to "Guides model-driven app".   A better solution will have to be found to "customize" core power apps support documents to address the specific D365 Guides user experience.  
https://docs.microsoft.com/powerapps/user/assign-or-share-records -->

# Share Guides model-driven app to limit access.

When you create a guide, it can be managed in Guides model-driven app.

>[!CAUTION] The Guides model-driven app isn't intended as a replacement for authoring in the PC and HoloLens apps. If you use the model-driven app to create, update, or delete records, you might make Guides nonfunctional or prevent users from using the PC or HoloLens apps in the intended way. Currently, modification through the model-driven app isn't fully supported and should be reserved for experienced Dynamics 365 developers who are familiar with Microsoft Dataverse.

## Access the Guides model-driven app

1. In the PC app, sign in to the Dynamics 365 instance that includes the guide.

2. On the **Analyze** tab, select **Copy** to copy the **Instance URL** value, and then paste the value into the address bar of a web browser.

    ![Copy the Instance URL value](media/copy-instance-url.jpg "Copy the Instance URL value")

3. Sign in, and then select the **Guides** model-driven app.

    ![Guides app](media/guides-model-driven-app.jpg "Guides app")

4. The interface for the Guides model-driven app will be available as  shown below:

![Guide model-driven app example](media/Guides-Hub.png)

It is common for organizations to manage which users can access the Guides model-driven app. Guides model-driven app is a type of Power App.    You can control who in your organization can access Guides model-driven app using the tools provided to manage access for Power Apps.  

Access to a Power App, like Guides model-driven app,  can be managed with individual users, or access can be managed using Azure Active Directory Groups using the steps in the article [Share a model-driven app using Power Apps](https://docs.microsoft.com/powerapps/maker/model-driven-apps/share-model-driven-app)
