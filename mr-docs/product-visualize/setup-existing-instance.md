---
author: mamithan
description: Set up Dynamics 365 Product Visualize on an existing Dynamics 365 for Sales instance
ms.author: mamithan
ms.date: 04/1/2019
ms.service: crm-online
ms.topic: article
title: Set up Dynamics 365 Product Visualize on an existing Dynamics 365 for Sales instance
ms.reviewer: v-brycho
---

# Set up Dynamics 365 Product Visualize on an existing Dynamics 365 for Sales instance

You can connect Microosft Dynamics 365 Product Visualize to a new or existing Dynamics 365 for Sales instance. This topic explains how to set it up on an existing Dyanmics 365 for Sales instance. If you don't already have Dynamics 365 for Sales, follow the instructions in the [Setup topic](setup.md) to sign up for a trial and get started today. 

## Minimum requirements

Existing Dynamics 365 for Sales instances must meet the following minimum requirements to connect to Product Visualize:

- The Dynamics 365 for Sales version, must be 9.0 or later.

- Server-based SharePoint document management muste be enabled.

- Products associated with 3D models must be in the GLB format.

    > [!IMPORTANT]
    > Server-based SharePoint integration is the prefered method for integrating Dynamics 365 for Sales with SharePoint. SharePoint Online has removed the code-based sandbox solution and the SharePoint List Component can no longer be installed. Product Visualize does not offer support for existing instances using the List Component.

### Verify the Dynamics 365 for Sales version

1. In a browser window, go to your organization's Sales or Sales Hub instance [https://\<org name>.crm.dynamics.com]().

2. In the upper-right corner of the screen, click the **Settings** button, and then select **About**.

3. The **Server version** listed must be greater than **9.0** to work with Product Visualize.

   ![Server version](media/sales-version.PNG "Server version")

## Set up SharePoint document management

   > [!NOTE] 
   > If you already have server-based SharePoint integration enabled in your instance, you can skip this step.

### Enable SharePoint integration

1. In a browser window, go to your organization's Sales or Sales Hub instance [https://\<org name>.crm.dynamics.com]().

2. Select the **Settings** button in the upper-right corner of the page, and then select __Advanced Settings__.

3. In the navigation bar at the top of the page, select the down arrow next to __Settings__, and then select __Document Management__.

   ![Document Management settings](media/sharepoint.PNG "SharePoint")

4. Select __Enable Server-Based SharePoint Integration__ to set up the connection to SharePoint.

5. Continue through the setup. When prompted, enter the URL for your SharePoint ([https://\<org name>.sharepoint.com]()).

   > [!IMPORTANT]
   > Be sure to enter the full URL for your SharePoint instance, including `https://`.

6. When complete, return to the __Document Management__ settings page, and then select __Document Management Settings__.

7. Enter the URL for your SharePoint site if it isn't filled in by default. Then select __Next__.

8. Continue through the setup using the default values for the remaining options.

   Dynamics 365 will automatically create SharePoint folders for the Dynamics 365 entities. 

9. Close the window when done.

### Enable SharePoint document management

1. In a browser window, go to your organization's Sales or Sales Hub instance [https://\<org name>.crm.dynamics.com]().

2. In the upper-right corner of the screen, select the **Settings** button, and then select **Advanced Settings**.

3. In the **Document Management** settings page, select **Document Management Settings**.

4. Enter the URL for your SharePoint site, if it isn't filled in by default. Then select __Next__.

5. Continue through the setup using the default values for the remaining options.

   Dynamics 365 will automatically create SharePoint folders for the Dynamics 365 entities. Close the window when complete.

### Grant SharePoint permission

1. Go to the SharePoint site you just associated with your Dynamics 365 for Sales instance.

2. In the upper-right corner of the SharePoint site's homepage, select **Share Site**.

3. Add users or groups from the Search bar.

4. Select **Share**.

## Add Models to Your Products

1. In a browser window, go to the Product List in the Sales or Sales Hub applications.

2. Open a product by selecting the product name.

3. On the __Related__ tab, select __Documents__ to go to a view of the SharePoint Document location for that product.

4. In the __Open Location__ drop-down list, select __Documents on Default Site 1__ to open the SharePoint location outside of Dynamics 365 for Sales.

5. Drag and drop your Model folder into this location. It will automatically show up in Product Visualize. Models should be added with the following folder structure:
    * \<Product>
      * \<Model Name> (Folder)
        * \<Model Name>.gltf
        * Thumbnails (Folder)
            * \<ModelName>.png
      *  \<Model Name> (Folder)
         * \<Model Name>.gltf
         * Thumbnails (Folder)
            * \<ModelName>.png

   > [!IMPORTANT]
   > SharePoint folders are created when you first visit a product's documents through the Dynamics for Sales interface. Once the folder has been created, you can access the folder directly from the SharePoint site.

## Accept app permissions

The Product Visualize mobile app requires permission to access the Dynamics 365 for Sales and SharePoint instances. As a global administrator for the trial tenant you can grant access to the entire organization so that each user doesn't have to do it individually.

1. Download the __Microsoft Dynamics 365 Product Visualize__ app from the iOS App Store.

2. Open the app, select __Sign In__, and then sign in with the trial environment's administrator credentials.

3. When prompted for permissions, select __Consent on behalf of your organization__.

4. Select __Accept__ to return to the app.

## Next steps
You're now ready to use Microsoft Dynamics 365 Product Visualize with all of your sales opportunities. The Product Visualize mobile app can be downloaded from the iOS App Store. Users can sign in with the same Azure Active Directory credentials that they use to connect to Dynamics 365 for Sales.
  
