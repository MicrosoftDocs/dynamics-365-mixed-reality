---
author: davepinch
description: Learn how to view and access call data stored by Dynamics 365 Guides.
ms.author: davepinch
ms.date: 02/22/2024
ms.topic: how-to
title: View and access call data stored by Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# View and access call data stored by Dynamics 365 Guides

When Microsoft Dynamics 365 Guides users make or receive calls in the HoloLens app, [call information](call-data-logs.md) is stored in Microsoft Dataverse. Users can view only their own calling data; administrators can view calling data from all users.

> [!NOTE]
> This feature is intended to help supervisors and managers derive insights regarding operational efficiencies and usage of Dynamics 365 Guides. This feature is not intended for use in making—and should not be used to make—decisions that affect the employment of an employee or group of employees, including compensation, rewards, seniority, or other rights or entitlements. Customers are solely responsible for using Dynamics 365, this feature, and any associated feature or service in compliance with all applicable laws, including laws relating to accessing individual employee analytics and monitoring. End users will need to enable access from their device to phone call records and specifically consent to sharing location information before that information is shared and available. However, customers are also encouraged to have a mechanism in place to inform their users that analytics (such as call duration and location) relating to their communications are collected.

## View call data

1. [Open the Guides model-driven app](open-model-driven-app.md).

1. On the left side of the screen, under **Analytics and Insights**, select **Phone Calls**.

   :::image type="content" source="media/call-logging-model-driven-app.JPG" alt-text="Screenshot of model-driven app with call information.":::
  
1. If you're a user, you can view your own call records. If you're an administrator, to view all call records, select the **All Phone Calls** view.

   > [!NOTE]
   > If location fields are empty, the HoloLens user didn't provide [permission](hololens-permissions.md) for that data to be stored.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
