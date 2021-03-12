---
title: Asset capture overview for Dynamics 365 Remote Assist
author: dhgoelmsft
description: Overview of the asset capture feature
ms.author: dhgoel
ms.date: 09/23/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Asset capture overview

[!INCLUDE[cc-data-platform-banner](../includes/cc-data-platform-banner.md)]

Using the asset capture feature in Dynamics 365 Remote Assist, technicians can capture data about the assets they operate, inspect, and maintain without them having to make a video call. Data is captured in a consistent and structured way, and made available through the new Dynamics 365 Remote Assist model-driven app for easy validation, report generation, and auditing.

Compared to the snapshot tool for capturing images that's currently available in Dynamics 365 Remote Assist, asset capture has several benefits:

- **Available independent of calls**: Technicians can use Dynamics 365 Remote Assist to capture processes such as inspections, audits, repair procedures, and factory acceptance tests without having to make a video call. This is great for scenarios where technicians are working by themselves or when a video call isn't possible. Asset capture, spatial markup tools, and reference documents are now always available the moment you open Dynamics 365 Remote Assist.
- **More flexible and robust**: Asset capture is built on Common Data Service and Common Data Model. Data generated in Dynamics 365 Remote Assist can be used in automated processes with Power Automate flows or in your existing Dynamics 365 apps and apps built on Power Apps. Because Dynamics 365 Remote Assist uses the same customer asset entity used in Field Service, Connected Field Service, and Supply Chain Management, Dynamics 365 Remote Assist seamlessly extends those applications, enabling technicians to capture spatial data to the asset from Dynamics 365 Remote Assist.
- **Easier to manage**: Data captured with asset capture is automatically related back to a digital record of the equipment (assets) you maintain and operate. Over time, these records become a historical record and audit trail of rich spatial data captured from Dynamics 365 Remote Assist. And compared to OneDrive where the user must share the folder with specific individuals for viewing, asset data is saved to Common Data Service so anyone in the organization with access to Common Data Service can view data from Dynamics 365 Remote Assist.

Asset capture is easy to use:

1. An admin installs the Dynamics 365 Remote Assist app in a Dynamics 365 environment.
2. The admin adds Dynamics 365 Remote Assist users to the environment.
3. The admin manually creates digital asset records or imports existing data to Common Data Service.
4. A technician selects the Dynamics 365 environment where Remote Assist app in installed in the client app.
5. The technician completes their work (an inspection, for example) and captures the inspection data to the asset record through Dynamics 365 Remote Assist.
6. The captured data is available to view.

## Next steps

To use the Asset capture feature of Dynamics 365 Remote Assist, check out the following series of articles:

1. [Installing the model-driven app](./ra-webapp-install.md)
2. [Adding users to the environment](./asset-capture-add-users.md)
3. [Importing and creating asset records](./asset-capture-create-asset.md)
4. Capturing pictures and videos with spatial markup on [HoloLens](./asset-capture-photos.md) and Mobile
5. [Reviewing asset captures from the Dynamics 365 Remote Assist model-driven app](./asset-capture-review.md)
6. [Creating Power Automate flows to automate business processes with captured asset data](./integrate-power-automate.md)

## Additional notes

- Dynamics 365 Remote Assist uses the same common solution for the asset entity that Dynamics 365 Field Service uses.
- Video capture length is currently limited to 30-45 seconds depending upon device. Support for longer video captures is planned for a future release.
- After signing in to the client application, the user must select the environment with Dynamics 365 Remote Assist model-driven app installed. This can be done by going into **Settings**. This is the environment from which asset data will be fetched and new assets and captures will be added to.

### Entity reference

Asset capture uses several entities stored in Common Data Model:

- **Customer Asset**: The individual asset. This entity is also used in Dynamics 365 Field Service and Connected Field Service. More info: [msdyn_customerasset EntityType](https://docs.microsoft.com/dynamics365/customer-engagement/web-api/msdyn_customerasset)
- **Customer Asset Category**: A way to describe a group of similar assets.
- **Customer Asset Attachment**: A media artifact of a single asset, captured in HoloLens.
- **Account**: The customer account where the asset currently exists.
- **Product**: The make and model of the asset.

### Known issues

- Dynamics 365 Remote Assist supports a maximum of 5,000 asset records.
- Dynamics 365 Remote Assist on HoloLens won't automatically update the list of asset records. If you create or update an asset from the model-driven app and don't see it in HoloLens, restart Dynamics 365 Remote Assist on HoloLens by closing the live tile and reopening the app.


[!INCLUDE[footer-include](../includes/footer-banner.md)]