


# Integrate Dynamics 365 for Field Service with Dynamics 365 Guides

Dynamics 365 for Field Service integration (included in version 104.1907.XXXX) enables Field Service 
customers to attach guides to field service tasks in Dynamics 365. When work orders are assigned to technicians, 
the technicians can use a dedicated tab in the Guides HoloLens app to retrieve and launch the assigned guide and do their work.

ADD SCREENSHOT HERE (select-guide)

## Prerequisites

Integration between Dynamics 365 Guides and Dynamics 365 Field Service requires:

- A Dynamics 365 instance (not a Common Data Service instance) with Field Service version 8.6.0.183 or later.

- Dynamics 365 Guides Common Data Service version 104.1907.0.18 or later. [Learn how to upgrade the Dynamcis 365 Guides 
solution.](upgrade.md)

- Dynamics 365 Guides PC and HoloLens app versions 104.1907.XXXX or later. [Learn how to install the apps.]()

## Enable your technicians to use Dynamics 365 Guides for work orders

1. Create a guide using hte Dynamics 365 Guides PC and HoloLens apps. For information on creating a guide, see:
  
   - [Use the PC authoring app to create a guide](pc-authoring.md)
   
   - [Use the HoloLens app to place your holograms](hololens-authoring.md)
   
2. Create a Field Service work order and attach a service task to it:

   1. To create a new work order in Dynamics 365 for Field Service, select **Word Orders**, and then select **New Work Order**.
   
      ADD SCREENSHOT HERE (create-work-order)
      
   2. In the **Service Tasks** view, select the More info button (...), and then select **Add New Work Order Service Task**.
   
      ADD SCREENSHOT HERE (add-new-task)
      
   3. In the **New Work Order Service Task** view, select a task type, provide an optional description, and then select a 
   guide to associate with the service task. Select ** Save** when you're done.
   
      ADD SCREENSHOT HERE (new-work-order-options)
      
      
      
      
   
