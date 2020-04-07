---
author: Mamaylya
description: Learn about Dynamics 365 Guides entities that you can use to extend Dynamics 365 if you're a developer.
ms.author: mamaylya
ms.date: 04/28/2020
ms.service: crm-online
ms.topic: article
title: Entity Reference for Dynamics 365 Guides (for developers)
ms.reviewer: v-brycho
---

# Entity Reference for Dynamics 365 Guides (for developers)

When a guide is created using the Dynamics 365 Guides PC application, content and information in that guide is stored using the 
following Dynamics 365 Guides [entities](https://docs.microsoft.com/powerapps/maker/common-data-service/entity-overview) 
in [Common Data Service](https://docs.microsoft.com/powerapps/maker/common-data-service/data-platform-intro).

>[!IMPORTANT]
>All entities installed as a part of the Dynamics 365 Guides solution support the standard extensibility/programming model in 
Dynamics 365. You can access entity information by using the [Web API](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/overview) 
or [Common Data Service Organization Service](https://docs.microsoft.com/powerapps/developer/common-data-service/org-service/overview).<br>However, 
at this time, we recommend that you use Dynamics 365 Guide entities and fields for exploration, future planning, and 
testing only when using the Web API or creating an app with [Power Apps](https://powerapps.microsoft.com/en-us/) or a flow with 
[Power Automate](https://flow.microsoft.com/en-us/). This is because we anticipate these entities will evolve quickly in the near future. 
If you have an urgent need to do a business-critical integration, contact the Dynamics 365 Guides team directly for guidance through 
your Microsoft Account team.<br>Also, be careful when programmatically creating, updating, or deleting Dynamics 365 Guides entity records. 
Some entities have a dependency on other entities to provide user experiences and functionalities in the PC and HoloLens apps. 
Manipulating these entities programmatically may prevent you from using the functionalities in the intended and supported way.

## Dynamics 365 Guides entities

|Entity name|Description|
|----------------------------------------------|--------------------------------------------------------------------------|
|msmrw_3dasset|Stores a 3D object file and information associated with that 3D object file.|
|msmrw_3dasset_localized|Stores localized information for a 3D object.|
|msmrw_assetcollection|Stores a group of 3D objects (asset collection).|
|msmrw_assetcollection_localized|Stores localized information for an asset collection.|
|msmrw_audioasset|Stores an audio file and information associated with that audio file.|
|msmrw_guide|Stores information about the content of a guide, including its anchor information.|
|msmrw_guidecompletionstepobject|Stores information about the 3D objects added to the completion step of a guide.|
|msmrw_guidecompletionstepobjectplacement|Specifies which 3D objects have been placed in the world in the completion step of a guide. Other information about the 3D objects is also stored.|
|msmrw_guideevent|Used to track telemetry information for a guide.|
|msmrw_guide_localized|Stores localized information for a guide.|
|msmrw_guidestep|Stores content and information about a guide step.|
|msmrw_guidestepobject|Stores information about 3D objects added to a guide step.|
|msmrw_guidestepobjectplacement|Specifies which 3D objects have been placed in the world in a guide step. Other information about the 3D objects is also stored.|
|msmrw_guidetask|A parent container for a group of guide steps.|
|msmrw_guideviewconfiguration|Stores the record ID for Common Data Service views. Each record is shown as a tab in the HoloLens app.|
|msmrw_imageasset|Stores an image file and information associated with the image.|
|msmrw_imageasset_localized|Stores localized information for an image. |
|msmrw_usersettings|Stores custom setting configuration info for a specific user when using the  HoloLens app.|
|msmrw_videoasset|Stores a video file and information associated with that video file.|
|msmrw_videoasset_localized|Stores localized information for a video.|

## See also

[Entity reference for Dynamics 365](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/about-entity-reference)
