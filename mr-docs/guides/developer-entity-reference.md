
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
