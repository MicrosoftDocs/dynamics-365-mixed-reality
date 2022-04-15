---
title: Dynamics 365 Field Service integration with Dynamics 365 Remote Assist mobile
author: amaraanigbo
description: How Dynamics 365 Field Service integration works with Dynamics 365 Remote Assist mobile
ms.author: soanigbo
ms.date: 07/01/2020
ms.topic: article
ms.reviewer: v-bholmes
---

# Use Dynamics 365 Field Service with Dynamics 365 Remote Assist mobile

By pairing the Microsoft Dynamics 365 Remote Assist mobile application with Dynamics 365 Field Service, organizations can seamlessly capture relevant contextual information from their technicians in the field. Field service technicians can:

- Use Dynamics 365 Field Service mobile to launch the Dynamics 365 Remote Assist mobile app and make calls to remote collaborators on both iOS and Android devices.

- Seamlessly post call history to their Dynamics 365 Field Service work order at the end of a Dynamics 365 Remote Assist mobile call, including:

   - Call logs, including time, date, call duration, and the remote collaborator's name
   - File URLs
   - In-call snapshot URLs

## Prerequisites

- Complete the setup instructions for [Dynamics 365 Field Service integration](../troubleshoot-field-service.md). 

## How it works

1. At the end of a Dynamics 365 Remote Assist mobile call, if no files, images, or snapshots are shared, the field technician is prompted to post their call log to their Dynamics 365 Field Service work order. The technician selects **Post**.

    ![Screenshot of Dynamics 365 Remote Assist on a mobile device showing the end of a call, with the option to post the call log to a work order.](./media/postfs_2.png "Call log")

    If files, images, and/or snapshots are shared in the Dynamics 365 Remote Assist text chat, the technician will see a list with their call log and files, images, and snapshots that can be posted to the work order. To post everything, the field technician selects **Post All**.

    > [!Tip]
    > To post the Dynamics 365 Remote Assist call recording to a work order, copy and paste the OneDrive for Business or SharePoint URL from the Microsoft Teams chat into the work order. Remember to adjust the OneDrive for Business or SharePoint permissions to allow access to others.

    ![Screenshot of Dynamics 365 Remote Assist on a mobile device showing the list of items in the call log after the call has ended.](./media/postfs_1.png) 

3. If active bookings have been assigned to the technician through Dynamics 365 Field Service, they'll appear in the **Select a Booking** list. The technician can select a booking, and then select **Post** to post it to the work order.

    ![Screenshot of Dynamics 365 Remote Assist mobile showing available bookings pulled in from Field Service.](./media/post_1.png "Select Booking")

   If no bookings appear in the technician's account, they can refresh their screen or discard the post.

    ![Screenshot of Dynamics 365 Remote Assist mobile showing the option to refresh Dynamics 365.](./media/post_3.png "No Bookings")

   > [!NOTE]
   > If the technician still doesn't see the booking they're looking for, it might be because they have access to multiple instances (organizations). They can select the **More** (ellipsis) button to return to their instance, and then select another instance. 

    ![Screenshot of Dynamics 365 Remote Assist mobile showing the Select an Instance screen.](./media/post_2.png "Select Instance")

4. The technician returns to their contact list and will be notified when their call log and files have successfully been posted to their work order. Then they can sign in to their work order.

    ![Screenshot of Dynamics 365 Remote Assist mobile on the contacts list, showing a notification that says items have been posted to a work order.](./media/postfs_3.png "End of call notification")

5. The technician can go to the work order and view the call log and files that have been posted from Dynamics 365 Remote Assist mobile. They can then copy and paste the files URL in a new tab to view the files.

    > [!Note]
    > If someone (such as an admin or dispatcher) viewing the work order wants to view the files, they must request access to the technician's files on OneDrive for Business. 

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
