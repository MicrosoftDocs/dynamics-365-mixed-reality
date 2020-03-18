---
title: Dynamics 365 Field Service integration with Remote Assist mobile
author: xonatia
description: How Dynamics 365 Field Service integration works with Remote Assist mobile
ms.author: xolee
ms.date: 02/27/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Use Dynamics 365 Field Service with Remote Assist mobile 

By pairing the Dynamics 365 Remote Assist mobile application with Dynamics 365 Field Service, field service technicians can: 

1. Use Field Service mobile to launch the Remote Assist mobile app and make calls to remote experts on their Android devices.

2. Automatically post **call logs**, such as time, date, call duration, and the expert's name, and **files shared** in the Remote Assist text chat into their Field Service work order at the end of a Remote Assist mobile call.

## Prerequisites 
- In order to follow along with this guide, you should have completed the set up instructions for Field Service and Remote Assist integration. Learn how to set up the Dynamics 365 Field Service app to launch calls to Remote Assist mobile on your Android devices [here](../troubleshoot-field-service.md). 

## How it works

Now that we have it enabled, let's see how integration with Field Service works for Remote Assist mobile.

1.	At the end of a Remote Assist mobile call, you are prompted to post your call log, if no files are shared, to your Field Service work order. Select **Post**.

![Call log](./media/postfs_1.png "Call log only")

2. If files are shared during your Remote Assist call, you will see a list with your call log and files that you can post to your Field Service work order. Select **Post**.

![List view](./media/postfs_2.png "Call log and Files")

3. If you have **active bookings** assigned to you through Field Service, you'll see them listed. Select your booking and select **Post**.

    ![Screenshot of Remote Assist mobile showing available bookings pulled in from Field Service.](./media/selectbooking.png "Select Booking")

4. If you have no bookings assigned to your account, you can **Refresh** your screen or **Discard** your post.

![Screenshot of Remote Assist mobile showing the option to refresh Dynamics 365.](./media/fs_6.png "No Bookings")

5.	If you still don't see the booking you're looking for, it might be because you have access to multiple instances (organizations). You can select the **Ellipses** icon to return to your instance, and then select another **Instance**. Then continue from **Step 2**.
###
![Screenshot of Remote Assist mobile showing the Select an Instance screen](./media/Instance.png "Select Instance")
### 

6.	You will return to the **Contact information** for the expert you just got off the call with.

![Screenshot of Remote Assist mobile showing the contact information of the remote expert.](./media/fs_5.png "Booking")

7. In your contact list, you will be notified that your call log and files have successfully been posted to your Field Service work order and you can sign in to your work order.

![Notification](./media/postfs_3.png "End of call notification")

8. The technician can go to the work order and find the call logs and files. They can copy and paste the files URL in a new tab to view the files.  
