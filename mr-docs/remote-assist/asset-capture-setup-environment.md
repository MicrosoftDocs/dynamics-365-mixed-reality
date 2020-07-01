---
title: Set up a Dynamics 365 environment to use asset capture in Remote Assist
author: bencorn
description: How to set up an environment for the Asset Capture Public Preview
ms.author: becorn
ms.date: 07/01/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Setup a Dynamics 365 environment to use asset capture in Remote Assist

This tutorial is the first of a series. As you progress through the series, you'll:

1. Create an environment and install the app
2. Add users to the environment
3. Learn how to import and create asset records
4. Capture pictures with spatial markup
5. Review the captured pictures from the Remote Assist model-driven app
6. Learn how to create Power Automate flows to automate business processes with captured asset data.

## Prerequisites

To complete the steps article, you need:

- **A Dynamics 365 Remote Assist subscription**, which enables you to create environments and install the app.
- **Ability to manage environments in Power Platform Admin Center**. This tutorial covers creating Dynamics 365 environments and installing apps. Admin access is required (Dynamics 365 service admin, global admin, or Power Platform service admin).
- **Available database capacity**. If you're creating a new environment for Remote Assist, you'll need at least 1 GB of available database capacity. Paid subscriptions of Remote Assist provide default tenant capacity. Learn more about the capacity model here: [New Common Data Service storage capacity
](https://docs.microsoft.com/power-platform/admin/capacity-storage).

> [!IMPORTANT]
> Trial subscriptions of Remote Assist can be used for the public preview if your organization has **existing Dynamics 365 subscriptions** such as Field Service, Customer Service, or paid Power Apps plans. The in-app 90 day viral trial is not compatible with this preview.

## Install Dynamics 365 Remote Assist model-driven app

There are a couple ways you can install the Dynamics 365 Remote Assist app:

- Create an entirely new Dynamics 365 environment for Remote Assist.
- Use an existing environment to install the Remote Assist app on. This environment must be **Dynamics 365 apps enabled**.

### Create a new environment

1. Sign in to the [Power Platform admin center](https://admin.powerplatform.com) as an admin (Dynamics 365 service admin, Global admin, or Power Platform service admin).
2. In the navigation pane, select **Environments**, and then select **New**.
3. Enter a name, choose production or sandbox, and choose **Yes** for **Create a database for this environment**. Select **Next**.
4. Select **Yes** for **Enable Dynamics 365 apps** and then select **Remote Assist** from the dropdown and select **Save**. This will create an environment and automatically install the Remote Assist app. If you encounter an issue, see [the troubleshooting](#troubleshooting) section in this article.

For more detailed documentation on creating Dynamics 365 environments, see: [Create and manage environments in the Power Platform admin center](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center)

### Use an existing environment

1. Sign in to the [Power Platform Admin center](https://admin.powerplatform.com) as an admin (Dynamics 365 service admin, Global admin, or Power Platform service admin).
2. In the navigation pane, select **Resources** > **Dynamics 365 apps**.
3. Find the Dynamics 365 Remote Assist app, select the three-dots (ellipses) icon, and then select **Install**.
![Screenshot of Power Platform Admin center.](./media/AC_PPAC_InstallApp.png "Admin Portal")
4. Select an environment, review the packages to be installed, agree to the terms of service, and then select **Install**. This process may take a while.

> [!IMPORTANT]
> The environment selected must be **Dynamics 365 apps enabled**. For example, the default environment cannot be used. If it isn't compatible, the installation will fail. Choose another environment that is compatible or create a new environment with Dynamics 365 apps enabled.

## Next steps

You've installed the Dynamics 365 Remote Assist app! You can get to the app by opening the environment and selecting the Remote Assist app or from [https://home.dynamics.com/](https://home.dynamics.com). Find more information about accessing Unified Interface apps here: [About Unified Interface for model-driven apps in Power Apps](https://docs.microsoft.com/power-platform/admin/about-unified-interface).

The next tutorial goes into detail about adding users to the preview so they can interact with data and enable the preview in the HoloLens.

> [!div class="nextstepaction"]
> [Add users to the preview](./asset-capture-add-users.md)

## Troubleshooting

### Can't enable Dynamics 365 apps

If you aren't able to toggle **Enable Dynamics 365 apps** during environment creation, ensure you have an active Dynamics 365 Remote Assist subscription. Subscriptions can be viewed in [Microsoft 365 Admin Center](https://www.admin.microsoft.com).

### Not enough capacity to create environments

Environment creation requires at least 1 GB of available database capacity. Paid subscriptions of Remote Assist provide a default tenant entitlement of 10 GB of database capacity (if Remote Assist is your first Dynamics 365 subscription). If you are on a trial and don't have any existing Dynamics 365 subscriptions that grant database capacity, you will not be able to evaluate the preview. Learn more about capacity: [New Common Data Service storage capacity
](https://docs.microsoft.com/power-platform/admin/capacity-storage)

### The Remote Assist app isn't showing up in Power Platform Admin center

1. Check to ensure you have an active Dynamics 365 Remote Assist subscription.
2. Try assigning a Remote Assist license to your account from [Microsoft 365 Admin center](https://admin.microsoft.com) to force a license sync to occur. Wait 5 minutes and see if the app appears in [Power Platform Admin center](https://admin.powerplatform.com). The license can be unassigned afterwards.
3. If the steps above do not resolve the issue, file a **support request** by going to [Power Platform Admin center](https://admin.powerplatform.com) > **Help + support** > **New support request**.

### The Remote Assist model-driven app failed to install because of missing dependencies

This will occur if you try installing Remote Assist in an environment that is not **Enabled for Dynamics 365 apps**. Try installing the app in an environment where other Dynamics apps are installed, such as Field Service or Sales, or create a new environment that is enabled for Dynamics 365 apps. Learn more: [Create a new environment](#install-dynamics-365-remote-assist-model-driven-app)
