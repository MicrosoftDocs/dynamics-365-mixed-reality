
# Restrict the ability to access asset records in Dynamics 365 Remote Assist

If you [have a scenario where you need to protect your company information](restricted-mode-overview.md), you can restrict the ability for Dynamics 365 Remote Assist users on HoloLens from [accessing asset records](asset-capture-overview.md). If you don't restrict the ability to access asset records, by default, HoloLens users will be able to access them. 

When you restrict the ability to access asset records this way, if a user selects the **Assets** tab in the Remote Assit model-driven app, they'll see the following message.

SCREEN SHOT GOES HERE.

On HoloLens, users will see a message that lets them know they don't have the appropriate permissions. 

## Restrict the ability to access asset records

To restrict the ability to access asset records, you'll make a copy of the default role, and then remove the ability to access assets from the default role. You can use the copy of the original default role as a backup. 

> [!NOTE]
> If there are users that **DO** need access to asset records, you'lll need to create a new role with access to asset records. You'll need to do this for each user across each environment that they have access to.  

1. Sign into the environment that has the asset records you want to protect, select the **Settings** button, and then select **Advanced Settings**.

    SCREEN SHOT GOES HERE

2. In the Dynamics 365 window, select the down arrow next to **Settings**, and then select **Security**.

    SCREEN SHOT GOES HERE

3. Select **Security Roles**.

    SCREEN SHOT GOES HERE

4. Find and select the **Remote Assist - App User** role, select the down arrow next to **More Actions**, and then select **Copy Role**.

    SCREEN SHOT GOES HERE

5. Add a descriptive name for the new role (for example "Remote Assist - Ap User (with Assets)", and then select **OK**.

    SCREEN SHOT GOES HERE

6. Select the **Remote Assist - App User** role so you can edit it. 

    SCREEN SHOT GOES HERE

7. On the right side of the screen, select **Custom Entities**, and then disable access for all scopes (Read, Write, and so on) for all of the following entities:

    - Customer Asset
    - Customer Asset Attachment
    - Customer Asset Category

    SCREEN SHOT GOES HERE

8. Go back to **Security > Settings**, and then select **Users**.

    SCREEN SHOT GOES HERE

9. Find and select the desired user, and then select **Manage Roles**.

    SCREEN SHOT GOES HERE

10. Make sure the **Remote Assist - App User** role is selected.

    SCREEN SHOT GOES HERE

11. Make sure the following roles are not selected:
    - Remote Assist - App User (with Assets)
    - Remote Assist - Administrator
    - Field Service - Administrator
    - Field Service - Dispatcher
    - Field Service - Resource

    > [!NOTE]
    > Because the default role does not have access to assets, if there are any users that you DO want to have access to assets, you must assign them the **Remote Assist – App User (with Assets)** role. You must do this for each user across each environment.

    SCREEN SHOT GOES HERE

NOTE- Verify that the user can access the desired resources and can’t access assets before handing the account to the end user.
