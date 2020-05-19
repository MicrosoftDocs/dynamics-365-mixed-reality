---
title: Set up Dynamics 365 Product Visualize on a new Dynamics 365 Sales instance
author: mamithan
description: Associate a Dynamics 365 Sales instance with a SharePoint site
ms.author: mamithan
ms.date: 12/22/2019
ms.service: crm-online
ms.topic: article
ms.reviewer: v-brycho
---

# Set up Dynamics 365 Product Visualize

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

Dynamics 365 Product Visualize requires an active Dynamics 365 Sales instance that's associated with a SharePoint site. This topic provides step-by-step procedures for setting up a new Sales trial instance. After the instance is running, see the [Administrator guide](admin-guide.md) instructions for adding users, products, opportunities, and models. The administrator guide also includes important information about downloading the Dynamics 365 Product Visualize solution package that connects the Sales instance with Dynamics 365 Product Visualize. 

## Create a new organization

The first thing you need to do is create a new Azure Active Directory (Azure AD) organization. This new organization provides a safe environment to try out Dynamics 365 Product Visualize that won't interfere with any existing Dynamics 365 instances. You can also use this organization to create and manage users, separate from your business organization.

   > [!NOTE]
   > If you prefer to add Sales to an existing Azure AD organization, skip ahead to the section [Add a Dynamics 365 Customer Engagement trial](#add-a-dynamics-365-customer-engagement-trial).<!--Please see the note about "Customer Engagement" in that section. -->

1. Sign in to the Azure portal at https://ms.portal.azure.com.

2. If your organization has multiple Azure<!--Should this be "Azure AD"?--> subscriptions, select **Directory & Subscription** ![Directory and Subscription](media/directory-and-subscription-button.PNG "Directory and Subscription") in the upper-right corner of the page to view the list of available subscriptions.

3. In the left pane, select **Create a resource** > **Identity** > **Azure Active Directory**.

   ![Create a resource](media/create-resource.PNG "Create a resource")

4. Under **Create directory**, give the organization a name and an initial domain name.

   ![Name and domain name](media/name-and-domain-name.PNG "Name and domain name")

5. Select **Create**. You might need to wait several minutes while the directory is created.

6. Select **Click here to manage your new directory**.

   ![Click to manage new directory link](media/manage-directory-link.PNG "Click to manage new directory link")

## Add an admin user

After creating the new organization, the next step is to add an admin user for the organization. The admin user is responsible for creating additional users, assigning licenses, and initializing Dynamics 365. As the creator of this organization, you can use your work account to manage the system, but we recommend creating a separate administrator account for each organization.

1. In the left pane, select **Azure Active Directory**, and then select **Users**.

   ![Azure Active Directory](media/azure-active-directory.PNG "Azure Active Directory")

2. Select **New User** at the top of the page, and then fill in the following fields:

    - **Name**: Enter any name.

    - **Username**: Enter a fully qualified username (<username>@\<tenant>.onmicrosoft.com).

    - **Directory Role**: Global administrator

3. Select **Show Password**, and then write down the temporary password.

4. At the bottom of the page, select **Create** to finish creating the user.

## Add a Dynamics 365 Customer Engagement trial
<!--Please note question below about "Customer Engagement" -->
Dynamics 365 Product Visualize integrates directly with Sales, which enables your salespeople to seamlessly transition from vital customer data into an engaging sales experience that changes the way customers think about your products.

1. In a private browser window, go to the Microsoft 365 admin center at [https://admin.microsoft.com](https://admin.microsoft.com).

2. Sign in with the administrator credentials you created in the previous procedure, and, if prompted, set a new password.

3. In the left pane, select **Billing**, and then select **Purchase services**.

   ![Purchase services](media/billing_purchase_services.png "Purchase services")

4. Search for **Dynamics 365 Customer Engagement Plan**, and then select the **Dynamics 365 Customer Engagement Plan** panel from the results.<!--According to the Dynamics Style Guide, this plan was phased out as of October 1, 2019. It says "specifically, never use 'Dynamics 365 Customer Engagement.'" I'm not sure what to suggest in its place. Please see https://styleguides.azurewebsites.net/Styleguide/Read?id=2858&topicid=45368 and https://styleguides.azurewebsites.net/Styleguide/Read?id=2858&topicid=44518-->

   ![Dynamics 365 Customer Engagement plan](media/purchase_services_365_engagement_plan.png "Dynamics 365 Customer Engagement plan")

5. On the summary page, select **Get free trial**.

6. On the checkout page, select **Try now**. After this is processed, select **Continue**.

## Assign licenses

Before continuing, make sure the Dynamics 365 Customer Engagement<!--or...? --> license has been assigned to the admin user.

1. Go to the Microsoft 365 admin center at [https://admin.microsoft.com](https://admin.microsoft.com). In the left pane, select **Users** > **Active Users**.

2. Select the name of the admin user you created earlier.

3. In **Licenses and Apps**, under **Licenses**, make sure that **Dynamics 365 Customer Engagement Plan** is selected.<!--In the following graphic, is "Chris Green" a name from sample data? (Does this product even include sample data?) It's not a name in our Dynamics-specific list. -->

   ![Edit licenses](media/user_licenses.png "Edit licenses")

5. Save your changes, and then close the dialog box.

## Set up the Dynamics 365 Sales trial

The next step is to set up the Dynamics 365 Customer Engagement<!--or...? --> instance. This procedure provides step-by-step instructions for manually installing Sales, which generates a completely empty instance of Common Data Service. 

1. In the Microsoft 365 admin center at [https://admin.microsoft.com](https://admin.microsoft.com), in the left pane, in the drop-down list for **Admin Centers**, select **All admin centers**.

2. On the **All admin centers** page, select the **Dynamics 365** panel.

3. On the page that appears:

    - Set the language to your preferred language.

    - Under **Select which scenario fits you best**, select **None of these**.

    - Set the currency to your preferred currency.

4. Select **Complete Setup**, and then wait for the initial setup process to be completed.

   ![Complete Setup](media/complete-setup.PNG "Complete Setup")

5. In the left pane, in the **Admin Centers** list, select **Dynamics 365 Admin Portal**.

   On the **Instances** page, you should see your newly created instance selected and some properties in a gray box on the right. Your new solution is still being set up. Wait for setup to be completed before moving on to the next step.

   > [!NOTE]
   > It can take around 10 minutes for the setup process to finish. You'll know the process is complete when you see **CRM Hub** listed under **Solutions** for your instance. Refresh the page periodically to check the status.

6. Select the small **Edit** icon next to the word **Solutions** in the gray box on the right.

   ![Select the Edit icon](media/s7.png "Select the Edit icon")

7. In the list of available solutions, find **Dynamics 365 Sales Application**, and then select **Install**.

8. Review the terms of service. When you're ready, select the check box to confirm that you approve. This starts the installation.

   > [!NOTE]
   > This process might take a while to be completed. You can refresh the page to view the current status of the installation.

## Set up a SharePoint site

1. Go to the Sales Hub app for your newly created Dynamics 365 instance. To do this:

    1. On the admin center page, select **Open** next to your organization name in the gray box.

    2. Select **Sales Hub** in the list of available applications.

2. Select **Settings** in the upper-right corner of the page, and then select **Advanced Settings**.

3. In the navigation bar at the top of the page, select the arrow next to **Settings**, and then select **Document Management**.

   ![Document Management settings](media/sharepoint.PNG "Document Management settings")

4. Select **Enable Server-Based SharePoint Integration** to set up the connection to SharePoint.

   > [!NOTE]
   > If you opted to use the automated **Sales** setup option earlier, you can skip the steps to enable server-based SharePoint integration.

5. Continue through the setup. When prompted, enter the URL for your SharePoint instance ([https://\<org name>.sharepoint.com]()).

   > [!IMPORTANT]
   > Be sure to enter the full URL for your SharePoint instance, including `https://`.

6. When the connection has been set up<!--Edit okay? -->, return to the **Document Management** settings page, and then select **Document Management Settings**.

7. Enter the URL for your SharePoint site if it hasn't been filled in by default, and then select **Next**.

8. Continue through setup using the default values for the remaining options.

   Dynamics 365 automatically creates SharePoint folders for Dynamics 365 entities.

9. Close the window when you're done.

## What's next?

After you've finished the setup process, you'll have an Azure AD organization complete with Dynamics 365 Customer Engagement<!--or...? --> and SharePoint. At this point, you can start adding opportunities, products, and models to Sales. For more information, see the [Administrator guide for Dynamics 365 Product Visualize](admin-guide.md). The administrator guide also includes important information about downloading the Dynamics 365 Product Visualize solution package that connects the Sales instance with Dynamics 365 Product Visualize. 

### See also

[User guide](user-guide.md)<br>
[FAQ](faq.md)
