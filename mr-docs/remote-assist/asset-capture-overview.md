---
title: Asset capture overview for Dynamics 365 Remote Assist
author: bencorn
description: Overview of the Asset Capture Public Preview 
ms.author: becorn
ms.date: 06/10/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Asset capture public preview overview

The asset capture public preview introduces non-calling scenarios in Remote Assist by enabling technicians to capture data about the assets they operate, inspect, and maintain. The data is captured in a consistent and structured way and made available through the new Remote Assist model-driven app for easy validation, report generation, and auditing.

The Remote Assist model-driven app is built on Common Data Service and utilizes Common Data Model. This app is a companion to the Remote Assist apps for HoloLens, iOS, and Android that enables new scenarios for managing data generated and consumed by Remote Assist.

To learn more about Dynamics 365 model-driven apps, see: [What are model-driven apps in Power Apps?](https://docs.microsoft.com/powerapps/maker/model-driven-apps/model-driven-app-overview)

Compared to the snapshot tool currently available in Remote Assist for capturing images, asset capture has several additional benefits:

- **Available independent of calls**: Technicians can use Remote Assist to capture processes such as inspections, audits, repair procedures, and factory acceptance tests **independent of a call**. This is great for scenarios where technicians are working by themselves, or when a video call isn't possible. Asset capture, spatial markup tools, and reference documents are now always available  the moment you launch Remote Assist.
- **More flexible and robust**: Asset capture is built on Common Data Service and Common Data Model. Data generated in Remote Assist can be used in automated processes with Power Automate flows or in your existing Dynamics 365 apps and Power Apps. Because Remote Assist uses the same customer asset entity used in Field Service, Connected Field Service, and Supply Chain Management, Remote Assist seamlessly extends those applications, enabling technicians to capture spatial data to the asset from Remote Assist.
- **Easier to manage**: Data captured with asset capture is automatically related back to a digital record of the equipment (assets) you maintain and operate. Over time, these records become a historical record and audit trail of rich spatial data captured from Remote Assist. And compared to OneDrive where the user must share the folder with specific individuals for viewing, asset data is saved to Common Data Service so anyone in the organization with access to Common Data Service can view data from Remote Assist.

Asset capture is easy to use and involves the following steps to get started:

1. Administrator installs the Dynamics 365 Remote Assist app in a Dynamics 365 environment.
2. Administrator adds Remote Assist users to the environment.
3. Administrator manually creates digital asset records or imports existing data to Common Data Service.
4. Technician enables the asset capture preview on their HoloLens.
5. Technician completes their work, such as an inspection, and captures the inspection data to the asset record through Remote Assist.
6. View the captured data.

> [!Note]
> Asset capture is in public preview and currently only available on HoloLens 2. The feature is disabled by default when you download the update to ensure your current users are not impacted by the workflow changes. The following tutorials will guide you through how to get started with asset capture, including enabling the features in HoloLens 2.

## Next steps

Get started with the asset capture public preview with the following tutorial.

> [!div class="nextstepaction"]
> [Setup an environment](./asset-capture-setup-environment.md)

## Additional notes

- Remote Assist uses the same common solution for the asset entity that Dynamics 365 Field Service uses. If you have Field Service installed in the same environment as Remote Assist, you'll see a new tab on the customer asset form called **Captures**.
- Support for HoloLens 1 and mobile devices isn't part of the June public preview, but is **planned**.
- Support for video capture isn't available in the June release, but is **planned**.
- During sign-in, Remote Assist will try to automatically select the first environment the user has access to with the Remote Assist app installed. If the user has access to more than one environment with the Remote Assist app installed, the desired environment can be set by selecting **Settings** > **Links** > **Switch Dynamics Instance**.
- Fields such as account, product, category, and asset hierarchy are not visible in the HoloLens. Over time, we will add more support for relevant fields in the Remote Assist client apps.
- The snapshot tool has been replaced with the asset capture capabilities. Select an asset from the **Assets** tab and use the camera tool to take photos. You can re-enable the snapshot tool by turning off the Asset Capture feature from **Settings**.

### Entity reference

Asset capture uses several entities stored in Common Data Model:

- **Customer Asset**: The individual asset. This entity is also used in Dynamics 365 Field Service and Connected Field Service. More info: [msdyn_customerasset EntityType](https://docs.microsoft.com/dynamics365/customer-engagement/web-api/msdyn_customerasset?view=dynamics-ce-odata-9)
- **Customer Asset Category**: A way to describe a group of similar assets.
- **Customer Asset Attachment**: A media artifact captured in HoloLens of a single asset.
- **Account**: The customer account where the asset currently exists.
- **Product**: The make and model of the asset.

### Known issues

- Users with access to a large number of environments will experience long delays the first time they sign into Remote Assist with the preview turned on as Remote Assist tries to find an environment with the app installed.
- An environment set through **Settings** will not be saved after restarting the app. The environment needs to be reset through **Settings** > **Links** > **Switch Dynamics Instance**.
- Taking multiple photos in succession can be slow or may fail.
- Photos taken in Remote Assist have a limited resolution of 1280x720, lower than the maximum resolution available on the HoloLens.
- Captures viewed from the model-driven app may not appear the first time when loading the capture. If you don't see the asset capture, refresh the page and the capture preview will appear.
- Maximum support for 5,000 asset records.
- Remote Assist on HoloLens will not automatically update the list of asset records. If you create or update an asset from the model-driven app and do not see it in the HoloLens, restart Remote Assist on HoloLens by closing the live tile and reopening the app.
