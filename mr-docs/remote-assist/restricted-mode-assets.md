
# Restrict the ability to access asset records in Dynamics 365 Remote Assist

If you [have a scenario where you need to protect your company information](restricted-mode-overview.md), you can restrict the ability for Microsoft Dynamics 365 Remote Assist users on HoloLens from [accessing asset records](asset-capture-overview.md). If you don't restrict the ability to access asset records, by default, HoloLens users will be able to access them. 

When you restrict the ability to access asset records this way, if a user selects the **Assets** tab in the Remote Assist model-driven app, they'll see this message: "You do not have permissions to access these records. Contact your Microsoft Dynamics 365 administrator for help."

 ![Screenshot of model-driven app with message that says user doesn't have permissions to access records.](media/restricted-mode-assets-model-driven-app.jpg "Screenshot of model-driven app with message that says user doesn't have permissions to access records")

On HoloLens, users will see a message that lets them know they don't have the appropriate permissions. 

> [!NOTE]
> Users on the Dynamics 365 Remote Assist mobile app will not be able to access asset records if you restrict the ability to access asset records as described in this article. 

## Restrict the ability to access asset records

To restrict the ability to access asset records, first make a copy of the default role, and then remove the ability to access assets from the default role. The copied role retains the permissions for accessing asset records. You can assign this copied role to users that **DO** need to be able to access asset records. You'll need to do this for each each environment that the user has access to. 

### Make a copy of the default role

1. Sign into the environment that has the asset records that you want to protect, select the **Settings** button, and then select **Advanced Settings**.

    ![Screenshot with Advanced Settings command highlighted.](media/restricted-mode-assets-advanced-settings.jpg "Screenshot with Advanced Settings command highlighted")

2. In the Dynamics 365 window, select the down arrow next to **Settings**, and then select **Security**.

     ![Screenshot with Settings button and Security entry highlighted.](media/restricted-mode-assets-security.jpg "Screenshot with Settings button and Security entry highlighted")

3. Select **Security Roles**.

     ![Screenshot showing Security Roles command highlighted.](media/restricted-mode-assets-security-roles.jpg "Screenshot showing Security Roles command highlighted")

4. Find and select the **Remote Assist - App User** role (the default role), select the down arrow next to **More Actions**, and then select **Copy Role**.

     ![Screenshot of Remote Assist - App User role and Copy Role command highlighted.](media/restricted-mode-assets-copy-role.jpg "Screenshot of Remote Assist - App User role and Copy Role command highlighted")
    
5. Add a descriptive name for the new role (for example, **Remote Assist - App User (with Assets)**), and then select **OK**.

     ![Screenshot showing a descriptive name for the role.](media/restricted-mode-assets-describe-new-role.jpg "Screenshot showing a descriptive name for the role")
     
### Edit the default role and assign it

Next, you'll remove permissions to access asset records from the default role, and then assign it to the appropriate users.  

1. Select the **Remote Assist - App User** default role. 

     ![Screenshot showing Remote Assist - App User default role highlighted.](media/restricted-mode-assets-select-default-role.jpg "Screenshot showing Remote Assist - App User default role highlighted")

2. Select the **Custom Entities** tab, and then disable access for all scopes (Read, Write, and so on) for the following entities:

    - Customer Asset
    - Customer Asset Attachment
    - Customer Asset Category

     ![Screenshot showing Custom Entities tab and three Asset entities highlighted.](media/restricted-mode-assets-custom-entities.jpg "Screenshot showing Custom Entities tab and three Asset entities highlighted")

3. Go back to **Settings > Security**, and then select **Users**.

     ![Screenshot of Users command highlighted.](media/restricted-mode-assets-users.jpg "Screenshot of Users command highlighted")

4. Find and select the desired user, and then select **Manage Roles**.

     ![Screenshot of selected user role and Manage Roles command highlighted.](media/restricted-mode-assets-manage-roles.jpg "Screenshot of selected user role and Manage Roles command highlighted")

5. In the **Manage User Roles** dialog box, make sure that the **Remote Assist - App User** role is selected.

     ![Screenshot of Manage User Roles dialog box with Remote Assist - App User role highlighted.](media/restricted-mode-assets-selected-role.jpg "Screenshot of Manage User Roles dialog box with Remote Assist - App User role highlighted")

6. In the **Manage User Roles** dialog box, make sure that the following roles are not selected:

    - Remote Assist - App User (with Assets)
    - Remote Assist - Administrator
    - Field Service - Administrator
    - Field Service - Dispatcher
    - Field Service - Resource

     ![Screenshot of Manage User Roles dialog box with roles cleared.](media/restricted-mode-assets-cleared-roles.jpg "Screenshot of Manage User Roles dialog box with roles cleared")

7. Verify that the user can access the desired resources and can’t access assets before handing the account to the end user.

## See also

- [Overview of restricting capabilities in Dynamics 365 Remote Assist](restricted-mode-overview.md)
- [Restrict calling and the ability to access contacts](restricted-mode-calling.md)
- [Restrict the ability to access OneDrive files](restricted-mode-files.md)
- [Restrict the ability to change user accounts](restricted-mode-signout.md)
