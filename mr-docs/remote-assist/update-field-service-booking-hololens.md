---
title: Update a Dynamics 365 Field Service booking in Dynamics 365 Remote Assist on HoloLens
author: sophiasysun
description: Update a Dynamics 365 Field Service booking in Dynamics 365 Remote Assist on HoloLens
ms.date: 03/15/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Update a Dynamics 365 Field Service booking in Dynamics 365 Remote Assist on HoloLens

Empower technicians to solve problems faster by pairing Dynamics 365 Remote Assist HoloLens application with the Dynamics 365 Field Service application. This allows technicians to:

- Call the expert assigned to the booking.
- Automatically attach their call log to the Field Service work order that their booking is associated with.
- Save snapshots to their booking so technicians and inspectors can more seamlessly document their work.

With Field Service, technicians manage their assigned work orders, or the service work needed, and perform maintenance and inspections onsite at customer locations. With Remote Assist mobile, technicians, and inspectors can directly post essential call data and history to their Field Service work orders without opening their work order. 

If your organization uses Dynamics 365 Field Service to manage field service work orders and bookings and has [set up Dynamics 365 integration](./mobile-app/fs-integration.md), you can view Field Service bookings from Dynamics 365 Remote Assist and call the collaborator assigned to the booking. This allows you to do heads-up, hands-free calling through HoloLens in the context of a Field Service booking, add snapshots from the call to the booking, and add files shared during the call to the work order associated with that booking.

## View a Field Service booking and call an assigned resource

1.  From the **Call** tab, select the **[!include[pn-dyn-365](../includes/pn-dyn-365.md)]** icon to open the **Booking** pane. (Select the **[!include[pn-dyn-365](../includes/pn-dyn-365.md)]** icon again to close the **Booking** pane.)  
      
    The **Booking** pane will remain available on the right side of the window until you close it.
    
    ![Screenshot of the active bookings panel that appears on HoloLens](media/07.01-dynamics-booking.png "ViewBookings")
    
    > [!Note]
    > Only bookings with the **In Progress** status are listed. When a booking is open, any Dynamics 365 Remote Assist call you make will be associated with that booking, even if you do not collaborate with the resource listed.
    
2.  Now, you'll see booking details, including the **Work Order ID** and **Support Contact**. 

       ![Screenshot of the booking details panel.](media/RAHL_SelectedBooking.PNG)    

If you'd like to call the **Support Contact**, select their name. Then, in the filtered contacts list, select the tile for the expert. If you don’t see the contact you’re looking for, select **Search** to bring up the holographic keyboard.  
      
    
## View and update booking details during a call

During a call, you may want to view booking details, such as the start and end time of the booking, the resource assigned to the booking, and a Power BI link to relevant data. To view the booking, select Dynamics (or say, “Remote Assist, Dynamics”). 

Booking information is blurred out when you’re in a video call, but remains visible during an audio-only call.

You may update your booking status.

![MarkComplete](media/RAHL_MarkComplete.PNG "MarkComplete")

## Open a Power BI dashboard from a Dynamics 365 Field Service booking

-   Select a [!include[pn-power-bi](../includes/pn-power-bi.md)] link to open [!include[pn-power-bi](../includes/pn-power-bi.md)] Online in a browser or to open the
    [!include[pn-power-bi](../includes/pn-power-bi.md)] desktop application.
    
    > [!NOTE]
    > When you open a [!include[pn-power-bi](../includes/pn-power-bi.md)] dashboard, [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] closes. If you’re on a call with an expert, the expert will remain on the call. To return to Dynamics 365 Remote Assist, navigate to the Start menu and select the Dynamics 365 Remote Assist tile. 
    

## Modify the default booking view

To modify the default view of information in the **Booking** pane, [edit the view as
you would any Dynamics 365 view](https://docs.microsoft.com/dynamics365/customer-engagement/customize/create-and-edit-views).



[!INCLUDE[footer-include](../includes/footer-banner.md)]