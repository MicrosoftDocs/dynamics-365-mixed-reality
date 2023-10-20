---
author: davepinch
description: In this step of the setup process, you create a Microsoft Dataverse environment and install the Dynamics 365 Guides solution.
ms.author: davepinch
ms.date: 10/20/2023
ms.topic: how-to
title: Install the Dynamics 365 Guides solution 
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Install the Dynamics 365 Guides solution

After buying a Microsoft Dynamics 365 Guides subscription, create an environment where you can install the Guides solution.

If you already have an environment that you want to use (for example, an instance in your company's Dynamics 365 tenant), skip to [**Install and configure the solution**](#install-and-configure-the-solution).

## Prerequisites

- [System Administrator role](/power-platform/admin/database-security) in Power Platform admin center.
- Assigned Dynamics 365 Guides license with Power Apps or a Power Apps license.

## Set up a production environment

1. Go to the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments).

1. [Create a new environment](/power-platform/admin/create-environment#create-an-environment-with-a-database) and select **Production** for **Type** and **Yes** to **Add a Dataverse data store**.

   > [!IMPORTANT]
   > The Dynamics 365 Guides solution can also be installed on a trial environment. **We don't recommend that you use a trial environment, because that environment, together with all your content, is automatically disabled after the 30-day trial period expires.** You have a seven-day grace period to upgrade to a production environment or migrate your content to another environment.

1. In the **Region** field, keep the default setting.

   > [!IMPORTANT]
   > If you set up a Dataverse environment instance in a different region than your default Azure Active Directory tenant region, the Dynamics 365 Guides model-driven app won't be available to install. If you'd like to set up a Dataverse environment instance in a region other than your default region, you must first [contact Microsoft support](https://support.serviceshub.microsoft.com/supportforbusiness) and ask to make your tenant into a multi-geo tenant for Power Platform.  

1. Select **Next**. For the database, select your language and currency, and set the **Enable Dynamics 365 apps** option to **Yes**. Keep the default values for the other fields. Then select **Save**.

   When the new environment is active, **Ready** appears in the **State** field for the environment.

1. Go to **Install and configure the solution**.

## Install and configure the solution

1. In the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), in the left pane, select **Resources** > **Dynamics 365 apps**, select **Dynamics 365 Guides** in the list, and then select **Install**.

    > [!NOTE]
    > It might take a few minutes for **Dynamics 365 Guides** to appear in the list.

1. In the **Install Dynamics 365 Guides** dialog box, select an environment, select the **I agree to the terms of service** check box, and then select **Install**.

   > [!NOTE]
   > If you don't see your environment and you have a valid Guides license, you might have installed Dynamics 365 Guides on a trial environment that has expired. You can go to the  [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), select your trial environment, and [switch it to a production environment](/power-platform/admin/switch-environment).

    In the Power Platform admin center, the following message is shown: "Dynamics 365 Guides installation started at \<*time*\>, \<*date*\> by \<*name*\> Account."

    While the solution is being installed, **Installing** appears in the **Status** field for the app. After the app has been installed, the **Status** field is updated to **Installed**.

    > [!NOTE]
    > The installation process can take up to one hour. The amount of time varies, depending on the time of day and the region. If the status hasn't changed after an hour, refresh the page.

## Microsoft platforms and Guides

[!INCLUDE [microsoft-platforms](../includes/microsoft-platforms-dependency.md)]

For more information, see [Manage Dynamics 365 apps](/power-platform/admin/manage-apps).

## Next step

- [Assign licenses and add users](add-users.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]