---
title: Deploy Dynamics 365 Remote Assist
author: xonatia
description: Dynamics 365 Remote Assist users can deploy and set up Dynamics 365 Remote Assist on their devices. 
ms.author: xolee
ms.date: 04/28/2021
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Deploy Dynamics 365 Remote Assist

After you get your [free trial](try-remote-assist.md) or [purchase](buy-remote-assist.md) Dynamics 365 Remote Assist, you can assign licenses to users. Once assigned, users can deploy Dynamics 365 Remote Assist on their individual devices.

> [!Note]
> There are two types of users for Dynamics 365 Remote Assist and Dynamics 365 Remote Assist Attach: remote experts and field service technicians. Field service technicians require a Dynamics 365 Remote Assist license **and** a Microsoft Teams license. When you buy a Dynamics 365 Remote Assist license, a Microsoft Teams license is included. However, remote experts (who aren't in the field) require only a Microsoft Teams license. For more information, see [deploying Microsoft Teams licenses in your organization](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/use-microsoft-teams-with-remote-assist).

In this article, we’ll walk through how to deploy Dynamics 365 Remote Assist or Dynamics 365 Remote Assist Attach (for Field Service customers). This includes:

-	Assigning licenses to users in your organization (for IT Admins)

-	Deploying Dynamics 365 Remote Assist on a device (for individuals in your organization) 

You can also learn how to [deploy to multiple tenants](multi-tenant-deployment.md) or [enable vendors and contractors to use Dynamics 365 Remote Assist](vendor-use-RA.md).

## Add and assign licenses

### Prerequisites

Your organization must have:

- A Microsoft 365 or Microsoft 365 [administrator account](https://www.microsoft.com/microsoft-365/business/office-365-administration). [Learn more about admin permissions](https://docs.microsoft.com/office365/admin/admin-overview/admin-overview?redirectSourcePath=%252farticle%252foffice-365-admin-overview-c7228a3e-061f-4575-b1ef-adf1d1669870&view=o365-worldwide). 

- A [free trial](try-remote-assist.md) of Dynamics 365 Remote Assist, or a [purchased license](buy-remote-assist.md). 

- An Azure Active Directory account for each licensed user. They'll use Azure Active Directory to sign into the app.

Make sure that users in your organization have the required licensing and devices. For more information, see [licensing and product requirements](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/requirements).

### Adding and assigning licenses

Once prerequisites are met, you can now add and assign licenses to *individual users* or a *group of users* in your organization through the Microsoft 365 or Microsoft 365 administrator portal. 

1.	Log into the [Microsoft 365 or Microsoft 365 administrator portal](https://www.microsoft.com/microsoft-365/business/office-365-administration ) using your organization’s admin account.

    ![Screenshot of the admin portal.](./media/buy_1.png "Admin Portal")

2.	Make sure the **Try the new admin center** toggle is turned off.

3.	In the left navigation bar, select **Billing** > **Subscriptions**. 

    ![Screenshot showing billing subscriptions](./media/deploy_3.png "Billing subscriptions")

4.	Select **Assign to users**. 

    ![Screenshot showing assigning users](./media/deploy_4.png "Assign users")

5. Select **Add a user**. For more information, see [Add users and assign licenses at the same time](https://docs.microsoft.com/office365/admin/add-users/add-users?view=o365-worldwide).

6.	Find the users in your organization that you want to add. In the **Product licenses** section, make sure to provide them with Dynamics 365 Remote Assist and Microsoft Teams licenses. 

    ![Screenshot of product licenses](./media/deploy_6.png "Product licenses")

7. To add multiple users, go to **More** > **Import multiple users**. Fill out the CSV file, set user options, and view your results. 

    ![Screenshot of adding multiple users.](./media/deploy_7.png "Add multiple users")

8.	After you have added a user or users, you can assign licenses to them through the Microsoft 365 or Microsoft 365 administrator portal. See [Assing licenses to users](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users?view=o365-worldwide).

At this point, users in your organization can set up Dynamics 365 Remote Assist on their devices, as described below. 


## Download and install the app

After assigning licenses, users can set up and use the app on their HoloLens, HoloLens 2, or mobile devices. 

### Prerequisites

- The organization's IT admin must add the user and assign a Dynamics 365 Remote Assist license **and** Microsoft Teams license in the Microsoft 365 or Microsoft 365 administrator portal, as described above. 

- A [Microsoft Teams account](https://teams.microsoft.com/start). See [Using Teams with Dynamics 365 Remote Assist](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/use-microsoft-teams-with-remote-assist) for more information.

- Azure Active Directory [Premium trial](https://azure.microsoft.com/trial/get-started-active-directory/) (for HoloLens users only).

- A HoloLens, HoloLens 2, or mobile device. See [Licensing and product requirements can be found](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/requirements).

### Steps for HoloLens and HoloLens 2

1.	Go to the **Start** menu, and then select **Microsoft Store**. 

2.	Search for and download **Dynamics 365 Remote Assist** and launch the app.

3.	Sign into Dynamics 365 Remote Assist with your Microsoft Teams account. 

4.	You'll be taken to your **Contacts** page. If you're using a free trial, you'll be prompted to start your **Free Trial of Dynamics 365 Remote Assist**. 

5.	You can now use Dynamics 365 Remote Assist on your HoloLens or HoloLens 2. Next up, [Learn how make calls](making-taking-calls-hololens.md). 

### Steps for mobile devices

1.	Go to the appropriate iOS or Android app store.

2.	Search for and download **Dynamics 365 Remote Assist** and launch the app.

3.	Sign into Dynamics 365 Remote Assist with your Microsoft Teams account. 

4.	You'll be taken to your **Contacts** page. If you're using a free trial, you'll be prompted to start your **Free Trial of Dynamics 365 Remote Assist**.

5.	You can now use Dynamics 365 Remote Assist on your mobile device. Next up, [Learn how make calls](mobile-app/making-calls-with-ar.md). 

>[!Note]
> For Enterprise environments that manage application deployments using an MDM provider, please contact d365rafb@microsoft.com for assistance obtaining the Dynamics 365 Remote Assist mobile application binary.

## Next steps
- [Set up Microsoft Teams on PC or mobile for various scenarios](set-up-teams.md).
- [Install Dynamics 365 Remote Assist model-driven app](ra-webapp-install.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]
