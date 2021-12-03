
# Restrict the ability to access OneDrive files in Dynamics 365 Remote Assist

If you [have a scenario where you need to protect your company information](restricted-mode-overview.md), you can restrict the ability for Dynamics 365 Remote Assist users on HoloLens from accessing OneDrive files. 

When you restrict the ability to access OneDrive files, users will see the **Files** tab, but no files will be visible. 

[HoloLens screenshot showing Files tab highlighted, no files showing, and messsage: "We can't connect to OneDrive".](media/restricted-mode-files-hololens.jpg "HoloLens screenshot showing Files tab highlighted, no files showing, and messsage: "We can't connect to OneDrive"")

> [!NOTE]
> When you restrict access to files described in this article, Dynamics 365 Remote Assist mobile app users will not be able to access OneDrive files in the mobile app. 

## Restrict access to OneDrive files

1. Sign in to the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?#/users) as an admin. 

2. In the left pane, select **Users** > **Active users**, and then select **Add a user**.

    ![Screenshot showing Active users and Add a user highlighted.](media/restricted-mode-files-add-user.jpg "Screenshot showing Active users and Add a user highlighted")

3. Fill out the user information, and then select **Next**.

    ![Screenshot of Set up the basics section.](media/restricted-mode-files-user-info.jpg "Screenshot of Set up the basics section")

4. Select the **Dynamics 365 Remote Assist** and **Microsoft Teams** license check boxes.

    ![Screenshot showing Dynamics 365 Remote Assist and Microsoft Teams check boxes selected.](media/restricted-mode-files-select-licenses.jpg "Screenshot showing Dynamics 365 Remote Assist and Microsoft Teams check boxes selected")

5. Clear the **SharePoint** and **Office for the Web** license check boxes, and then select **Next**.

    ![Screenshot showing SharePoint and Office for the Web check boxes cleared.](media/restricted-mode-files-clear-licenses.jpg "Screenshot showing SharePoint and Office for the Web check boxes cleared")

6. In the **Optional settings** section, leave the default value (no administration access), and then select **Next**.

    ![Screenshot of Optional settings section.](media/restricted-mode-files-optional-settings.jpg "Screenshot of Optional settings section")

7. In the **Review and finish** section, make sure the information is correct, and then select **Finish adding** when you're ready.
    
    ![Screenshot of Review and finish section filled out.](media/restricted-mode-files-review.jpg "Screenshot of Review and finish section filled out")

8. If you see the following confirmation screen, you'll know the user was added correctly. Select **Close**.

    ![Screenshot with user added highlighted.](media/restricted-mode-files-confirmation.jpg "Screenshot with user added highlighted")
