---
author: prashantyvr
description: Learn how to opt out of storing Microsoft Dynamics 365 Guides usage data in Microsoft Dataverse, for privacy reasons.
ms.author: prashan
ms.date: 02/20/2024
ms.topic: how-to
title: Opt out of storing Dynamics 365 Guides usage data in Microsoft Dataverse
ms.reviewer: v-wendysmith
ms.custom:
  - bap-template
  - sfi-image-nochange
---

# Opt out of storing Dynamics 365 Guides usage data in Microsoft Dataverse

Dynamics 365 Guides enable teams to capture usage statistics and detailed time-tracking information. This data is used to provide metrics for operator and author performance and to help you identify opportunities for process optimization. Administrators can turn off data collection for specific users if needed.

## Opt out of storing usage data

1. [Open the model-driven app](open-model-driven-app.md).

1. On the bottom left side of the screen, select **Main**, and then select **Settings**.

   :::image type="content" source="media/main-to-settings-area.PNG" alt-text="Screenshot that shows changing from Main to Settings area in the Guides model-driven app.":::

1. Select **New** at the top of the screen.

1. In the **New User Settings** screen, under **User Settings**, enter the following:

    - **Name:** Opt out for *[User name]*

    - **Record Guide Usage:** No

    - **Belongs To:** *[User name]*

1. Select **Save** at the top of the screen.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
