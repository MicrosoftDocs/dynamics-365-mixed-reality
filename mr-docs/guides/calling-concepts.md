---
title: Guides call types   
author: prashantyvr
description: Learn about the supported Dynamics 365 Guides call types and who can collaborate
ms.author: prashan
ms.date: 04/04/2023
ms.topic: conceptual
ms.reviewer: v-wendysmith
---

# Guides call types

Dynamics 365 Guides supports the following types of calls:  

- **One-to-one call**. A [one-to-one call](calling-start-call.md#start-a-one-to-one-call) includes two participants. For example, if you need help with a machine that you're repairing, start a one-to-one call with a remote expert.

- **Group call**. A [group call](calling-start-call.md#start-a-group-call) includes three or more participants. For example, if you're inspecting an asset in a one-to-one call but need a third person's expertise, either call participant can add the third person to form a group call.

- **Meeting**. A meeting is a call scheduled through Teams or Outlook. Meetings can include any number of participants. For example, if you want to have a weekly inspection with your team, create a meeting so that everyone receives notifications about the meeting and can [join the meeting](calling-meetings.md).

> [!NOTE]
> An administrator can remove the ability for a Dynamics 365 Guides user to share outgoing video in a call. In this case, the remote collaborator joins the call with audio only. [Learn more about Teams policies supported by Dynamics 365 Guides.](admin-teams-policies.md)

## Who can collaborate on a call?

A Dynamics 365 Guides HoloLens user can collaborate with:

- A Teams desktop user (PC or Mac) or Teams mobile user on a one-to-one call, group call, or scheduled meeting. To learn more about different combinations of HoloLens and Teams users on group calls, see [Group calls](#group-calls).

- A Dynamics 365 Remote Assist mobile user on a one-to-one or group call.

> [!NOTE]
> The mixed-reality toolbar doesn't appear if the Dynamics 365 Guides user joins the call from two different devices.

## Group calls

A group call can include a Dynamics 365 Guides user on HoloLens and a Teams user or Dynamics 365 Remote Assist mobile user. You can combine HoloLens users with Teams users in different combinations:

- Multiple HoloLens users can collaborate on the same Dynamics 365 Guides call.

- Any Teams desktop user can choose any HoloLens user's space to annotate on if there's more than one HoloLens user.

  > [!NOTE]
  > A Teams mobile user cannot annotate in a group call.

- Multiple Teams desktop users can annotate on the same HoloLens user's space at the same time.

## Spotlight in Dynamics 365 Guides

Dynamics 365 Guides supports [Teams spotlighting](https://support.microsoft.com/en-us/office/spotlight-someone-s-video-in-a-teams-meeting-58be74a4-efac-4e89-a212-8d198182081e). When someone is spotlighted in Teams, the video feed in Dynamics 365 Guides changes to show the spotlighted person. If the spotlighted person is the Dynamics 365 Guides user, the user will see a notification above the video feed that indicates that they've been spotlighted.

A Dynamics 365 Guides user cannot spotlight anyone else on the call, including themselves.  

## Outgoing video quality is adjusted if the HoloLens device gets too hot

If you're on a longer call, the HoloLens device can become hot if it's using several device capabilities at the same time (for example, multiple cameras, Mixed Reality Capture, and Wi-Fi). To extend the length of the call and keep the device from overheating, Dynamics 365 Guides gradually reduces outgoing video quality. If this happens, you'll see a series of messages to let you know how and why the outgoing video quality is being adjusted. [Learn more about how Dynamics 365 Guides automatically adjusts video quality.](calling-hololens-thermal-adjusting.md)

## Next steps

- [Start a call](calling-start-call.md)
- [Join a meeting](calling-meetings.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
