---
title: Set up Dynamics 365 Product Visualize on a new Dynamics 365 instance
description: Instructions to set up a Dynamics 365 instance and install the Dynamics 365 Product Visualize solution
author: sbmjais
ms.author: shjais
manager: shujoshi
ms.date: 07/29/2020
ms.service: crm-online
ms.topic: article
ms.reviewer:
---

# Set up Dynamics 365 Product Visualize on a new Dynamics 365 instance

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

Dynamics 365 Product Visualize requires an active Dynamics 365 instance. This topic provides step-by-step instructions for setting up a new Dynamics 365 trial instance and installing the Dynamics 365 Product Visualize solution.

> [!NOTE]
> If you have an existing Dynamics 365 instance, you can skip to [Step 2: Install the Dynamics 365 Product Visualize solution](#step-2-install-the-dynamics-365-product-visualize-solution) and start working with the solution immediately.

## Step 1: Get a Dynamics 365 trial instance

1. Go to [https://trials.dynamics.com/](https://trials.dynamics.com/).

2. Scroll down and select **Sign up here**.

    ![Sign up for a trial](media/trials-page.png "Sign up for a trial")

3. In the pop-up window, select **No, continue signing up**.

    ![Continue signing up](media/continue-step.png "Continue signing up")

4. In the **Let's set up your account** step, enter your email address, and then select **Next**.

    ![Enter your email to set up your account](media/wizard-step1.png "Enter your email to set up your account")

5. Select **Set up account**.

    ![Set up your account](media/wizard-step1_1.png "Set up your account")

6. In the **Tell us about yourself** step, enter your personal details and verify your phone number.

7. In the **Create your business identity** step, enter a domain name&mdash;for example, **productvisualize**&mdash;and check its availability. If the domain name is available, select **Next**.

    ![Create a domain name](media/wizard-step3.png "Create a domain name")

8. Create a user ID and password to sign in to your account, and then select **Sign up**.

    ![Create a user ID and password](media/wizard-step3_1.png "Create a user ID and password")

    > [!NOTE]
    > Store the user ID and password in a safe place; you'll need them later.

9. As soon as your account is set up, select **Let's go**.

    ![Finish setup](media/wizard-step4.png "Finish setup")

    After your account is created, you'll be redirected to [Power Platform admin center](https://admin.powerplatform.microsoft.com) to create a new environment.

10. In the **New environment** panel, enter the required details and select **Next**.

11. In the **Add database** panel, verify the information, and select **Save**.

    The environment and the database will be created. The state of the environment will be **PreparingInstance**. You must wait until it changes to **Ready**.

 > [!IMPORTANT]
 > In the following steps, you must use the credentials you created for your Dynamics 365 instance, if asked.

## Step 2: Install the Dynamics 365 Product Visualize solution

1. Go to the [Dynamics 365 Product Visualize app](https://appsource.microsoft.com/en-us/product/dynamics-365/mscrm.d365_product_visualize?tab=Overview) on Microsoft AppSource.

2. Select **Get it now**.

3. In the **One more thing...** pop-up window, select **Continue**.

    ![Select Continue to proceed with installation](media/continue-step-app.png "Select Continue to proceed with installation")

    You'll be redirected to the `https://port.crm.dynamics.com` page.

4. Under **Add the application to Dynamics 365**, select both check boxes, and then select **Agree**.

    ![Add the application to Dynamics 365](media/add-app-to-d365.png "Add the application to Dynamics 365")

    You'll be redirected to the Dynamics 365 admin center.

5. On the **Instances** tab, find the **Dynamics 365 Product Visualize** solution.

6. Check the status of the solution. If it says **Installation pending**, refresh the page until the status is changed to **Installed**.

## What's next

After you've finished the setup process, you'll have a Dynamics 365 trial instance with the Dynamics 365 Product Visualize Hub app installed. You can sign in to the Dynamics 365 Product Visualize Hub app and start adding products and 3D models, and creating mixed-reality sessions. More information: [Dynamics 365 Product Visualize Hub user guide](hub-user-guide.md)

### See also

[Dynamics 365 Product Visualize iOS app user guide](user-guide.md)<br>
[FAQ](faq.md)
