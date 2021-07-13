---
title: Use Dynamics 365 Remote Assist mobile in low-bandwidth situations
author: BryceHolmes
description: Learn how the Microsoft Dynamics 365 Remote Assist mobile app works in environments with poor network conditions. 
ms.author: soanigbo
ms.date: 04/08/2021
ms.service: crm-online
ms.topic: article
ms.reviewer: v-bholmes
---

# Use the Dynamics 365 Remote Assist mobile app in low-bandwidth situations

Technicians sometimes find themselves on factory floors or remote locations with poor network connectivity. Without strong network connectivity (bandwidth (up/down) of 1.5 Mbps or higher), technicians might experience difficulty troubleshooting and resolving problems in real time. Dynamics 365 Remote Assist mobile now gives technicians the ability to discuss, diagnose, and resolve issues with remote collaborators even in low bandwidth scenarios.

## What determines poor network connectivity

Poor network connectivity is determined by the following conditions:

- The bandwidth is between 150 kbps and 1.5 Mbps

- The latency is higher than 1,000 ms

- The packet loss is higher than 10 percent

Dynamics 365 Remote Assist mobile **autodetects** if the technician is experiencing poor network conditions. If so, the technician is prompted to **share snapshots** with the remote expert to collaborate, instead of transmitting a live video feed. This way, the expert can view and annotate images of better quality, instead of a low-quality video feed.

## How it works

Let's take a quick look at what happens in a field scenario when a technician encounters poor network connectivity. In this scenario, the technician is a field worker. The remote expert is elsewhere with good network conditions. 

1. The technician launches a video call with a remote expert.

    ![Side-by-side screenshots of Dynamics 365 Remote Assist on mobile and Microsoft Teams, launching a call.](./media/03.07-call-ink.png "Launch Call") 

2. In the call, Dynamics 365 Remote Assist mobile autodetects if the technician is experiencing poor network conditions. If so, the technician is prompted to use the **Snapshot** tool to share images with the remote expert. 

    ![Side-by-side screenshots of Dynamics 365 Remote Assist on mobile and Microsoft Teams, showing a low-quality image in the chat window because of poor network conditions.](./media/03.14-call-low-bandwidth-dialog.png "Detection") 

3. The technician is instructed to use the **Snapshot** tool.

    ![Side-by-side screenshots of Dynamics 365 Remote Assist on mobile and Microsoft Teams, showing the Poor Network notification and the Share Snapshot option on the mobile device screen.](./media/03.15-call-snapshot-teach.png "Share") 

4. The technician takes a snapshot, which is shared to the remote expert's screen. The expert now sees a high-quality snapshot. The technician and expert can annotate simultaneously on the snapshot.

    ![Side-by-side screenshots of Dynamics 365 Remote Assist on mobile and Microsoft Teams, showing the tooltip on mobile that prompts the technician to share a snapshot.](./media/03.16-call-snapshot-active.png "Tool Tip") 
 
5. After sharing a snapshot, the technician can save it to the mobile device's photo gallery or call chat, or can discard it. 

    ![Side-by-side screenshots of Dynamics 365 Remote Assist on mobile and Microsoft Teams, showing the snapshot on both screens.](./media/03.19-call-save-snapshot-dialog-selected.png "Expert-side Snapshot") 

6. The technician returns to the video call and can continue to send snapshots to the expert.	

    ![Side-by-side screenshots of Dynamics 365 Remote Assist on mobile and Microsoft Teams, showing annotations on the snapshot on both screens.](./media/03.21-call-save-snapshot-saved.png "Annotate")  

> [!NOTE]
> The low-bandwidth feature is not supported in group calling scenarios. 


