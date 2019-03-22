
# Set up Dynamics 365 Product Visualize (in preview)
Microsoft Dynamics 365 Product Visualize requires an active Dynamics 365 for Sales instance that's backed by a SharePoint site. This document provides step-by-step procedures for setting up a new trial instance of Dynamics 365 for Sales. 

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

After creating the Active Directory tenant, the next step is to add an admin user to the tenant. The admin user will be responsible for creating additional users, assigning licenses, and initializing Dynamics 365. 

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

# Add a Dynamics 365 Customer Engagement Trial
Product Visualize integrates directly into Dynamics 365 for Sales, allowing your salespeople to seamlessly transition from the vital customer data into an engaging sales experience that will change the way customers think about your products.
1. In a private browser window, return to [https://admin.microsoft.com](https://admin.microsoft.com)
2. Click __Billing > Subscriptions__ and click __Add Subscription__
3. Find __Dynamics 365 Customer Engagement__ and select __Start Free Trial__
4. At the summary page double-check  that you are signing-up for a __Dynamics 365 Customer Engagement__ trial and click __Try Now__. Then click __Continue__ from the confirmation page.

## Assign licenses
Now that you have license to Dynamics 365 Customer Engagement you have to assign that licenses to your admin user. 
1. In a private browser window, return to [https://admin.microsoft.com](https://admin.microsoft.com)
2. From the navigation menu on the left select __Users > Active Users__
3. Edit the properties for your admin user created earlier by double clicking the name 
4. On the __Product Licenses__ line click __Edit__
5. __Enable__ the Licenses for __Dynamics 365 Customer Engagement__ and __Office 365 Enterprise E3__
6. Save the changes and close the user dialog

## Set up the Dynamics 365 for Sales trial
It is time to finally set up your instance of Dynamics 365 Customer Engagement. This guide walks you through the manual installation of the Dynamics for Sales app, which generates a completely empty instance of the Dynamics CDS. If you would prefer for a simpler set up procedure, refer to the note below.
1. Return to  Return to [https://admin.microsoft.com](https://admin.microsoft.com) and select __Dynamics 365__ from the _Admin Centers__ dropdown on the Microsoft Admin Portal
2. A new page is brought up that asks you to set up your Dynamics 365 instance.
    * Set the language to your preferred language
    * Under __Select which scenario fits you best__ check __None of these__ (See note below)
    * Set the currency to your preferred currency
3. Click __Complete Setup__ which will likely take a few minutes to complete.
4. Return to the Dynamics 365 Admin Portal
5. From the __Instances__ page, ensure your newly created instance is selected and click the __Edit__ button next to the word __Solutions__ in the gray box on the right
6. From the list of available solutions find __Dynamics 365 Sales Application__ and click __Install__
7. This process may take a while to complete. You can refresh the page to view the current status of your installation.

**NOTE:** In step 2 you could optionally select __Sales__ for your scenario which would allow you to skip step 4 - 7. However, this will install some additional sample data that may not be relevant to your organization. 

## Set up a SharePoint site
1. Navigate to the Sales Hub of your newly created Dynamics 365 instance 
    * Visit [https://\<org>.crm.dynamics.com]()
    * Find __Sales Hub__ from the list of available applications
2. Click the __Gear__ icon in the upper-right corner of the page and select __Advanced Settings__
3. At the top of the page click the down arrow next to __Settings__ and click __Document Management__
4. Click the button for __Enable Server-Based SharePoint Integration__
5. Continue through  the setup and, when prompted, enter the URL for your SharePoint ([https://\<org name>.sharepoint.com]())
6. When complete, return to the __Document Management__ settings page and click __Document Management Settings__
7. Enter the URL of your SharePoint site, if it isn't filled in by default. Then, click __Next__.
8. Continue through the setup leaving the remaining options at the default values.
9. Dynamics will now take a minute to set up the SharePoint connection.

**Note:** If you opted to use the automated __Sales__ setup earlier you can skip the steps of Enabling Server-Based SharePoint Integration.

# Conclusion
Once the setup process has finished you will have an Azure Active Directory Tenant complete with Microsoft Office 365 and Microsoft Dynamics 365 Customer Engagement. At this point you can start adding Opportunities, Products, and Models to Dynamics. This is covered in the __Product Visualize Administrator's Guide__

