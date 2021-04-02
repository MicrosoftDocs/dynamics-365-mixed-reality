---
title: Using Dynamics 365 Remote Assist HoloLens in low bandwidth scenarios
author: amaranigbo
description: How the app works in environments with low network conditions 
ms.author: soanigbo
ms.date: 04/05/2021
ms.service: crm-online
ms.topic: article
ms.reviewer: v-bholmes
---

# Use Dynamics 365 Remote Assist in low-bandwidth scenarios

Technicians sometimes find themselves on factory floors or remote locations with poor network connectivity. Without strong network connectivity (bandwidth (up/down) of 1.5 Mbps or higher), technicians may experience difficulty troubleshooting and resolving problems in real time. Dynamics 365 Remote Assist HoloLens gives technicians the ability to discuss, diagnose, and resolve issues with remote collaborators even in low-bandwidth situations.

## What determines poor network connectivity 

Poor network connectivity is determined by the following conditions: 

- The bandwidth is between 150 kbps and 1.5 Mbps

- The latency is higher than 1,000 ms

- The packet loss is higher than 10 percent

Dynamics 365 Remote Assist **autodetects** if the technician is experiencing poor network conditions. If so, the technician is prompted to **share snapshots** with the remote expert to collaborate, instead of transmitting a live video feed. This way, the expert can view and annotate high-quality images instead of a low-quality video feed.

## Components that cause poor network conditions
	
The interaction of the three components can cause poor network connectivity: **bandwidth**, **latency**, and **packet loss**:

- Minimum bandwidth (in/out) - 150 kbps / 150 kbps
- Maximum latency (in/out) - 500 ms / 500 ms (1,000 ms) 
- Maximum packet loss (in/out) - 10% / 10%  

Here's an example of a poor network profile that allows users to sign into HoloLens and connect to a call with an expert.
    
| Variables  | Measurements |
| ------------- | ------------- |
| Bandwidth  | 150 kbps / 150 kbps  |
| Latency  | 400 ms / 400 ms = 800 ms  |
| Packet loss  | 10% / 10%  |

> [!NOTE]
> Given the above known values for **bandwidth** and **packet loss**, exceeding a round trip **latency** of 800 ms will result in a slower in-app experience. These variables are interdependent and change in one variable can affect the other variables. 

## How it works

Let's take a quick look at what happens in a field scenario when a technician encounters poor network connectivity. In this scenario, the technician is a field worker. The  remote collaborator is elsewhere with good network conditions. 

1. The technician launches a video call with a remote collaborator.

    ![Screenshot of Dynamics 365 Remote Assist on HoloLens, launching a call.](./media/03.14-call-snapshot-poor-connection.png "Launch Call") 

2. In the call, Dynamics 365 Remote Assist autodetects if the technician is experiencing poor network conditions. 

    ![Screenshot of Dynamics 365 Remote Assist on HoloLens, showing a low-quality image in the chat window because of poor network conditions](./media/03.15-call-snapshot-poor-connection-message.png "Detection") 

3. The technician is prompted to use the **Snapshot** tool to share images with the expert.

    ![Screenshot of Dynamics 365 Remote Assist on HoloLens, showing the Poor Network notification and the Share Snapshot option on the HoloLens device screen.](./media/03.16-call-snapshot-poor-connection-tip.png "Share") 

4. The technician is instructed on how to use the **Snapshot tool**.

    ![Screenshots of Dynamics 365 Remote Assist on HoloLens , showing the tooltip on HoloLens that prompts the technician to share a snapshot.](./media/03.17-call-snapshot-camera.png "Tool Tip") 
 
5. The technician takes a snapshot, which is shared with the remote collaborator. The remote collaborator now sees a snapshot that has better quality. The technician and remote collaborator can annotate simultaneously on the snapshot.

    ![Screenshot of Dynamics 365 Remote Assist on HoloLens, showing the snapshot is sent.](./media/03.23-call-snapshot-sent.png "Snapshot sent")  

6. After sharing a snapshot, the technician can save it to the meeting's **chat** or **retake the snapshot**.

    ![Screenshot of Dynamics 365 on HoloLens, showing the option to either save or retake snapshot on HoloLens.](./media/03.24-call-snapshot-re-sending "Photo Gallery") 

7. The technician returns to the video call and can continue to send snapshots to the remote collaborator.

    ![Screenshot of Dynamics 365 Remote Assist on HoloLens showing the return to video call.](./media/03.25-call-snapshot-saved-to-chat "Video Feed") 

> [!NOTE]
> The low-bandwidth feature is not supported in group calling scenarios. 
