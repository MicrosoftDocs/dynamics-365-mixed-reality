

# Working with an Existing Dynamics Instance
Product Visualize easily connects to new and existing instances of Dynamics 365 for Sales. If you do not already have Dynamics 365 for Sales, follow the instructions in the Setup guide to sign-up for a trial and get started today. Existing instances must meet the minimum requirements in order to connect to Product Visualize.

## Minimum Requirements
1. Dynamics 365 For Sales V.9 or above

2. Server-Based SharePoint Document Management Enabled

3. Products associated with 3D Models in the .glb format

    > [!IMPORTANT]
    > Server-Based SharePoint Integration is the prefered method for integrating Dynamics with SharePoint. SharePoint Online has removed code-based sandbox solution and the SharePoint List Component can no longer be installed. Product Visualize does not offer support for existinginstances using the List Component.

### Verifying Your Version Number
1. In a browser window navigate to your organization's Sales or Sales Hub instance [https://\<org name>.crm.dynamics.com]().

2. In the upper-right corner of the screen click the Gear Icon and select **About**.

3. The **Server Version** listed must be greater than **9.0** in order to work with Product Visualize.

   ![About](media/about.png "About")

## Set Up SharePoint Document Management
   > [!NOTE] 
   > If you already have Server-Based SharePoint Integration enabled in your instance, you can skip this step.

### Enable SharePoint Integration
1. In a browser window navigate to your organization's Sales or Sales Hub instance [https://\<org name>.crm.dynamics.com]()

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
### Enable SharePoint Document Management
1. In a browser window navigate to your organization's Sales or Sales Hub instance [https://\<org name>.crm.dynamics.com]()
2. In the upper-right corner of the screen find the Gear Icon and click **Advanced Settings**.
3. From the **Document Management** settings page, click **Document Management Settings**
4. Enter the URL of your SharePoint site, if it isn't filled in by default. Then, click __Next__.
5. Continue through the setup leaving the remaining options at the default values.
6. Dynamics will automatically create SharePoint folders for the Dynamics Entities. Close the window when complete.

### Granting SharePoint Permission
1. Visit the SharePoint site you just associated with your Dynamics Instance
2. Toward the upper-right corner of the SharePoint site's homepage click **Share Site**
3. Add Users or Groups from the Search bar
4. Click **Share**

## Add Models to Your Products
1. In a browser window navigate to the Product List in the Sales or Sales Hub applications
2. Open a Product by clicking on its name
3. From the __Related__ tab select __Documents__, which takes you to a view of the SharePoint Document location for that Product
4. From the __Open Location__ dropdown select __Documents on Default Site 1__ to open the SharePoint location outside of Dynamics
5. Drag and drop your Model folder into this location and they will automatically show up in Product Visualize. Models should be added with the following folder structure:
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
> SharePoint folders are only created when you first visit a Product's documents through the Dynamics for Sales interface. Once the folder has been created, you can access the folder straight through the SharePoint website.

## Accept App Permissions
The Product Visualize mobile app requires permission to access the Dynamics 365 for Sales and SharePoint instances you set up earlier. As a global administrator for the trial tenant you can grant access to the entire organization so that each user doesn't have to do it individually.
1. Download the __Microsoft Dynamics 365 Product Visualize__ app from the iOS App Store
2. Open the app and click __Sign In__ with the trial environment's administrator credentials
3. On the __Permissions Requested__ prompt click __Consent on behalf of your organization__
4. Click __Accept__ to return to the app

## Next Steps
You are now ready to use Microsoft Dynamics 365 Product Visualize with all of your sales Opportunities. The Product Visualize mobile app can be downloaded from the iOS App Store. Users will be able to login with the same AAD credentials they use to connect to Dynamics 365.
  
