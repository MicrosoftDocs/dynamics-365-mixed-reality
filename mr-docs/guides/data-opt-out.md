---
author: Mamaylya
description: Learn how to opt out of storing Microsoft Dynamics 365 Guides usage data in Microsoft Dataverse, for privacy reasons.
ms.author: mamaylya
ms.date: 12/13/2022
ms.topic: article
title: Opt out of storing Dynamics 365 Guides usage data in Microsoft Dataverse
ms.reviewer: v-brycho
---

# Opt out of storing Dynamics 365 Guides usage data in Microsoft Dataverse

Dynamics 365 Guides apps enable teams to capture usage statistics and detailed time-tracking information. This data is used to provide metrics for operator and author performance and to help you identify opportunities for process optimization. Administrators can turn off data collection for specific users if needed. 

## Opt out of storing usage data

1. Go to [https://powerapps.microsoft.com](https://powerapps.microsoft.com) and sign in as an admin.

2. In the tenant/instance drop-down, select the instance that has Dynamics 365 Guides installed.

3. Select the **Guides** app in the list. A new tab for the Guides model-driven app is opened.

    > [!NOTE]
    > The Guides model-driven app isn't intended as a replacement for authoring in the PC and HoloLens apps. If you use the model-driven app to create, update, or delete records, you might make Guides nonfunctional or prevent users from using the PC or HoloLens apps in the intended way. Currently, modification through the model-driven app isn't fully supported and should be reserved for experienced Dynamics 365 developers who are familiar with Microsoft Dataverse.

4. On the left side of the screen, select the up arrow next to **Main**, and then select **Settings**.

    ![User Settings.](media/data-opt-out-user-setting.PNG "User Settings")

5. Select **New**.

    ![Select New.](media/data-opt-out-new.PNG "Select New")

6. In the **New User Settings** screen, under **User Settings**, enter the following:

    - **Name:** Opt out for *[User name]*

    - **Record Guide Usage:** No

    - **Belongs To:** *[User name]*

    ![Filled-out form.](media/data-opt-out-filled-out-form.PNG "Filled-out-form")

7. Select **Save** at the top of the screen.

## See also

[Overview of analyzing and integrating Dynamics 365 Guides operations data](analytics-overview.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
