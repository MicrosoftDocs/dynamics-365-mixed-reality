---
title: Set up Dynamics 365 Product Visualize on an existing Dynamics 365 Sales instance
description: Learn how to set up Dynamics 365 Product Visualize on an existing Dynamics 365 Sales instance.
author: sbmjais
ms.author: shjais
manager: shujoshi
ms.date: 06/08/2020
ms.service: crm-online
ms.topic: article
ms.reviewer:
---

# Set up Dynamics 365 Product Visualize on an existing Dynamics 365 Sales instance

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

You can connect Dynamics 365 Product Visualize to a new Dynamics 365 Sales instance or an existing instance. This topic explains how to set it up on an existing Sales instance. If you don't already have Dynamics 365 Sales, you can set up a free trial. More information: [Set up Dynamics 365 Product Visualize](setup.md) 

## Minimum requirements

Existing Sales instances must meet the following minimum requirements to connect to Dynamics 365 Product Visualize:

- The Sales version must be 9.0 or later.

- Server-based SharePoint document management must be enabled.

- Products associated with 3D models must be in the GLB format.

    > [!IMPORTANT]
    > Server-based SharePoint integration is the preferred method for integrating Dynamics 365 Sales with SharePoint. You can't use the SharePoint List Component with SharePoint Online. Dynamics 365 Product Visualize doesn't support existing instances that use the List Component.

### Verify the Dynamics 365 Sales version

1. In a browser window, go to your organization's Sales or Sales Hub instance [https://\<org name>.crm.dynamics.com]().

2. In the upper-right corner of the screen, select **Settings**, and then select **About**.

   ![Server version](media/sales-version.PNG "Server version")

## Set up SharePoint document management

   > [!NOTE] 
   > If you already have server-based SharePoint integration enabled in your instance, you can skip this step.

### Enable SharePoint integration

1. In a browser window, go to your organization's Sales or Sales Hub instance [https://\<org name>.crm.dynamics.com]().

2. Select **Settings** in the upper-right corner of the page, and then select **Advanced Settings**.

3. In the navigation bar at the top of the page, select the down arrow next to **Settings**, and then select **Document Management**.

   ![Document Management settings](media/sharepoint.PNG "Document Management settings")

4. Select **Enable Server-Based SharePoint Integration** to set up the connection to SharePoint.

5. Continue through the setup. When prompted, enter the URL for your SharePoint site: ([https://\<org name>.sharepoint.com]()).

   > [!IMPORTANT]
   > Be sure to enter the full URL for your SharePoint site, including `https://`.

6. When the connection setup is complete, return to the **Document Management** settings page, and then select **Document Management Settings**.

7. Enter the URL for your SharePoint site if it isn't filled in by default, and then select **Next**.

   ![Enter your SharePoint site URL in Document Management settings](media/document-management-settings.PNG "Enter your SharePoint site URL in Document Management settings")

8. Continue through setup by using the default values for the remaining options.

   SharePoint folders will automatically be created for the Dynamics 365 Sales entities.

9. Close the window when you're done.

### Grant SharePoint permission

1. Go to your trial's SharePoint site: [https://\<org name\>.sharepoint.com]().

2. In the upper-right corner of the page, select **Share site**.

   ![Share site command](media/share-site.PNG "Share site command")

3. In the **Share** window, search for the group you created earlier, and then select the group name to add it to the site.

4. Grant the group Edit permission by selecting the small arrow under the group name.

   ![Edit share site](media/edit-share-site.PNG "Edit the share site settings")

5. Select **Share** to finish granting group access to SharePoint.

## Add 3D models to your products

1. In a browser window, go to the Sales or Sales Hub application, and then in the left pane, under **Collateral**, select **Products**.

   ![Product navigation](media/products-navigation.PNG "Product navigation")

2. Open a product by selecting the product name.

3. On the **Related** tab, select **Documents** to go to a view of the SharePoint document location for that product.

   ![Documents link on the Related tab](media/related-documents.PNG "Documents link on the Related tab")

4. In the **Open Location** drop-down list, select **Documents on Default Site 1** to open the SharePoint location outside of Sales.

   ![Open location](media/open-location.PNG "Open location")

5. Drag your model file (as a GLB file) into this location. It will automatically show up in Dynamics 365 Product Visualize.

   > [!IMPORTANT]
   > SharePoint folders are created when you first visit a product's documents through the Sales interface. After the folder has been created, you can access the folder directly from the SharePoint site.

6. Optional: SharePoint automatically provides a thumbnail for Dynamics 365 Product Visualize; however, if you want to add a custom thumbnail to a model, drag a PNG image with the same name as the model into this location. For example, ModelName1.png would be a custom thumbnail for ModelName1.glb.

## Install the Dynamics 365 Product Visualize solution

The Dynamics 365 Product Visualize solution is a package that customizes your Sales installation to support Dynamics 365 Product Visualize.

### Import the Dynamics 365 Product Visualize solution

1. [Download the **Dynamics 365 Product Visualize** solution](https://download.microsoft.com/download/F/D/E/FDEE4BA0-F7E5-4FBD-80C1-E670F9F397BA/ProductVisualize.Solution.zip).

2. Go to the Dynamics 365 Sales Hub.

2. Select **Settings**, and then select **Advanced Settings**.

3. In the **Settings** drop-down list at the top of the page, select **Solutions**.

5. Select **Import**, and then select the solution (.zip file) you downloaded.

   ![Import the solution](media/import-solution.PNG "Import the solution")
 
6. In the **Solution Information** dialog box, select **Import** to begin the import process.

   ![Import information](media/import-information.PNG "Import information")
   
    > [!NOTE]
    > Importing a solution will replace any existing versions of that solution.
    
    After the import process is completed, you'll see the **Importing Solution** dialog box.

   ![Import complete](media/import-complete.PNG "Import complete")

7. Select **Close**.

## What's next?

You're now ready to use Dynamics 365 Product Visualize with all your sales opportunities. You can download the Dynamics 365 Product Visualize mobile app from the Apple App Store. You can sign in by using the same Azure Active Directory (Azure AD) credentials that you use to connect to Sales.
  
### See also

[User guide](user-guide.md)<br>
[FAQ](faq.md)
