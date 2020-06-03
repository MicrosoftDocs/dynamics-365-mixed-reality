---
title: Add users to the Asset Capture preview
author: bencorn
description: Learn how to add users to the preview of asset capture.
ms.author: becorn
ms.date: 5/30/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Add users to the Asset Capture preview

Learn how to add users to the Asset Capture public preview so they can access the app and use the HoloLens 2 to capture asset data.

In this tutorial, you assign users a Remote Assist license and security roles.

## Prerequisites

To complete this article, you need:

- **A Dynamics 365 Remote Assist subscription**, this enables you to assign licenses to the intended set of Remote Assist users.
- **Ability to manage user licenses in Microsoft Admin Center**. To manage user licenses, you need to have an admin role for the Microsoft Admin Center.
- **Admin access to the environment Remote Assist is installed in**. You will be managing security roles for users in the environment. A system administrator role is required in the environment you are managing.

## Assign Remote Assist licenses

Anyone who will be using Remote Assist on HoloLens 2 or accessing the Dynamics 365 Remote Assist UCI app to review captured data will need a Dynamics 365 Remote Assist license. If these users already have a Remote Assist license, you can skip this step.

1. Sign in to the [Microsoft Admin Center](https://admin.microsoft.com) as an admin (User admin or Global admin).
2. Go to the **Billing** > **Licenses** page.
3. Select Dynamics 365 Remote Assist.
4. Select **Assign licenses**.
5. In the Assign licenses to users pane, begin typing a name, and then choose it from the results to add it to the list. You can add up to 20 users at a time.
6. When you're finished, select **Assign**, then select **Close**.

For more detailed documentation on managing user licenses, refer to the docs here: [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide)

## Assign Dynamics 365 security roles

Security roles define how different users, such as service technicians, access different types of records. To enable Asset Capture, security roles must be assigned to each user.

1. Sign in to the [Power Platform Admin Center](https://admin.powerplatform.com) as an admin (Dynamics 365 service admin, Global admin, or Power Platform service admin).
2. Select **Environments**, find the environment Remote Assist is installed in, and select the dots for **More environment actions**.
3. Select **Settings**, then select **Users + permissions** > **Users**.
4. From the top toolbar, select **Manage users in Dynamics 365**.
5. Using the checkboxes on the left, select all the users who will be using Remote Assist. Then select **Manage Roles** from the top toolbar.
6. Select the **Common Data Service User** and **Remote Assist - App User** roles. When you're finished, select **OK** .

## Manage app roles

Security roles must be assigned to apps to ensure users with those roles can access the app. The Remote Assist - App User role must be enabled for the Dynamics 365 Remote Assist app.

1. Sign in to the [Power Platform Admin Center](https://admin.powerplatform.com) as an admin (Dynamics 365 service admin, Global admin, or Power Platform service admin).
2. Select **Environments**, find the environment Remote Assist is installed in, and select the dots for **More environment actions**.
3. Select **Open environment**.
4. If you see a list of **Published Apps**, proceed to step 5. Select **Settings** from the top right toolbar > **Advanced Settings** > select the dropdown next to **Settings** > **My Apps**.
![Screenshot of Dynamics 365 environment.](./media/06.24-d365-settings-my-apps.png "Dynamics 365")
5. Select the **More options** menu on the Remote Assist app tile and then select **Manage Roles**.
![Screenshot of Dynamics 365 manage roles for app menu.](./media/06.25-d365-settings-manage-roles.png "Dynamics 365")
6. From the right side panel, select the **Remote Assist - App User** role from the list and then select **Save**.
![Screenshot of Dynamics 365 assigning app role.](./media/06.26-d365-settings-manage-roles-set.png "Dynamics 365")

## Next steps

In this tutorial, you learned how to assign security roles and enable the app for Remote Assist users. To learn how to create asset records and import your existing asset catalog, see:

> [!div class="nextstepaction"]
> [Create assets](./asset-capture-create-asset.md)