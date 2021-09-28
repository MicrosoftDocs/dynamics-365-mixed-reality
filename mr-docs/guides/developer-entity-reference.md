---
author: Mamaylya
description: Learn about Microsoft Dynamics 365 Guides tables (entities) that you can use to extend Dynamics 365.
ms.author: mamaylya
ms.date: 05/04/2021
ms.topic: article
title: Dataverse table (entity) reference for Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Microsoft Dataverse table (entity) reference for Dynamics 365 Guides

When a guide is created with the Microsoft Dynamics 365 Guides PC app, content and information in that guide are stored by using the 
Dynamics 365 Guides [tables](/powerapps/maker/common-data-service/entity-overview) from [Microsoft Dataverse](/powerapps/maker/common-data-service/data-platform-intro) that are listed later in this topic.

> [!IMPORTANT]
> All tables that are installed as part of the Dynamics 365 Guides solution support the standard extensibility/programming model in Dynamics 365. You can access table information by using either the [Web application programming interface (API)](/powerapps/developer/common-data-service/webapi/overview) or the [Microsoft Dataverse Organization Service](/powerapps/developer/common-data-service/org-service/overview).
>
> Dynamics 365 Guides tables and columns can be used with the Web API, and in [Power Apps](https://powerapps.microsoft.com/) or a flow using [Power Automate](https://flow.microsoft.com/). However, we anticipate that these tables will evolve quickly in the near future. If you have an urgent need to do a business-critical integration, contact the Dynamics 365 Guides team directly for guidance, through your Microsoft Account team.
>
> Additionally, be careful when you programmatically create, update, or delete records for Dynamics 365 Guides tables. Some tables depend on other tables to provide user experiences and functionalities in the PC and HoloLens apps. Programmatic manipulation of these tables might prevent you from using the functionalities in the intended and supported way.

## Dynamics 365 Guides tables

| Table name | Description |
|-------------|-------------|
| msmrw\_3dasset | Stores a 3D object file and information associated with that 3D object file. |
| msmrw\_3dasset\_localized | Stores localized information for a 3D object. |
| msmrw\_assetcollection | Stores a group of 3D objects (asset collection). |
| msmrw\_assetcollection\_localized | Stores localized information for an asset collection. |
| msmrw\_audioasset | Stores an audio file and information associated with that audio file. |
| msdyn\_mrfolder | A parent container for a group of guides.|
| msmrw\_guide | Stores information about the content of a guide, including its anchor information. |
| msmrw\_guidecompletionstepobject | Stores information about the 3D objects that have been added to the completion step of a guide. |
| msmrw\_guidecompletionstepobjectplacement | Specifies which 3D objects have been placed in the world in the completion step of a guide. Other information about the 3D objects is also stored. |
| msmrw\_guideevent | Used to track telemetry information for a guide.<br><br> **Note:** This table will be deprecated in the near future.|
|msmrw_guidesession |	Stores information about the duration, progress, and status of an operator's guide sessions.|
|msmrw_guidesessionstepvisit| Stores information about every operator visit to a step.|
| msmrw\_guide\_localized | Stores localized information for a guide. |
| msmrw\_guidestep | Stores content and information about a guide step. |
| msmrw\_guidestepobject | Stores information about 3D objects that have been added to a guide step. |
| msmrw\_guidestepobjectplacement | Specifies which 3D objects have been placed in the world in a guide step. Other information about the 3D objects is also stored. |
| msmrw\_guidetask | Parent container for a group of guide steps. |
| msmrw\_guideviewconfiguration | Stores the record ID for Microsoft Dataverse views. Each record is shown as a tab in the HoloLens app. |
| msmrw\_imageasset | Stores an image file and information associated with the image. |
| msmrw\_imageasset\_localized | Stores localized information for an image. |
| msmrw\_usersettings | Stores information about the custom setting configuration for a specific user who is using the HoloLens app. |
| msmrw\_videoasset | Stores a video file and information that is associated with that video file. |
| msmrw\_videoasset\_localized | Stores localized information for a video. |

## See also

- [Create a guide with Microsoft Power Automate](workflow-create-guide.md)
- [Entity reference for Dynamics 365](/dynamics365/customerengagement/on-premises/developer/about-entity-reference)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
