---
author: Mamaylya
description: Guides model-driven app overview
ms.author: mamaylya
ms.date: 06/22/2023
ms.topic: overview
title: Guides model-driven app overview
ms.reviewer: v-wendysmith
---

<!-- This article could be a redirect to the article below with the term "App" updated to "Guides model-driven app".   A better solution will have to be found to "customize" core power apps support documents to address the specific D365 Guides user experience.  
https://learn.microsoft.com/powerapps/user/assign-or-share-records -->

# Guides model-driven app overview

When you create a guide in the PC authoring app, the content is stored in Microsoft Dataverse. The Guides model-driven app enables you to access and view guide content quickly from Microsoft Dataverse.

If you're an admin or an author for Dynamics 365 Guides, you can use the Guides model-driven app to do things that you can't do in the PC app or HoloLens app. For example, you can:

- [Change a thumbnail for a video associated with a step](pc-app-add-media.md#change-a-video-thumbnail)

- [Create a 3D object collection](workflow-example-2.md)

- [Create folders to organize your guides](admin-create-folders.md)

- [Create workflows in Microsoft Power Apps to automate Dynamics 365 Guides processes](workflow-examples-overview.md)

- [Activate, deactivate, or delete a guide](admin-deactivate-guide.md)

- [Fix a corrupted guide](corrupted-guide.md)

- [Set up Guides Analytics reports](analytics-ga-setup.md)

- [Share content](admin-share-guide.md)

- [View call data stored by Dynamics 365 Guides](call-logging.md)

> [!CAUTION]
> The Guides model-driven app isn't intended as a replacement for authoring in the PC and HoloLens apps. If you use the model-driven app to create, update, or delete records, you might make Dynamics 365 Guides nonfunctional or prevent users from using the PC or HoloLens apps in the intended way. Currently, guide modification through the model-driven app isn't fully supported unless specifically covered in the Dynamics 365 Guides documentation and should be reserved for experienced Dynamics 365 users who are familiar with Microsoft Dataverse.

## Limit access to the model-driven app

The Guides model-driven app is a type of app created in Microsoft Power Apps.  Organizations may limit users who can access the model-driven app, but a user must be able to access the model-driven app to use the Guides HoloLens or PC app.  You can limit access by sharing the app with individual users, or by sharing it with one or more Azure Active Directory Groups. See [Share a model-driven app using Power Apps](/powerapps/maker/model-driven-apps/share-model-driven-app) for detailed steps on either option.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
