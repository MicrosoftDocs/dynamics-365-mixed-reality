

# Troubleshoot Field Service integration with Dynamics 365 Remote Assist

If your organization uses [Dynamics 365 for Field Service](https://dynamics.microsoft.com/en-us/field-service/overview/?&OCID=AID720979_SEM_yeaT05hp&lnkd=Bing_D365_Brand) to manage field service work orders, 
the first-line worker using HoloLens can view Dynamics 365 for Field Service bookings from Remote Assist and 
quickly call the expert listed in the **Support Contact** field when needed. This enables first-line workers 
to do heads-up, hands-free calling through HoloLens in the context of a Dynamics 365 for Field Service booking.

This topic describes:

- Requirements for Field Service integration
- How to make sure Field Service is set up correctly 
- How to upgrade the Dynamics 365 instance if you don’t have the correct Field Service version
- How to add data for required fields in a Field Service work order and booking
- How to customize the **Dynamics 365** pane that appears in Remote Assist

## Requirements

Before you begin, make sure you have the following set up:

- A Microsoft Azure tenant with a Dynamics 365 subscription **and** a Dynamics 365 Remote Assist subscription. Both are required—Remote Assist is not included in any Dynamics 365 bundle.

<NOTE>
  
The tenant can have more than one Dynamics 365 instance. Remote Assist has the option to select an instance from within the app.

- You must have admin access to add or update the Dynamics 365 tenant instance.
- The Dynamics 365 instance must have the Field Service app installed, and it must include the **My In Progress Bookings** view. To make sure this view is installed, we recommend Field Service version 8.1 or later. This topic describes how to make sure you have the correct version and view.
- The tenant must have at least two user accounts.
- The user accounts must have the following licenses assigned:
  - Office 365 license that includes Microsoft Teams
  - Remote Assist
  - A Dynamics 365 license that includes Field Service
