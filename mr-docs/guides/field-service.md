---
author: davepinch
description: How to integrate Dynamics 365 Field Service with Dynamics 365 Guides so Field Service technicians can follow a guide while doing a work order
ms.author: davepinch
ms.date: 11/08/2023
ms.topic: how-to
title: Integrate Dynamics 365 Field Service with Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Integrate Dynamics 365 Field Service with Dynamics 365 Guides

<!---
> ![Video camera graphic](media/video-camera.PNG "Video camera graphic") [Watch a video on integrating Dynamics 365 Field Service with Dynamics 365 Guides](https://www.youtube.com/watch?v=IzTU-6o1XqE) --->

Microsoft Dynamics 365 Field Service integration enables Field Service customers to attach guides to Field Service tasks in Dynamics 365 Field Service. When work orders are assigned to technicians, the technicians can use a dedicated **Field Service** tab in the Dynamics 365 Guides HoloLens app to launch the assigned guide and do their work.

<!-- How to add a guide to service task? FS and Guides on same env only prereq?-->

## Enable your technicians to use Dynamics 365 Guides for work orders

1. Create a guide using the Dynamics 365 Guides PC and HoloLens apps. For information on creating a guide, see:
  
   - [Use the PC authoring app to create a guide](pc-app-overview.md)

   - [Use the HoloLens app to place your holograms](hololens-app-overview.md)

1. [Create a work order](/dynamics365/field-service/create-work-order) in Field Service.

1. [Add a service task](/dynamics365/field-service/set-up-service-task-types) to the work order.

   1. In the **Service Tasks** view, select the **More Commands** button (...), and then select **Add New Work Order Service Task**.

   1. In the **New Work Order Service Task** view, select a task type, provide an optional description, and then select a guide to associate with the service task. Select **Save** when you're done.

      ![Select task type and associate guide.](media/new-work-order-options.PNG "Select task type and associate guide")

1. [Schedule the work order](/dynamics365/field-service/schedule-work-order) to a resource.

After the technician signs in to the Dynamics 365 Guides app on HoloLens, they see the **Field Service** tab. This tab shows the guides, which relate to service tasks they're assigned to. There's also a short description of the booking and the work order.

   > ![Select guide.](media/field-service-guides-integration-over.png "Select guide")

The Guides HoloLens app shows work orders for the current day and the following eight days. Work orders appear in the HoloLens app until they're marked as **Complete** in Field Service or assigned to someone else.

## Known issues

- Service task names that are longer than approximately 50 characters are cut off in the HoloLens user interface.

- When assigning a guide to a Field Service service task, you can also create a new guide. Don't use this option to create a new guide. Guides must be created using the Dynamics 365 Guides PC app or HoloLens app.

## Next steps

[Overview of Dynamics 365 Field Service](/dynamics365/field-service/overview)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
