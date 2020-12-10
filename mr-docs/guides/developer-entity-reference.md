---
author: Mamaylya
description: Learn about Microsoft Dynamics 365 Guides tables (entities) that you can use to extend Dynamics 365 if you're a developer.
ms.author: mamaylya
ms.date: 12/10/2020
ms.service: crm-online
ms.topic: article
title: Dataverse table reference for Dynamics 365 Guides (for developers)
ms.reviewer: v-brycho
---

# Table (entity) reference for Dynamics 365 Guides (for developers)

When a guide is created with the Microsoft Dynamics 365 Guides PC app, content and information in that guide are stored by using the 
Dynamics 365 Guides [tables](https://docs.microsoft.com/powerapps/maker/common-data-service/entity-overview) from [Microsoft Dataverse](https://docs.microsoft.com/powerapps/maker/common-data-service/data-platform-intro) that are listed later in this topic.

> [!IMPORTANT]
> All tables that are installed as part of the Dynamics 365 Guides solution support the standard extensibility/programming model in Dynamics 365. You can access table information by using either the [Web application programming interface (API)](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/overview) or the [Microsoft Dataverse Organization Service](https://docs.microsoft.com/powerapps/developer/common-data-service/org-service/overview).
>
> Dynamics 365 Guides tables and columns can be used with the Web API, and in [Power Apps](https://powerapps.microsoft.com/) or a flow using [Power Automate](https://flow.microsoft.com/). However, we anticipate that these tables will evolve quickly in the near future. If you have an urgent need to do a business-critical integration, contact the Dynamics 365 Guides team directly for guidance, through your Microsoft Account team.
>
> Additionally, be careful when you programmatically create, update, or delete records for Dynamics 365 Guides tables. Some tables depend on other tables to provide user experiences and functionalities in the PC and HoloLens apps. Programmatic manipulation of these tables might prevent you from using the functionalities in the intended and supported way.

## Dynamics 365 Guides entities

| Table name | Description |
|-------------|-------------|
| msmrw\_3dasset | This table stores a 3D object file and information that is associated with that 3D object file. |
| msmrw\_3dasset\_localized | This table stores localized information for a 3D object. |
| msmrw\_assetcollection | This table stores a group of 3D objects (asset collection). |
| msmrw\_assetcollection\_localized | This table stores localized information for an asset collection. |
| msmrw\_audioasset | This table stores an audio file and information that is associated with that audio file. |
| msmrw\_guide | This table stores information about the content of a guide, including its anchor information. |
| msmrw\_guidecompletionstepobject | This table stores information about the 3D objects that have been added to the completion step of a guide. |
| msmrw\_guidecompletionstepobjectplacement | This table specifies which 3D objects have been placed in the world in the completion step of a guide. Other information about the 3D objects is also stored. |
| msmrw\_guideevent | This table is used to track telemetry information for a guide. |
| msmrw\_guide\_localized | This table stores localized information for a guide. |
| msmrw\_guidestep | This table stores content and information about a guide step. |
| msmrw\_guidestepobject | This table stores information about 3D objects that have been added to a guide step. |
| msmrw\_guidestepobjectplacement | This table specifies which 3D objects have been placed in the world in a guide step. Other information about the 3D objects is also stored. |
| msmrw\_guidetask | This table is a parent container for a group of guide steps. |
| msmrw\_guideviewconfiguration | This table stores the record ID for Microsoft Dataverse views. Each record is shown as a tab in the HoloLens app. |
| msmrw\_imageasset | This table stores an image file and information that is associated with the image. |
| msmrw\_imageasset\_localized | This table stores localized information for an image. |
| msmrw\_usersettings | This table stores information about the custom setting configuration for a specific user who is using the HoloLens app. |
| msmrw\_videoasset | This table stores a video file and information that is associated with that video file. |
| msmrw\_videoasset\_localized | This table stores localized information for a video. |

## See also

[Entity reference for Dynamics 365](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/about-entity-reference)
