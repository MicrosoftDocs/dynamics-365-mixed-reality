---
author: Mamaylya
description: Learn about Microsoft Dynamics 365 Guides entities that you can use to extend Dynamics 365 if you're a developer.
ms.author: mamaylya
ms.date: 04/28/2020
ms.service: crm-online
ms.topic: article
title: Entity reference for Dynamics 365 Guides (for developers)
ms.reviewer: v-brycho
---

# Entity reference for Dynamics 365 Guides (for developers)

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

When a guide is created by using the Microsoft Dynamics 365 Guides PC app, content and information in that guide are stored by using the 
Dynamics 365 Guides [entities](https://docs.microsoft.com/powerapps/maker/common-data-service/entity-overview) from [Microsoft Dataverse](https://docs.microsoft.com/powerapps/maker/common-data-service/data-platform-intro) that are listed in the table later in this topic.

> [!IMPORTANT]
> All entities that are installed as part of the Dynamics 365 Guides solution support the standard extensibility/programming model in Dynamics 365. You can access entity information by using either the [Web application programming interface (API)](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/overview) or the [Microsoft Dataverse Organization Service](https://docs.microsoft.com/powerapps/developer/common-data-service/org-service/overview).
>
> Dynamics 365 Guides entities and fields can be used with the Web API, and in [Power Apps](https://powerapps.microsoft.com/) or a flow using [Power Automate](https://flow.microsoft.com/). However, we anticipate that these entities will evolve quickly in the near future. If you have an urgent need to do a business-critical integration, contact the Dynamics 365 Guides team directly for guidance, through your Microsoft Account team.
>
> Additionally, be careful when you programmatically create, update, or delete records for Dynamics 365 Guides entities. Some entities depend on other entities to provide user experiences and functionalities in the PC and HoloLens apps. Programmatic manipulation of these entities might prevent you from using the functionalities in the intended and supported way.

## Dynamics 365 Guides entities

| Entity name | Description |
|-------------|-------------|
| msmrw\_3dasset | This entity stores a 3D object file and information that is associated with that 3D object file. |
| msmrw\_3dasset\_localized | This entity stores localized information for a 3D object. |
| msmrw\_assetcollection | This entity stores a group of 3D objects (asset collection). |
| msmrw\_assetcollection\_localized | This entity stores localized information for an asset collection. |
| msmrw\_audioasset | This entity stores an audio file and information that is associated with that audio file. |
| msmrw\_guide | This entity stores information about the content of a guide, including its anchor information. |
| msmrw\_guidecompletionstepobject | This entity stores information about the 3D objects that have been added to the completion step of a guide. |
| msmrw\_guidecompletionstepobjectplacement | This entity specifies which 3D objects have been placed in the world in the completion step of a guide. Other information about the 3D objects is also stored. |
| msmrw\_guideevent | This entity is used to track telemetry information for a guide. |
| msmrw\_guide\_localized | This entity stores localized information for a guide. |
| msmrw\_guidestep | This entity stores content and information about a guide step. |
| msmrw\_guidestepobject | This entity stores information about 3D objects that have been added to a guide step. |
| msmrw\_guidestepobjectplacement | This entity specifies which 3D objects have been placed in the world in a guide step. Other information about the 3D objects is also stored. |
| msmrw\_guidetask | This entity is a parent container for a group of guide steps. |
| msmrw\_guideviewconfiguration | This entity stores the record ID for Microsoft Dataverse views. Each record is shown as a tab in the HoloLens app. |
| msmrw\_imageasset | This entity stores an image file and information that is associated with the image. |
| msmrw\_imageasset\_localized | This entity stores localized information for an image. |
| msmrw\_usersettings | This entity stores information about the custom setting configuration for a specific user who is using the HoloLens app. |
| msmrw\_videoasset | This entity stores a video file and information that is associated with that video file. |
| msmrw\_videoasset\_localized | This entity stores localized information for a video. |

## See also

[Entity reference for Dynamics 365](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/about-entity-reference)
