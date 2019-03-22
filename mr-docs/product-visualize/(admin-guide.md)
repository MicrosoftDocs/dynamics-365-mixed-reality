

# Administrator's Guide

After you've completed the [setup process](setup.md) for Microsoft Dynamics 365 Product Visualize, you'll need to:

- Create an Office 365 user group and share your SharePoint site with the group

- Add users and assign security roles

- Add products

- Add opportunities

- Install the Product Visualize control if you want sales people to be able to open Product Visualize directly from Dynamics 365 for Sales

- Adjust permissions

This topic provides step-by-step procedures for all of the above.

# Set up a User Group
Groups in Office 365 let you choose a set of people that you wish to collaborate with and easily set up a collection of shared resources. For Product Visualize, this means you can give the group access to SharePoint which saves you the trouble of having to give every individual permission. This is a one-time step that will save you time later on. The User Group should have Read/Write permissions on the SharePoint site in order to make full use of our app.

## Create a User Group
1. Open a new private browser window
2. Visit [https://admin.microsoft.com](https://admin.microsoft.com) and login with the administrator credentials
3. From the navigation menu on the left, drop down the __Groups__ section and select __Groups__
4. Near the top of the page click the __Add a Group__ button
5. Give the group a __Name__ and set the __Group Type__ should be set to __Office 365__
6. Add the admin user as the owner of the group by clicking the __Select Owner__ button
7. Click __Add__ to finish adding the group

## Share the SharePoint site with the Group
1. Navigate to your trail's SharePoint site [https://\<org\>.sharepoint.com]()
2. In the upper right corner of the page click __Share Site__
3. From the __Share__ window search for the group you made earlier and click the group name to add it to the site
4. Grant the group __Edit__ permission by clicking the small arrow under the group name
5. Click __Share__ to finish granting the group access to SharePoint

# Adding Users
The administrative user created during the setup of your instance has full control of all aspects of your test environment. This user can administer your team's licenses, edit settings in Dynamics, and manage who has access to your services. Additional users can easily be added with more restrictive permissions so each salesperson can work with their own account.

New users must first be added in the Azure Active Directory, which assigns them a username and password. Then, the user must be assigned a security role in Dynamics 365 in order to access the Dynamics applications.

## Add a user to your Organization
1. Visit [https://admin.microsoft.com](https://admin.microsoft.com) and login with the administrator credentials
2. From the navigation menu on the left, drop down the __Users__ section and select __Active Users__
3. Near the top of the page find the __Add a User__ button and click it to open the New User dialog
4. In the New User dialog, fill in the following fields for the User:
    * First Name
    * Last Name
    * Display Name
    * Username
    * Location
5. Assign the user a role based on what resources they should be accessing:
    * **User** - This user won't have permissions to the Office 365 admin center or any admin tasks
    * **Global Administrator** - This user will have access to all features in the admin center and can perform all tasks in the Office 365 admin center
    * **Custom Administrator** - You can assign this user one or many roles so they can manage specific areas of Office 365
6. Enable the Licenses for __Dynamics 365 for Sales__ and __Office 365 Enterprise__
7. Click __Add__ to submit the changes
8. On the confirmation page, make note of the __Username__ and __Password__ before clicking __Close__
9. Select the user you just created and on the __Group Memberships__ line click __Edit__
10. Search for the user group you created earlier and click the group name to add the user to the group
11. Click __Close__ to finish adding the user

**Note:** It may take some time for users added to your organization to show up in Dynamics, so we suggest adding all the users to your Organization before continuing

## Assign a security Role to the User

1. In your private browser window navigate to your Dynamics 365 URL [https://\<org\>.crm.dynamics.com]()
2. Open the Sales Hub application from the list
3. Navigate to the Settings Menu by clicking the __Gear Icon__ in the upper-right corner of the page and select __Advanced Settings__
4. From the __Settings__ dropdown at the top of the page select __Security__.
5. On the __Security Page__ click on __Users__
6. Click on the name of the user you created to open the User page
7. From the menu bar near the top of the page click __Approve Email__ to allow the user to be synced by the server
8. Nearby on the menu bar click __Manage Roles__
9. Select the __Salesperson__ and __Sales, Enterprise app access__ options from the list and click __OK__

# Adding Products
Products represent the things you sell to customer, whether they be physical goods or services. Products that a customer may be interested in purchasing will be added to a sales Opportunity. This allows salespeople to exactly track a customers needs the potential revenue a sale might bring in.

__Products__ are sold in __Units__, which represent the possible quantities that are sold together. _Hours_, _Cases_, and _Pallets_ are good examples of Units. Units are grouped into __Unit Groups__ which keep Units with a similar purpose together. If you sell services, 'Time' might be a Unit Group containing _Days_, _Hours_, and _Minutes_. 

Products may be priced differently depending on who you are selling to, when the sale is happening, and where the customer works. Prices with a similar purpose are grouped together into __Price Lists__. For example, you may have one price list for customers in Canada and another for customers in the U.S.

Individual Products can be arranged into a hierarchy, as well. __Product Families__ allow you to categorize similar Products based on your organization's needs.

This section will walk you through creating a new Price List, Product Family, and Product. Dynamics 365 provides default values for Units and Unit Groups.

## Create a Price List
1. Return to the Sales Hub application for your Dynamics 365 instance
2. Navigate to the Settings Menu by clicking the __Gear Icon__ in the upper-right corner of the page and select __Advanced Settings__.
3. From the __Settings__ dropdown at the top of the page select __Product Catalog__
4. Click __Price Lists__
5. Create a new price list by pressing __New__ near the top-left of the page
6. Give the price list a name (Default Price List, for example) and click __Save and Close__

## Create a Product Family (Optional)
1. Return to your Dynamics 365 Sales Hub [https://\<org\>.crm.dynamics.com](https://\<org\>.crm.dynamics.com)
2. Open the Navigation menu on the left and click __Products__
3. Create a new Product Family by clicking __Add Family__
4. Give the family a __Name__ (Product Samples) and __Product ID__ (PS-1) before clicking __Save__
5. Now click __Publish__ to finish creating the Product Family
6. 
## Create a Product
1. Return to the Product list page by click __Products__ in the Navigation bar on the left
2. Create a new Product by clicking __Add Product__
3. Fill in the __Name__ and __Product ID__ with any values you want
4. Set the __Parent__ value to the __Product Samples__ family created earlier. 
5. Set the __Unit Group__ field to __Default Unit__, set the __Default Unit__ field to __Primary Unit__
6. Set the __Supported Decimals__ to 2
7. __Save__ (but don't close) the Product
8. Set the __Default Price List__ to the one created earlier
9. Click the __Additional Details__ tab, directly above the __Name__ field
10. In the __Price List Items__ section click __Add New Price List Item__
11. Assign the Price List created earlier in the __Price List__ Field
12. Switch to the __Pricing Information__ tab and fill in the __Amount__ field with the price for your Product
13. __Save__ the Product again
14. Click __Publish__ to finish creating the Product

# Adding Models
Presenting complicated Products to a customer with traditional 2D materials always left something to be desired and creating physical 3D models was time-consuming and costly. Product Visualize simplifies the entire process by bringing 3D digital Models into the real-world. 

Product Visualize makes use of the widely available GL Transmission Format (glTF) to store Model data. Many of the most popular 3D Modeling Products used by Engineering and Marketing teams already supports this format and exporters exist to convert many other formats to glTF. This section will guide you through adding a Model and thumbnail image to Product Visualize.

1. Return to the Product list page by click __Products__ in the Navigation bar on the left
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

# Adding Opportunities
Opportunities represent a chance to sell your Products to a customer. They capture a customer's needs, budget, and timeline, in addition to the list of Products the customer is interested in buying. Salespeople can view their open Opportunities directly from the Product Visualize app, but they must be added through the Sales Hub interface
1. Return to your Dynamics 365 Sales Hub
2. Open the Navigation menu on the left and click __Opportunities__
3. Create a new Opportunity by clicking the __New__ button at the top of the page
4. Give the Opportunity a name by filling in the __Topic__ field
5. (Optional) Assign the __Owner__ field to any user you have already added
6. __Save__ (but do not close) the Opportunity
7. Open the __Product Line Items__ tab 
8. Set the __Price List__ to the one we created earlier
9. Click the __Add New Opportunity Product__ button 
10. In the __Existing Product__ field select one of the Products you created
11. Enter a __Quantity__
12. __Save and Close__

# Install the Product Visualize Control
The Product Visualize Control is an optional enhancement that allows salespeople to launch the Product Visualize app directly from Dynamics 365 on their mobile devices. The Control is lightweight and can easily be updated and removed.

## Import the Product Visualize Solution
1. Return to your Dynamics 365 Sales Hub
2. Navigate to the Settings Menu by clicking the __Gear Icon__ in the upper-right corner of the page and select __Advanced Settings__. 
3. From the __Settings__ dropdown at the top of the page select __Solutions__
4. Download the __Product Visualize__ solution to your PC.
5. Import the solution by clicking the __Import__ button and selecting the solution zip file you downloaded

## Customize the Opportunity Page
There are numerous ways you can customize your Opportunity pages in Dynamics 365 for Sales. This section guides you through our suggested customizations, but feel free to adapt this to your exact needs.
1. From the __Settings__ dropdown at the top of the page select __Customizations__ and then __Customize the System__
2. In the panel on the left find __Entities > Opportunity > Forms__
3. Click the __Opportunity__ form where the __Form Type__ is set to __Main__ (not the one marked __Quick Create__)
4. With the __Summary__ section insert a __One Column Tab__ from the __Insert__ menu at the top of the page
5. Double click on the newly created tab, set the __Name__ and __Label__ fields to __Product Visualize__, and click __OK__
6. Drag a the __Description__ field into the newly created tab from the menu on the right. You may have to uncheck the __Only Show Unused Fields__ options in order to see the __Description__ field
7. Double click on the __Description__ field you just placed to open the __Field Properties__ dialog
8. On the __Display__ tab uncheck __Display Label on the Form__
9. On the __Controls Page__ add the __Product Visualize__ control from the list and check the __Web__, __Phone__, and __Tablet__ options
10. Click __OK__ to finish adding the control
11. __Save__ your changes from the Menu bar
12. __Publish__ your changes and they will be immediately visible on any Opportunity page

# Accept App Permissions
The Product Visualize mobile app requires permission to access the Dynamics 365 for Sales and SharePoint instances you set up earlier. As a global administrator for the trial tenant you can grant access to the entire organization so that each user doesn't have to do it individually.
1. Download the __Microsoft Dynamics 365 Product Visualize__ app from the Apple App Store
2. Open the app and click __Sign In__ with the trial environment's administrator credentials
3. On the __Permissions Requested__ prompt click __Consent on behalf of your organization__
4. Click __Accept__ to return to the app

# Conclusion
You now have everything you need to start using Microsoft Dynamics 365 Product Visualize! New Opportunities, Products, and Models will show up automatically in the application after they have been added to Dynamics. For any help or feedback use the __Feedback__ button in the Product Visualize app.
