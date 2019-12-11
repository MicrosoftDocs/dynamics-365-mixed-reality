---
author: mamithan
description: Frequently asked questions about Dynamics 365 Product Visualize
ms.author: mamithan
ms.date: 10/01/2019
ms.service: crm-online
ms.topic: article
title: Frequently asked questions about Dynamics 365 Product Visualize
ms.reviewer: v-brycho
---

# FAQ: Dynamics 365 Product Visualize

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

## What are the requirements for running Microsoft Dynamics 365 Product Visualize, and what platforms does it support?

For information about platforms and requirements, check out our [Requirements page](requirements.md).

## What kind of 3D content can I add?

Dynamics 365 Product Visualize supports GLB files only.

## How do I get my content in the right format?

To learn how to format your content, see the following page on the Khronos website: [Art Pipeline for glTF](https://go.microsoft.com/fwlink/p/?linkid=2083000). 

## How does Dynamics 365 Product Visualize connect with Dynamics 365 Sales?

After you sign in with your Azure Active Directory credentials, Dynamics 365 Product Visualize displays organizations associated with your Dynamics 365 Sales account. Opportunities and products associated with your organizations automatically show up in the app, as do 3D models attached to your products.

## Can I use Dynamics 365 Product Visualize to do remote sales?

At this time, Dynamics 365 Product Visualize doesn't support remote capabilities.

## Why is the "Need admin approval" message displayed after signing in?

![Admin Approval](media/admin-approval.PNG "Admin Approval")

This message indicates that your organization requires administrator approval before any new apps can be used to access organizational resources. Talk to your system administrator to get approval to use Dynamics 365 Product Visualize in your organization. In the meantime, you can set up a [free trial version](setup.md).

## Why don't I see my Dynamics 365 instances?
 
Dynamics 365 Product Visualize can connect to instances of Dynamics 365 Sales version 9 or later. It doesn't support on-premises Dynamics 365 solutions or older instances of Dynamics 365 Sales. Make sure your instance meets the [minimum requirements](requirements.md) for using Dynamics 365 Product Visualize. If your instance meets the requirements, make sure you're signed in to the app with the same credentials you use to access Dynamics 365 Sales.

## Why am I getting a message that says my organization isn't set up to use Dynamics 365 Product Visualize?

This message indicates the Dynamics 365 Sales instance you selected doesn't meet the [minimum requirements](requirements.md) for using Dynamics 365 Product Visualize. If you have access to more than one Dynamics Sales instance, make sure you selected the correct one.

## How do I find my opportunities?

Dynamics 365 Product Visualize helps you stay organized by focusing only on the opportunities that are important to you. From the Opportunity Selection view, there are three options for viewing your opportunities:

1. **My Open Opportunities** - Open opportunities where you're listed as the owner.
2. **My Connected Opportunities** - Open opportunities where you've been added to the Sales team.
3. **My Followed Opportunities** - Open opportunities that have been marked as __Followed__.

If an opportunity doesn't show up in the app, go to the Dynamics 365 Sales Hub and ensure that at least one of these criteria is met.

## Why doesn't my model load?

Models with very high polygon counts might take a long time to load, especially over slower connections. If the model doesn't load at all, the GLB file might not be valid. A corrupt or invalid GLB file can appear as if it were loading but it will never actually load. If this happens, restart the app and try again. If, after restarting, the model still fails to load, try re-exporting the GLB from your authoring software and upload it again to SharePoint. If that doesn't work, try loading the model in a different glTF viewer like [BabylonJS Sandbox](https://sandbox.babylonjs.com/).

Larger models might exceed the memory of the mobile device you're using. This is especially true on previous-generation iPhones. To reduce the model's memory requirements, reduce the size of any textures associated with the model and decimate the model to use fewer polygons.

### See also

[Requirements for setting up Dynamics 365 Product Visualize](requirements.md)<br>
[Set up Dynamics 365 Product Visualize](setup.md)<br>
[Administrator guide](admin-guide.md)<br>
[User guide](user-guide.md)<br>
