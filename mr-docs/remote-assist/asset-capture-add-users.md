---
title: Add users to the Dynamics 365 Remote Assist model-driven app
author: dhgoelmsft
description: Learn how to add users to the model-driven Dynamics 365 Remote Assist app.
ms.author: dhgoel
ms.date: 04/28/2021
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Add users to the Dynamics 365 Remote Assist model-driven app

After you [install the Microsoft Dynamics 365 Remote Assist model-driven app](ra-webapp-install.md), you'll need to add users so they can use the Dynamics 365 Remote Assist client app on HoloLens or mobile to:

- [Capture and view asset data](./asset-capture-overview.md).

- Create and share [one-time call links](./one-time-call.md).

- Record call metrics for the [Calls dashboard](./calls-dashboard.md).

This article shows you how to assign a Dynamics 365 Remote Assist license to users and set up security roles.

## Prerequisites

To complete the steps in this article, you need:

* **A Dynamics 365 Remote Assist subscription**. The subscription enables you to assign licenses to users you want to give access to Dynamics 365 Remote Assist.
* **The ability to manage user licenses in the Microsoft 365 admin center**. To manage user licenses, you need to have an admin role for the Microsoft 365 admin center.
* **Admin access to the environment Dynamics 365 Remote Assist is installed in**. You'll be managing security roles for users in the environment. A system administrator role (typically a Power Apps admin, Global admin, or Dynamics 365 admin) is required in the environment you're managing.

## Assign Dynamics 365 Remote Assist licenses

Anyone who will be using Dynamics 365 Remote Assist client app on HoloLens or Mobile or accessing the Dynamics 365 Remote Assist model-driven app will need a Dynamics 365 Remote Assist license. If these users already have a Dynamics 365 Remote Assist license, you can skip this step.

1. Sign in to the [Microsoft 365 admin center](https://admin.microsoft.com) as an admin (User admin or Global admin).
2. Go to **Billing** > **Licenses**.
3. Select **Dynamics 365 Remote Assist**.
4. Select **Assign licenses**.
5. In the **Assign licenses to users** pane, begin typing a name, and then choose it from the results to add it to the list. You can add up to 20 users at a time.
6. When you're finished, select **Assign**, and then select **Close**.

More information: [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)

## Assign Dynamics 365 security roles

> [!NOTE]
> Users can take up to one hour to appear in the Dynamics 365 admin center after the licenses are added in the Microsoft 365 admin center.

1. Open the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), and sign in using your admin credentials.

2. If the **Environments** page doesn't appear, select **Environments** in the left pane to open it.

3. Select the environment that you want to work with, select the **More environment actions** (**...**) button, and then select **Settings**.

    ![Settings command](media/power-platform-environment-settings.PNG "Settings command")

4. Select **Users + permissions** to expand the list of options, and then select **Users**. If you're prompted to sign in to Dynamics 365, be sure to use your admin credentials.

    ![Users command selected](media/user-permissions-users.PNG "Users command selected")
    
5. Follow one of these steps:

    - If the users are already in the list, skip ahead to step 6 to assign user roles.
    
    - If you need to add one or more users, select **Add user** at the top of the page, enter the account details in the **Add user** dialog box, and then select **Add**. For more information, see the "Troubleshooting" section later in this topic.

        > [!NOTE]
        > When you add a user in this way, you trigger synchronization. The user is added to the instance within a few minutes.  
    
6. Select **Manage users in Dynamics 365** at the top of the page. 

   ![Manage users in Dynamics 365 command](media/manage-user-roles.PNG "Manage users in Dynamics 365 command")

7. Select one or more users, and then select **Manage Roles** at the top of the page.

    ![Manage Roles button](media/manage-roles.PNG "Manage Roles button")

8. In the **Manage User Roles** dialog box, select the **Basic User** check box.

    ![Basic User check box](media/basic-user.PNG "Basic User check box")
    
    > [!NOTE]
    > You may see a **Common Data Service** check box instead of a **Basic User** check box. If so, select that check box. 

9. Select the check box for **Remote Assist - App User**.
        
10. For supervisors, service managers, and other users who may need access to advanced features, such as the [Calls dashboard](./calls-dashboard.md), select the check box for the **Remote Assist - Administrator** role. When you're finished, select **OK**.
    
### Troubleshooting security roles

If users don't appear on the **Security** page (**Dynamics 365** \> **Settings** \> **Security**), in the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), select **Add user**. In the **Add user** dialog box, enter the account details, and then select **Add**. This operation triggers synchronization, so the user is added to the instance within a few minutes.

![Adding a user in Power Platform admin center](media/add-users-troubleshooting.PNG "Adding a user in Power Platform admin center")

## Manage app roles

> [!Note]
> The necessary security roles are associated with the model-driven app automatically. Depending on your organization's setup, this next section may not be required. If you're running into issues accessing the model-driven app, it is recommended that you complete the setup as described in this section.

Security roles must be assigned to apps to ensure that users who have those roles can access the app. The **Remote Assist - App User** and the **Remote Assist - Administrator** roles must be enabled for the Dynamics 365 Remote Assist app.

1. Sign in to the [Power Platform admin center](https://admin.powerplatform.com) as an admin (Dynamics 365 service admin, Global admin, or Power Platform service admin).
2. Select **Environments**, find the environment that Dynamics 365 Remote Assist is installed in, and then select !["More environment actions"](./media/ellipsis.png "More environment actions").
3. Select **Open environment**.
4. If you see a list of **Published Apps**, proceed to step 5. Otherwise, select **Settings** from the upper-right toolbar, select **Advanced Settings**, and then select the drop-down menu next to **Settings** > **Apps**.
:::image type="content" source="media/06.24-d365-settings-my-apps.png" alt-text="Screenshot of the Dynamics 365 environment.":::
5. On the Dynamics 365 Remote Assist app tile, select **More options**, and then select **Manage Roles**.
:::image type="content" source="media/06.25-d365-settings-manage-roles.png" alt-text="Screenshot of the Dynamics 365 Manage Roles for app menu.":::
6. From the right side panel, select the **Remote Assist - App User** and **Remote Assist - Administrator** roles from the list, and then select **Save**.
:::image type="content" source="media/06.26-d365-settings-manage-roles-set.png" alt-text="Screenshot of Dynamics 365 assigning app role":::

## Selecting the right environment from the client app

After end users have been assigned licenses and security roles, they must also select the correct environment with the Dynamics 365 Remote Assist model-driven app installed to use related features within the HoloLens or Mobile app. This can be done by going into the settings menu of the respective client apps and selecting the environment. By default, there is no environment associated with the client app.

### Selecting the right environment in HoloLens

1. Go to the settings menu and click on the **Dynamics 365 environment** :::image type="content" source="media/HololensSettingsEnvironmentSelection01.png" alt-text="Remote Assist settings in the HoloLens":::

1. You will see a list of environments with either Dynamics 365 Remote Assist or Dynamics 365 Field Service or both installed. To use Dynamics 365 Remote Assist related features, such as [asset capture](./asset-capture-photos.md) and [calls dashboard](./calls-dashboard.md), you will need to select an environment with Dynamics 365 Remote Assist installed. To update [Field Service bookings](./update-field-service-booking-hololens.md), you will need to select an environment with Field Service installed. :::image type="content" source="media/HololensSettingsEnvironmentSelection02.png" alt-text="List of environments in Remote Assist settings menu on the HoloLens":::

### Selecting the right environment on Android or iOS

1. Go to the settings menu and click on the **Dynamics 365 environment**\
:::image type="content" source="mobile-app/media/RAMSettingsEnvironmentSelection01.png" alt-text="Remote Assist settings in the Mobile app":::

1. You will see a list of environments. To use Dynamics 365 Remote Assist related features, such as [asset capture](./asset-capture-photos.md) and [calls dashboard](./calls-dashboard.md), you will need to select an environment with Dynamics 365 Remote Assist installed. Click **Confirm** after selecting the right environment.\
:::image type="content" source="mobile-app/media/RAMSettingsEnvironmentSelection02.png" alt-text="List of environments in Remote Assist settings menu in the Mobile app":::

## Next steps

After assigning security roles, you can check out the following articles to use the model-driven app:

* [Create asset records and import your existing asset catalog](./asset-capture-create-asset.md)
* [Get insights with Calls Dashboard](./calls-dashboard.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
