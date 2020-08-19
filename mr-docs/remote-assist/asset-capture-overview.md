---
title: Asset capture overview for Dynamics 365 Remote Assist
author: dhgoelmsft
description: Overview of the asset capture public preview 
ms.author: dhgoel
ms.date: 08/19/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Asset capture public preview overview

Using the asset capture public preview in Dynamics 365 Remote Assist, technicians can capture data about the assets they operate, inspect, and maintain without their having to make a video call. Data is captured in a consistent and structured way, and made available through the new Dynamics 365 Remote Assist model-driven app for easy validation, report generation, and auditing.

The Dynamics 365 Remote Assist model-driven app is built on Common Data Service and uses Common Data Model. This app is a companion to the Dynamics 365 Remote Assist apps for HoloLens, iOS, and Android, and enables new scenarios for managing data generated and consumed by Dynamics 365 Remote Assist.

More information: [What are model-driven apps in Power Apps?](https://docs.microsoft.com/powerapps/maker/model-driven-apps/model-driven-app-overview)

Compared to the snapshot tool for capturing images that's currently available in Dynamics 365 Remote Assist, asset capture has several benefits:

- **Available independent of calls**: Technicians can use Dynamics 365 Remote Assist to capture processes such as inspections, audits, repair procedures, and factory acceptance tests without having to make a video call. This is great for scenarios where technicians are working by themselves or when a video call isn't possible. Asset capture, spatial markup tools, and reference documents are now always available the moment you open Dynamics 365 Remote Assist.
- **More flexible and robust**: Asset capture is built on Common Data Service and Common Data Model. Data generated in Dynamics 365 Remote Assist can be used in automated processes with Power Automate flows or in your existing Dynamics 365 apps and apps built on Power Apps. Because Dynamics 365 Remote Assist uses the same customer asset entity used in Field Service, Connected Field Service, and Supply Chain Management, Dynamics 365 Remote Assist seamlessly extends those applications, enabling technicians to capture spatial data to the asset from Dynamics 365 Remote Assist.
- **Easier to manage**: Data captured with asset capture is automatically related back to a digital record of the equipment (assets) you maintain and operate. Over time, these records become a historical record and audit trail of rich spatial data captured from Dynamics 365 Remote Assist. And compared to OneDrive where the user must share the folder with specific individuals for viewing, asset data is saved to Common Data Service so anyone in the organization with access to Common Data Service can view data from Dynamics 365 Remote Assist.

Asset capture is easy to use:

1. An admin installs the Dynamics 365 Remote Assist app in a Dynamics 365 environment.
2. The admin adds Dynamics 365 Remote Assist users to the environment.
3. The admin manually creates digital asset records or imports existing data to Common Data Service.
4. A technician enables the asset capture preview on HoloLens.
5. The technician completes their work (an inspection, for example) and captures the inspection data to the asset record through Dynamics 365 Remote Assist.
6. The captured data is available to view.

> [!Note]
> Asset capture is in public preview and only available on HoloLens 1 and HoloLens 2. The feature is disabled by default when the update is downloaded, to ensure that current users won't be negatively affected by the workflow changes. The tutorials in this section will guide you through getting started with asset capture, including enabling the features in HoloLens.

## Next step

Use the following tutorial to get started with the asset capture public preview.

> [!div class="nextstepaction"]
> [Set up an environment](./asset-capture-setup-environment.md)

## Additional notes

- Dynamics 365 Remote Assist uses the same common solution for the asset entity that Dynamics 365 Field Service uses. If you have Field Service installed in the same environment as Dynamics 365 Remote Assist, you'll see a new tab on the customer asset form called **Captures**.
- Support for HoloLens and mobile devices isn't part of the June public preview, but is planned for a future release. For more information, see: [2020 release wave 2 for Dynamics 365 Remote Assist](https://docs.microsoft.com/dynamics365-release-plan/2020wave2/service/dynamics365-remote-assist/planned-features)
- Support for video capture isn't available in the June release, but is planned for a future release.
- During sign-in, Dynamics 365 Remote Assist will try to automatically select the first environment the user has access to that has the Dynamics 365 Remote Assist app installed. If the user has access to more than one environment that has the Dynamics 365 Remote Assist app installed, they can choose the environment they want by selecting **Settings** > **Links** > **Switch Dynamics Instance**.
- Fields such as account, product, category, and asset hierarchy aren't visible in HoloLens. Over time, we'll add more support for relevant fields in the Dynamics 365 Remote Assist HoloLens and mobile apps.
- The snapshot tool has been replaced with asset capture capabilities. Select an asset from the **Assets** tab, and then use the camera tool to take photos. You can re-enable the snapshot tool by turning off the asset capture feature from **Settings**.

### Entity reference

Asset capture uses several entities stored in Common Data Model:

- **Customer Asset**: The individual asset. This entity is also used in Dynamics 365 Field Service and Connected Field Service. More info: [msdyn_customerasset EntityType](https://docs.microsoft.com/dynamics365/customer-engagement/web-api/msdyn_customerasset?view=dynamics-ce-odata-9)
- **Customer Asset Category**: A way to describe a group of similar assets.
- **Customer Asset Attachment**: A media artifact of a single asset, captured in HoloLens.
- **Account**: The customer account where the asset currently exists.
- **Product**: The make and model of the asset.

### Known issues

- Users with access to a large number of environments will experience long delays the first time they sign in to Dynamics 365 Remote Assist with the preview turned on. It can take Dynamics 365 Remote Assist a long time to find an environment that has the app installed.
- An environment set through **Settings** won't be saved after you restart the app. The environment needs to be reset through **Settings** > **Links** > **Switch Dynamics Instance**.
- Taking multiple photos in succession can be slow, or might fail entirely.
- Photos taken in Dynamics 365 Remote Assist have a limited resolution of 1280 &times; 720, lower than the maximum resolution available on the HoloLens headset.
- Captures viewed from the model-driven app might not appear the first time you load the capture. If you don't see the asset capture, refresh the page and the capture preview will appear.
- Dynamics 365 Remote Assist supports a maximum of 5,000 asset records.
- Dynamics 365 Remote Assist on HoloLens won't automatically update the list of asset records. If you create or update an asset from the model-driven app and don't see it in HoloLens, restart Dynamics 365 Remote Assist on HoloLens by closing the live tile and reopening the app.
