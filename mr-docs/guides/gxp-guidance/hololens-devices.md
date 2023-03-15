---
title: HoloLens devices
description: Learn about setting up and maintaining HoloLens devices in a regulated industry
ms.date: 03/13/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# HoloLens devices

Guides usage in regulated industries requires two types of devices to run the relevant software: PCs and HoloLens devices. We recommend the business be in tight control of these devices. In the case that GxP requirements apply, consider what level of validation is required for these devices with the respective QA staff of responsibility.

We assume that your organization already has personal computers enrolled into your IT infrastructure. Therefore, this topic discusses HoloLens devices only.

## Setup HoloLens devices

Familiarize yourself with the hardware:

- [Introduction to HoloLens](/hololens/hololens2-hardware)

- [Choose the right HoloLens edition](/hololens/hololens2-options) – are the device(s) to be used in standard, regulated, or safety-controlled physical environments?

- [Procure HoloLens](/hololens/hololens2-purchase) devices – find an authorized reseller that is relevant for your implementation plans and support the countries involved.

To enroll HoloLens devices, your mobile device management (MDM) / endpoint management specialists need to:

- Decide which [HoloLens deployment scenario](/hololens/hololens-requirements#scenario-a) is relevant for your situation and organization and follow the related deployment guide.

- [Deploy and manage endpoints (HoloLens devices) through Microsoft's Endpoint Manager](/hololens/hololens-mdm-configure): [Intune](/mem/endpoint-manager-overview). In Intune, you can enable and disable device settings and features, and automatically add devices to a group for them to inherit a specific configuration profile.

- Consider the connectivity method for HoloLens devices and the potential coverage. Will [WiFi certificates](/hololens/hololens-certificates-network) be part of the deployment or will other means of control to the network be established?

Your organization should consider the relevance and effectiveness of:

- [Windows Autopilot](/hololens/hololens2-autopilot) – to deploy devices at scale.

- [Kiosk mode](/hololens/hololens-kiosk) - for controlling selectable applications in an end-user context.

- [Windows Update for Business](/mem/intune/protect/windows-update-for-business-configure) – for automation and customization of the OS update process.

- [Windows Hello for Business](/windows/security/identity-protection/hello-for-business/hello-overview) – for strong two-factor authentication on devices.

However, make sure to adhere to your organization's requirements regarding security and end-user experience.

We recommend utilizing Windows Autopilot and Intune to ensure a proper governance for deploying HoloLens devices and the Guides app. With these management tools, you can control when an update should be pushed to the devices. In some instances, it might be beneficial to delay an update to a HoloLens and/or PC until a proper risk assessment and test has been conducted or a required upgrade to the Power Platform environment has been performed.

## User-based versus device-based setup

Depending on use case, cost, operation, and organizational policies, HoloLens as well as Guides can be operated in a user-based or [device-based](../device-license.md) setup. In user-based setup, individuals have their own Guides account, while a single device is used by multiple individuals under a shared user account in a device-based setup.  
  
Usually, due to regulatory requirements, all authors and approvers of guides need to have individual users, meaning the licensing structure must be user-based for these personas. If your organization has operators who will be regular users of guides, we recommend having individual usage accounts as well.

For sporadic guides operators, a device-based setup can make sense from an operational and cost perspective but the regulatory requirements you are subject to might demand a user-based setup to ensure traceability.

In general, the user-based setup is recommended within regulated industries. Together with [Power BI](/power-bi/) statistics, a user-based setup enables logging of actions and ensures complete traceability in relation to auditing.  
  
If you choose this setup and operate within EU, ensure that any personal data that is processed or analyzed in reports is done so in compliance with [General Data Protection Regulation](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) (GDPR). This includes but is not limited to policies such as:

- Collecting and processing only the minimum amount of personal data necessary to achieve the intended purpose
- Informing users of the purpose and scope of data processing activities and their rights under GDPR

Always consult with a legal counsel or a GDPR specialist to ensure that your logging of actions complies with all relevant GDPR policies.

If you prefer to run a device-based setup without sacrificing traceability, your organization has the option to utilize digital signatures whenever an action is completed.  

## Maintain HoloLens devices

Maintenance of the HoloLens devices helps to ensure that the device is running efficiently and effectively. Regular maintenance can prevent equipment failure and prolong the lifespan of the equipment. Best practices for maintaining devices include:

- [Charge the HoloLens](/hololens/hololens2-charging)

- [Clean the HoloLens](/hololens/hololens2-maintenance)

- [Restart, reset, or recover the HoloLens](/hololens/hololens-recovery) if experiencing issues with a device

- Check if your organization is covered by [warranty](https://support.microsoft.com/en-us/warranty) if your device is broken.

A charged, clean, and functional device is always important for individual safety as well as for instant availability of specific guides for operation. However, if you run a device-based setup where a HoloLens device is shared among employees, your organization can't rely on best practices but will also need a governance model for the operation of devices. This includes but is not limited to information on how to book HoloLens devices, register them as unavailable due to software errors or hardware damage, and where to store or charge them.

## Store HoloLens devices in cabinets with charging capabilities

For a seamless daily use of HoloLens devices, we recommend storing devices in cabinets with charging capabilities. Benefits of doing so include:

- **Organization**: The devices of your unit, factory, or department are organized in one place, making it easier to find and utilize them.

- **Instant availability**: Charging capabilities in the cabinet ensures that devices are always charged and ready to use when they are needed. At worst, devices with an empty battery can result in production downtime, if guides are used for following SOPs and no back-up solutions, like paper-based instructions, are available.

- **Safety**: Cabinets with charging capabilities can help keep cords out of sight, meaning clutter is reduced and the risk of tripping reduced. In this way, workplace safety is improved.

- **Life span extension**: When HoloLens devices are stored in a cabinet, your organization protects devices from being taken, knocked over, or damaged, extending the life span of devices.

## Track your HoloLens devices

Your organization can use small Bluetooth or GPS trackers placed on a device or in its protective carrying case to keep track of the location and movement of your devices. Trackers can mitigate the risk of:

- **Misplacement**: Devices are easily lost or forgotten if they are frequently moved between production stations and sites. This is particularly true if governance around who brings what, when, and where is unclear.

- **Theft**: HoloLens is a valuable mobile device with a weight of only 566 grams. This makes it easy and attractive to steal.

- **Equipment damage**: Extend the life span of your HoloLens devices by ensuring they are not left in hazardous places potentially damaging the device.

## Next steps

- [Power Platform environments](power-platform-environments.md)
