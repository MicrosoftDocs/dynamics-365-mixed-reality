---
author: Mamaylya
description: Learn how to opt out of storing Microsoft Dynamics 365 Guides usage data in Microsoft Dataverse, for privacy reasons.
ms.author: mamaylya
ms.date: 06/23/2023
ms.topic: how-to
title: Opt out of storing Dynamics 365 Guides usage data in Microsoft Dataverse
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Opt out of storing Dynamics 365 Guides usage data in Microsoft Dataverse

Dynamics 365 Guides enable teams to capture usage statistics and detailed time-tracking information. This data is used to provide metrics for operator and author performance and to help you identify opportunities for process optimization. Administrators can turn off data collection for specific users if needed.

## Opt out of storing usage data

1. [Open the model-driven app](open-model-driven-app.md).

1. On the left side of the screen, select the up arrow next to **Main**, and then select **Settings**.

    ![User Settings.](media/data-opt-out-user-setting.PNG "User Settings")

1. Select **New** at the top of the screen.

1. In the **New User Settings** screen, under **User Settings**, enter the following:

    - **Name:** Opt out for *[User name]*

    - **Record Guide Usage:** No

    - **Belongs To:** *[User name]*

    ![Filled-out form.](media/data-opt-out-filled-out-form.PNG "Filled-out-form")

1. Select **Save** at the top of the screen.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
