
# Restrict the ability to access OneDrive files in Dynamics 365 Remote Assist

If you [have a scenario where you need to protect your company information](restricted-mode-overview.md), you can restrict the ability for Dynamics 365 Remote Assist users on HoloLens from accessing OneDrive files. 

When you restrict the ability to access OneDrive files, users will see the **Files** tab, but no files will be visible. 

> [!NOTE]
> When you restrict access to files described in this article, Dynamics 365 Remote Assist mobile app users will not be able to access OneDrive files in the mobile app. 

## Restrict access to OneDrive files

1. Sign in to the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?#/users) as an admin. 
2. In the left pane, select **Users** > **Active users**, and then select **Add a user**.
3. Fill out the user information, and then select **Next**.
4. Select the **Dynamics 365 Remote Assist** and **Microsoft Teams** license check boxes.
5. Clear the **SharePoint** and **Office for the Web** license check boxes, and then select **Next**.
6. In the **Optional settings** section, leave the default value (no administration access), and then select **Next**.
7. In the **Review and finish** section, make sure the information is correct, and then select **Finish adding** when you're ready.
    You'll see the following confirmation screen. 
