---
author: mamithan
description: Set up Dynamics 365 Product Visualize (in preview)
ms.author: mamithan
ms.date: 04/2/2019
ms.service: crm-online
ms.topic: article
title: Set up Dynamics 365 Product Visualize (in preview)
ms.reviewer: v-brycho
---

# Set up Dynamics 365 Product Visualize (in preview)

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

Microsoft Dynamics 365 Product Visualize (in preview) requires an active Dynamics 365 for Sales instance that's backed by a SharePoint site. This document provides step-by-step procedures for setting up a new trial instance of Dynamics 365 for Sales. 

After the Dynamics 365 for Sales instance is running, you'll need to add users, products, opportunities, and 3D models as described [in the Admin guide](admin-guide.md).

## Create a new tenant

The first step is to setup a new Azure Active Directory tenant. This ensures taht your Dynamics 365 Trial instance won't interfere with any existing instances and provides the ability to create new users with credentials separate from your corporate credentials.

1. Go to the Azure portal at \([https://ms.portal.azure.com](https://ms.portal.azure.com)) and sign in.

   > [!NOTE]
   > If your organization has multiple Azure subscriptions, select from the __Directory & Subscriptions__ menu in the upper-right corner of the page.
   
3. In the navigation menu, select **Create a Resource**.

4. In the **New Resource** window, select **Identity > Azure Active Directory**.

5. Give the organization a name and initial domain name.

6. Select **Create**. 

   > [!NOTE]
   > This may take several minutes until you see the **Success** message.
   
7. From the **Directory & Subscriptions** menu in the upper-right corner, select the newly created domain directory. 

## Add an admin user

After creating the Active Directory tenant, the next step is to add an admin user to the tenant. The admin user is responsible for creating additional users, assigning licenses, and initializing Dynamics 365. 

> [!NOTE] 
> We suggest creating a separate administrator account for each tenant.

1. In the Azure Portal \([https://ms.portal.azure.com](https://ms.portal.azure.com)), make sure your newly created organization is selected in the **Directory** field of the **Directory & Subscriptions** menu.

2. From the navigation menu on the left, select **Azure Active Directory**, and then select **Users**.

3. Select **New User** at the top of the page, and then fill in the following fields:

    * Name: Enter any name.
    
    * Username: Enter a fully qualified username (username@\<tenant>.onmicrosoft.com).
    
    * Directory Role: Global Administrator
    
4. Select **Show Password**, and then write down the temporary password.

5. Sign out, and then sign back in as the admin user.

6. If prompted, create a new password for the admin user.

## Add a Dynamics 365 Customer Engagement trial

Product Visualize integrates directly with Dynamics 365 for Sales, which enables your salespeople to seamlessly transition from essential customer data to an engaging sales experience that changes the way customers think about your products.

1. In a private browser window, go to [https://admin.microsoft.com](https://admin.microsoft.com).

2. Under **Billing**, select **Subscriptions**, and then select **Add Subscription**.

3. Search for **Dynamics 365 Customer Engagement** and then select **Start Free Trial**.

4. In the summary page, make sure you're signing-up for a Dynamics 365 Customer Engagement trial, select **Try Now**, and then select **Continue**.

## Assign licenses

The next step after signing up for the trial is to assign a license to the admin user. 

1. In a private browser window, go to [https://admin.microsoft.com](https://admin.microsoft.com).

2. In the navigation menu on the left, select **Users > Active Users**.

3. Double-click the name of the admin user you created earlier. 

4. Next to **Product Licenses**, select **Edit**.

5. Turn on the cicenses for **Dynamics 365 Customer Engagement** and **Office 365 Enterprise E3**.

6. Save the changes and close the **Users** dialog box.

## Set up the Dynamics 365 for Sales trial

The next step is to set up your instance of Dynamics 365 Customer Engagement. This procedure walks you through the manual installation of the Dynamics for Sales app, which generates an empty instance of the Dynamics Common Data Service for Apps. If you would prefer for a simpler set up procedure, refer to the note below.

1. Go to [https://admin.microsoft.com](https://admin.microsoft.com), and then from the **Admin Centers** list, select **Dynamics 365**.

2. A the page that appears:

    - Set the language to your preferred language.
    
    - Under **Select which scenario fits you best**, select **None of these**.
    
      > [!NOTE]
      > As an alternative, if you select **Sales** as the scenario, you can skip steps 4 - 7. If you choose this option, additional sample data will be installed that may not be relevant to your organization, however.
    
    - Set the currency to your preferred currency.
    
3. Select **Complete Setup**.

    > [!NOTE]
    > The setup process may take a few minutes.

4. Go back to the [Dynamics 365 Admin Portal](https://admin.microsoft.com).

5. On the **Instances** page, make sure the newly created instance is selected, and then select the **Edit** button next to the word **Solutions** in the gray box on the right.

6. In the list of available solutions, select **Dynamics 365 Sales Application**, and then select **Install**.

    > [!NOTE]
    > This process may take a while to complete. You can refresh the page to view the current status of your installation.


## Set up a SharePoint site

1. Go to [https://\<org>.crm.dynamics.com](), and then search for **Sales Hub** in the list of available applications.
    
2. Select the **Gear** icon in the upper-right corner of the page, and then select **Advanced Settings**.

3. At the top of the page, select the down arrow next to **Settings**, and then select **Document Management**.

4. Select the **Enable Server-Based SharePoint Integration** button. 

5. Continue through the setup. When prompted, enter the URL for your SharePoint ([https://\<org name>.sharepoint.com]()).

6. When complete, go back to the **Document Management** settings page, and then select **Document Management Settings**.

7. Enter the URL for your SharePoint site, if it isn't filled in by default. Then select **Next**.

8. Continue through the setup screens using the default values.

   It will take about a minute for Dynamics 365 to set up the SharePoint connection.

   > [!NOTE]
   > If you opted to use the automated **Sales** setup earlier you can skip the steps of Enabling Server-Based SharePoint Integration.

## What's' next?

When you're finished setting everything up, you'll have an Azure Active Directory tenant complete with Microsoft Office 365 and Microsoft Dynamics 365 Customer Engagement. At this point you can start adding opportunities, products, and 3D models to Dynamics 365 for Sales. For more information, see the [Admin guide](admin-guide.md).

### See also

[User Guide](user-guide.md)<br>
[FAQ](faq.md)<br>

