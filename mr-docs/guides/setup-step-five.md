
# Setup Step 5: Add additional user accounts to Dynamics 365 Guides (optional)

>[!NOTE]
>Before completing the procedure in this step, make sure to see [Step 4: Set up Guides Analytics reports](setup-step-four.md)

If you want to add additional users to [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)], you need to assign the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] license to them and configure the roles they will have access to in the Dynamics 365 admin center.

## Add a user account

1. Go to the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home).

2. In the left pane, select **Users**, and then select **Active users**. 

3. On the **Active users** page, select **Add a user**.

   ![Add a user command](media/add-additional-user.png "Add a user command") 

4. On the **Set up the basics** page, fill in the information for the new user. Select **Next** when you're done.

   ![Set up the basics page](media/setup-basics.png "Set up the basics page")

   > [!NOTE]
   > By default, an auto-generated password will be generated for the user. The user is required to change the password the first time they sign in with this account. If you want to change the password to a permanent password instead of using the auto-generated password, select the **Let me create the password** option, and then clear the **Require this user to change their password when they first sign in** check box. 
 
5. Select the location for this user, and then under **Licenses**, select the **Dynamics 365 Guides** check box. 

    ![Dynamics 365 Guides check box](media/assign-license-user.png "Dynamics 365 Guides check box") 

     Select **Next** when you're done.
   
6. On the **Optional settings** page, leave the **User (no administrator access)** box selected unless this new user will be an administrator. In that case, select the **Global administrator** check box. 

   ![Optional settings page](media/user-optional-settings.png "Optional settings page") 
   
7. To fill out the new user's profile info, scroll down, and then expand **Profile info**. Select **Next** when you're done.
   
   ![Expanded Profile info](media/expanded-profile-info.png "Expanded Profile info")
   
8. Review the information on the last page. To make changes, select the **Edit** button below each section. Select **Finish Adding** when you're done.

   ![Review page with Edit buttons](media/review-page.png "Review page with Edit buttons")

8. If you selected **Auto-generate password** in step 4, make note of the password. The user will need this password to sign in.

   ![Auto-generated password](media/review-user-settings.png "Auto-generated password") 
   
9. Select **Close**.

10. Set up user roles for the solution as described in [Step 2: Create a Common Database environment and install the solution](setup-step-two.md).

## What's next?

If you have trouble with any of the procedures in this step, please:

- Ask on our community site at https://community.dynamics.com/365/guides.

- Contact customer service at https://dynamics.microsoft.com/support/.

### Other useful links

[Learn about resources you can use to get started with Dynamics 365 Guides](get-started.md)<br>
[Author a guide](authoring-overview.md)<br>
[Overview of operating a guide](operator-overview.md)<br>
[Analyze your guides to improve process efficiencies](analytics-guide.md)<br>
[FAQ](faq.md)
