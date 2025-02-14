---
author: prashantyvr
description: In this step of the setup process, you create a Microsoft Dataverse environment and install the Dynamics 365 Guides solution.
ms.author: prashan
ms.date: 02/13/2025
ms.topic: how-to
title: Install the Dynamics 365 Guides solution 
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Install the Dynamics 365 Guides solution

After buying a Microsoft Dynamics 365 Guides or Field Service license, create an environment where you can install the Guides solution.

If you have another environment that you want to use (for example, an instance in your company's Dynamics 365 tenant), skip to [**Install and configure the solution**](#install-and-configure-the-solution). Otherwise, perform the following steps to set up a production environment.

## Prerequisites

- [System Administrator role](/power-platform/admin/database-security) in Power Platform admin center.
- A license that [allows environment creation](/power-platform/admin/create-environment#who-can-create-environments) such as Power Apps.

## Set up a production environment

1. Go to the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments).

1. [Create a new environment](/power-platform/admin/create-environment#create-an-environment-with-a-database) and select **Production** for **Type** and **Yes** to **Add a Dataverse data store**.

1. In the **Region** field, keep the default setting.

   > [!IMPORTANT]
   > If you set up a Dataverse environment instance in a different region than your default Microsoft Entra tenant region, the Dynamics 365 Guides model-driven app won't be available to install. If you'd like to set up a Dataverse environment instance in a region other than your default region, you must first [contact Microsoft support](https://support.serviceshub.microsoft.com/supportforbusiness) and ask to make your tenant into a multi-geo tenant for Power Platform.  

1. Select **Next** and select the following information:

   - **Language**: Your organization's supported language.
   - **Currency**" Your organization's currency.
   - **Security group**: If you have a security group set up, select the group or select **None**.
   - **Enable Dynamics 365 apps**: Yes.
   - **Automatically deploy these apps**: Guides

1. Select **Save**.

   When the new environment is active, **Ready** appears in the **State** field for the environment. The Guides solution is automatically installed.

1. [Assign licenses and add users.](add-users.md)

## Install and configure the solution

If you have an environment already created, perform the following steps to install the Dynamics 365 Guides solution.

1. In the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), in the left pane, select **Resources** > **Dynamics 365 apps**, select **Dynamics 365 Guides** in the list, and then select **Install**. It might take a few minutes for **Dynamics 365 Guides** to appear in the list.

1. In the **Install Dynamics 365 Guides** dialog box, select an environment, select the **I agree to the terms of service** check box, and then select **Install**.

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