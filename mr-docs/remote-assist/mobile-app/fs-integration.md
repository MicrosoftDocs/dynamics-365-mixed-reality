---
title: D365 Field Service Integration
author: xonatia
description: How D365 Integration works
ms.author: xolee
ms.date: 02/27/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Use Dynamics 365 Field Service with Remote Assist Mobile 

By pairing Dynamics 365 Remote Assist Mobile application with Dynamics 365 Field Service, field service technicians can: 
1. use the Field Service Mobile app to launch the Remote Assist Mobile app and make calls to remote experts on their Android devices
2. automatically post call logs, such as time, date, call duration, and the expert's name, into their Field Service work order at the end of a Remote Assist Mobile call

## Prerequisites 
- Learn how to set up the Dynamics 365 Field Service app to launch calls to Remote Assist Mobile on your Android devices [here](../troubleshoot-field-service.md). 

## How it works

Now that we have it enabled, let's see how integration with Field Service works for Remote Assist Mobile.

1.	At the end of a Remote Assist Mobile call, you are prompted to post your call metadata to your Field Service work order. Select **Post**.

    ![Screenshot of Remote Assist Mobile showing the option to post call information to a work order.](./media/fs_1.png "End Call")

2.	If you have **active bookings** assigned to you through Field Service, you'll see them listed. Select your booking and select **Post**.

    ![Screenshot of Remote Assist Mobile showing available bookings pulled in from Field Service.](./media/selectbooking.png "Select Booking")

3.	You will return to the **Contact information** for the expert you just got off the call with.

![Screenshot of Remote Assist Mobile showing the contact information of the remote expert.](./media/fs_5.png "Booking")

4.	If you have no bookings assigned to your account, you can **Refresh** your screen or **Discard** your post.

![Screenshot of Remote Assist Mobile showing the option to refresh Dynamics 365.](./media/fs_6.png "No Bookings")

5.	If you still don't see the booking you're looking for, it might be because you have access to multiple instances (organizations). You can select the **Ellipses** icon to return to your instance, and then select another **Instance**. Then continue from **Step 2**.
###
![Screenshot of Remote Assist Mobile showing the Select an Instance screen](./media/Instance.png "Select Instance")
### 
