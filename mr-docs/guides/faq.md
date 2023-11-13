---
author: davepinch
description: Frequently asked questions about Dynamics 365 Guides
ms.author: davepinch
ms.date: 11/01/2023
ms.topic: faq
title: FAQ about Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# Frequently asked questions about Microsoft Dynamics 365 Guides

## Dynamics 365 Guides 8.0 and Dynamics 365 Remote Assist FAQ

Frequently asked questions related to Dynamics 365 Guides 8.0.

## What licenses do I need to access the new collaboration features in Dynamics 365 Guides?

You need a Dynamics 365 Guides license and a Microsoft Teams license. [Learn more about licensing requirements](requirements.md)

## Can I collaborate with Teams users in the same way as I do in Dynamics 365 Remote Assist?

Yes.

## Does Dynamics 365 Guides 8.0 store call data the same way as Dynamics 365 Remote Assist?

Yes, it stores data in the same table and columns. In addition, Dynamics 365 Guides provides many improvements to the reliability of data collection, especially in environments where internet connections are spotty. [Learn more about viewing and accessing call data in Dynamics 365 Guides](call-logging.md)

## Does Dynamics 365 Guides 8.0 provide a Calls dashboard like Dynamics 365 Remote Assist to analyze call data?

With Dynamics 365 Guides 8.6, Guides has a Calls dashboard. [Learn more about the Guides Calls Dashboard.](calls-dashboard-guides.md)

## Do I need to update privileges for custom security roles?

Yes. If you have created custom security roles, you must update those roles to provide privileges to the Activity table (PhoneCall table). **Users won't be able to sign in to either app if you don't update custom security roles.** Users must have the following seven privileges to be able to sign in:

- prvAppendActivity
- prvAppendToActivity
- prvAssignActivity
- prvCreateActivity
- prvReadActivity
- prvShareActivity
- prvWriteActivity

![Screenshot of required privileges for Activity table.](media/admin-security-roles-activity-table.JPG "Screenshot of required privileges for Activity table")

> [!NOTE]
> The Delete privilege is not required. 

## Can I share a deep link to a guide through a HoloLens chat?

Yes, Teams desktop users can share a link to a guide directly in chat. HoloLens users can open a guide directly (or even a particular step in a specific guide) by selecting the link. [Learn more about creating a deep link](pc-app-copy-link-guide-step.md)

## Do I need to configure any new permissions?

There are two new permissions: 

- The Location permission (optional) can be enabled if you want to store location information in the PhoneCall table.

- The Background spatial perception (movement) permission is required if you want to use the new annotations capabilities.

[Learn more about permissions required for the HoloLens app](hololens-permissions.md)

## If I'm using both Dynamics 365 Guides and Dynamics 365 Remote Assist for a while, will I be able to filter call data by app?

Yes, you can filter by subject in the Guides model-driven app. The subject value for Dynamics 365 Remote Assist calls is "Dynamics 365 Remote Assist Call".

## How do I configure roles for users who need to use calling and annotations functionality only and who are mostly using Dynamics 365 Remote Assist currently?

There’s no built-in way to limit access in Dynamics 365 Guides to just calling functionality.

To transition a specific user to Dynamics 365 Guides 8.0, you need to do two things:

1. Assign the Dynamics 365 Guides license to that user.

2. Assign one of Dynamics 365 Guides roles.

The user will be able to sign into Dynamics 365 Guides after doing these two steps.

[Learn more about assigning security roles](assign-role.md)

## Copilot in Dynamics 365 Guides

### What is Copilot in Dynamics 365 Guides?

Microsoft Copilot in Dynamics 365 Guides combines the power of generative AI with mixed reality to help frontline workers complete complex tasks and resolve issues faster with less disruption to the flow of work. Copilot on HoloLens not only tells frontline workers how to accomplish a task in words but can also show them what to do in the context of their work with holograms.

### How and when is Copilot in Dynamics 365 Guides going to be available?

The Copilot capability in Dynamics 365 Guides is currently in private preview for HoloLens 2. We’ll share more details on public preview and general availability in the future.

### What capabilities are currently planned for Copilot in Dynamics 365 Guides?  

[Read the full blog to learn about Point and Ask, Spatial content generation, and more.](https://aka.ms/MixedReality)

### What is the process for training Copilot in Dynamics 365 Guides on an organization’s internal knowledge base?

Copilot will only have access to an organization’s internal knowledge bases, which would be supplied to it to learn from, for example schematics, manuals, 3D assets and standard operating procedures. The process is simple. An organization’s trainer or team lead/supervisor takes all relevant documentation, diagrams, etc. for a specific asset and places it into the corresponding folder in Microsoft Dataverse.

Customers can also expand the knowledge base of Copilot in Dynamics 365 Guides by adding remote support transcripts and other materials developed during use to its repository of information.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
