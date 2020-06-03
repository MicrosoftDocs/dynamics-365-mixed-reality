---
title: Setup a Dynamics 365 Environment
author: bencorn
description: How to setup an environment for the Asset Capture Public Preview
ms.author: becorn
ms.date: 5/30/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Setup a Dynamics 365 Environment

This tutorial is the first of a series. As you progress through the series, you will create an environment and install the app, add users to the environment, learn how to import and create asset records, capture pictures with spatial markup, review the captured pictures from the Dynamics 365 Remote Assist app, and learn how to create Power Automate Flows to automate business processes with asset capture data.

## Prerequisites

To complete this article, you need:

- **A Dynamics 365 Remote Assist subscription**, this enables you to create environments and install the app.
- **Ability to manage environments in Power Platform Admin Center**. This tutorial covers creating Dynamics 365 environments and installing apps. Admin access is required (Dynamics 365 service admin, Global admin, or Power Platform service admin).
- **Available database capacity**. If you are creating a new environment for Remote Assist, you will need at least 1GB of available database capacity to do so. Paid subscriptions of Remote Assist provide default tenant capacity. Learn more about the capacity model here: [New Common Data Service storage capacity
](https://docs.microsoft.com/power-platform/admin/capacity-storage).

> [!IMPORTANT]
> Trial subscriptions of Remote Assist can be used for the public preview if your organization has **existing Dynamics 365 subscriptions** that include apps such as Field Service or Customer Service. The in-app 90 day viral trial is not compatible with this preview.

## Install Dynamics 365 Remote Assist model-driven app

There are a few ways you can install the Dynamics 365 Remote Assist app:

1. Create an entirely new Dynamics 365 environment for Remote Assist.
2. Use an existing environment to install the Remote Assist app on. This environment must be **Dynamics 365 apps enabled**.

### Create a new environment

1. Sign in to the [Power Platform Admin Center](https://admin.powerplatform.com) as an admin (Dynamics 365 service admin, Global admin, or Power Platform service admin).
2. In the navigation pane, select **Environments**, and then select **New**.
3. Enter a name, choose production or sandbox, and choose Yes to **Create a database for this environment**. Select **Next**.
4. Select Yes to **Enable Dynamics 365 apps** and then select **Remote Assist** from the dropdown and select **Save**. This will create an environment and automatically install the Remote Assist app.

> [!IMPORTANT]
> If you do not see Remote Assist in the dropdown, it may not be available in your region yet for automatic deployment. If so, leave the toggle enabled but don't select any apps in the dropdown and proceed with creating the environment. Once created, follow the instructions below to **Use an existing environment**.

For more detailed documentation on creating Dynamics 365 Environments refer to this doc: [Create and manage environments in the Power Platform admin center](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center)

### Use an existing environment

1. Sign in to the [Power Platform Admin Center](https://admin.powerplatform.com) as an admin (Dynamics 365 service admin, Global admin, or Power Platform service admin).
2. In the navigation pane, select **Resources** > **Dynamics 365 apps**.
3. Find the Dynamics 365 Remote Assist app, select the three dots, and then select **Install**.
![Screenshot of Power Platform Admin Center.](./media/AC_PPAC_InstallApp.png "Admin Portal")
4. Select an environment, review the packages to be installed, agree to the terms of service, and then select **Install**. This process may take a while.

> [!IMPORTANT]
> The environment selected must be **Dynamics 365 apps enabled**. For example, the default environment cannot be used. If it isn't compatible, the installation will fail. Choose another environment that is compatible or create a new environment with Dynamics 365 apps enabled.

## Next steps

Congratulations, you've installed the Dynamics 365 Remote Assist app. The app is now accessible by opening the environment and selecting the Remote Assist app or from [https://home.dynamics.com/](https://home.dynamics.com). Find more information about accessing Unified Interface apps here: [About Unified Interface for model-driven apps in Power Apps](https://docs.microsoft.com/power-platform/admin/about-unified-interface)

The next tutorial goes into detail about adding users to the preview so they can interact with data and enable the preview in the HoloLens 2.

> [!div class="nextstepaction"]
> [Add users to the preview](./asset-capture-add-users.md)