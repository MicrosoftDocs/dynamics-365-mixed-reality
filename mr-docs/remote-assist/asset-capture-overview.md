---
title: Asset Capture Overview 
author: bencorn
description: Overview of the Asset Capture Public Preview 
ms.author: becorn
ms.date: 5/30/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Asset Capture Public Preview Overview

## Overview
The Asset Capture public preview introduces non-calling scenarios in Remote Assist by enabling technicians to capture data about the assets they operate, inspect, and maintain. The data is captured in a consistent and structured way and made available through the new Remote Assist model-driven app for easy validation, report generation, and auditing by stakeholders and other technicians.

The Remote Assist model-driven app is built on the Common Data Service platform and utilizes the Common Data Model. This app is a companion to the Remote Assist apps for HoloLens, iOS, and Android that enables new scenarios for managing data generated and consumed by Remote Assist.

To learn more about Dynamics 365 model-driven apps, see: [What are model-driven apps in Power Apps?](https://docs.microsoft.com/powerapps/maker/model-driven-apps/model-driven-app-overview)

Compared to the snapshot tool currently available in Remote Assist for capturing images, asset capture has several additional benefits:

- **Available independent of calls**: technicians can use Remote Assist to capture processes such as inspections, audits, repair procedures, and factory acceptance tests **independent of a call**. This is great for scenarios where they are working by themselves or a video call is not possible. Simply put, asset capture, spatial markup tools, and reference documents are now always available from the second you start Remote Assist.
- **More flexible and robust**: Asset Capture is built on Common Data Service and the Common Data Model. Data generated in Remote Assist can be used in automated processes with Power Automate Flows or in your existing Dynamics 365 apps and Power Apps. Because Remote Assist uses the same Customer Asset entity used in Field Service and Connected Customer Service, Remote Assist seamlessly extends those applications, enabling technicians to capture spatial data to the asset from Remote Assist.
- **Easier to manage**: Data captured with Asset Capture is automatically related back to a digital record of the equipment (assets) you maintain and operate. Overtime, these records become a historical record and audit trail of rich spatial data captured from Remote Assist. And compared to OneDrive where the user must share the folder with specific individuals for viewing, asset data is saved to Common Data Service so anyone in the organization with access to Common Data Service (CDS) can view data from Remote Assist.

Asset Capture is easy to start using and involves the following steps:

1. Administrator installs the Dynamics 365 Remote Assist app on a Dynamics 365 environment.
2. Administrator adds Remote Assist users to the environment.
3. Administrator manually creates digital asset records or imports existing data to Remote Assist.
4. Technician enables the Asset Capture preview on their HoloLens.
5. Technician completes their work, such as an inspection, and captures the inspection data to the asset record through Remote Assist.
6. View the captured data.

> [!NOTE]
> Asset Capture is in public preview and currently only available on HoloLens 2. The feature is disabled by default when you download the update to ensure your current users are not impacted by the workflow changes in this update. The following tutorials will guide you through how to get started with Asset Capture, including enabling the features in the HoloLens 2.

## Next steps

Get started with the Asset Capture public preview by starting with this tutorial:

> [!div class="nextstepaction"]
> [Setup an environment](./asset-capture-setup-environment.md)

## Additional notes

- Remote Assist uses the same common solution for the Asset entity that Dynamics 365 Field Service uses. If you have Field Service installed in the same environment as Remote Assist, you will see a new tab on the Customer Asset form called **Captures**.
- Support for HoloLens 1 and Mobile isn't part of the June public preview and is **planned**.
- Support for video capture isn't available in the June release and is **planned**
- During sign-in, Remote Assist will try to automatically select the first environment the user has access to with the Remote Assist app installed. If the user has access to more than one environment with the Remote Assist app installed, the desired environment can be set by selecting **Settings** > **Links** > **Switch Dynamics Instance**.
- Fields such as Account, Product, Category, and asset hierarchy are not visible in the HoloLens. Overtime we will add more support for relevant fields in the Remote Assist client apps.

### Entity reference

Asset Capture uses several entities stored in Common Data Model:

- **Customer Asset**: the individual asset. This entity is also used in Dynamics 365 Field Service and Connected Field Service. Find more information about this entity here: [msdyn_customerasset EntityType](https://docs.microsoft.com/dynamics365/customer-engagement/web-api/msdyn_customerasset?view=dynamics-ce-odata-9)
- **Customer Asset Category**: a way to describe a group of similar assets.
- **Customer Asset Attachment**: a media artifact captured in HoloLens of a single asset.
- **Account**: the customer account where the asset currently exists.
- **Product**: the make/model of the asset.

### Known issues

- Users with access to a large number of environments will experience long delays the first time they sign into Remote Assist with the preview turned on.
- An environment set through Settings will not be saved after restarting the app. The environment needs to be re-set through **Settings** > **Links** > **Switch Dynamics Instance**.
- Taking multiple photos in succession can fail or be slow.
- Photos taken in Remote Assist have a limited resolution of 1280x720; lower than the maximum resolution available on the HoloLens.
- Captures viewed from the model-driven app may not appear the first time when loading the capture. If this happens, refresh the page and the capture preview will appear.
- Maximum support for 5,000 asset records.
- Remote Assist on HoloLens will not automatically update the list of asset records. If you create or update an asset from the model-driven app and do not see it in the HoloLens, restart Remote Assist on HoloLens by closing the live tile and reopening the app.

### Troubleshooting

#### The Remote Assist app isn't showing up in Power Platform Admin Center

1. Check to ensure you have an active Dynamics 365 Remote Assist subscription.
2. Try assigning a Remote Assist license to your account from [Microsoft 365 Admin Center](https://admin.microsoft.com) to force a sync to occur. Wait 5 minutes and see if the app appears in [Power Platform Admin Center](https://admin.powerplatform.com). The license can be unassigned afterwards.
3. File a **support request** by navigating to [Power Platform Admin Center](https://admin.powerplatform.com) > **Help + support** > **New support request**.

#### I can't find the Remote Assist model-driven app

1. Check to see if you are accessing the right environment by checking the environment name in the URL.
2. Ensure the app was installed to the desired environment. Learn more: [Install Dynamics 365 Remote Assist model-driven app](./asset-capture-setup-environment.md#install-dynamics-365-remote-assist-model-driven-app)
3. The user must have the **Remote Assist - App User** role and **Common Data Service User** security roles assigned. Learn here: [Assign Dynamics 365 security roles](./asset-capture-add-users.md#assign-dynamics-365-security-roles)
4. The app must be enabled for the **Remote Assist - App User** role. Learn more: [Manage app roles](./asset-capture-add-users.md#manage-app-roles)

#### The environment I installed Remote Assist in doesn't appear in the HoloLens

Follow steps 2 and 3 from above.

#### The Snapshot tool is missing

The snapshot tool has been replaced with the Asset Capture capabilities. Select an asset from the **Assets** tab and use the camera tool to take photos. You can re-enable the snapshot tool by turning off the Asset Capture feature from **Settings**.

#### The Remote Assist model-driven app failed to install because of missing dependencies

This will occur if you try installing Remote Assist in an environment that is not **Dynamics 365 apps enabled**. Try installing the app in an environment where other Dynamics apps are available, such as Field Service or Sales, or create a new environment that is Dynamics 365 apps enabled. Learn more: [Create a new environment](./asset-capture-setup-environment.md#install-dynamics-365-remote-assist-model-driven-app)
