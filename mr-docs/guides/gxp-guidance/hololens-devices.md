---
title: 
description: 
ms.date: 03/09/2023
ms.topic: 
ms.service: 
author: 
ms.author: 
manager: 
---

# HoloLens Devices

Guides usage in regulated industries requires two types of devices, Personal Computers and HoloLens devices, to run the relevant software. It is recommended for the business to be in tight control of these. In the case that GxP requirements apply, it must be considered what level of validation is required for these with the respective QA staff of responsibility.

It is assumed that your organization already has personal computers enrolled into your IT infrastructure. Therefore, you'll only find information and links related to HoloLens in this section.

## Setup HoloLens devices

Familiarize yourself with the hardware:

-   [Introduction to HoloLens](https://learn.microsoft.com/en-us/hololens/hololens2-hardware)

-   [Choose the right HoloLens edition](https://learn.microsoft.com/en-us/hololens/hololens2-options) – are the device(s) to be used in standard, regulated, or safety-controlled physical environments?

-   [Procure HoloLens](https://learn.microsoft.com/en-us/hololens/hololens2-purchase) devices – find an authorized reseller that is relevant for your implementation plans and support the countries you are rolling out to.

To enroll HoloLens devices, your mobile device management (MDM) / endpoint management specialists need to:

-   Decide which [HoloLens deployment scenario](https://learn.microsoft.com/en-us/hololens/hololens-requirements#scenario-a) is relevant for your situation and organization and follow the related deployment guide.

-   [Deploy and manage endpoints (HoloLens devices) through Microsoft's Endpoint Manager](https://learn.microsoft.com/en-us/hololens/hololens-mdm-configure): [Intune](https://learn.microsoft.com/en-us/mem/endpoint-manager-overview). In Intune, you can enable and disable device settings and features, and automatically add devices to a group for them to inherit a specific configuration profile.

-   Consider the connectivity method for HoloLens devices and the potential coverage. Will [WiFi certificates](https://learn.microsoft.com/en-us/hololens/hololens-certificates-network) be part of the deployment or will other means of control to the network of use be established.

Furthermore, your organization should consider the relevance and effectiveness of:

-   [Windows Autopilot](https://learn.microsoft.com/en-us/hololens/hololens2-autopilot) – to deploy devices at scale

-   [Kiosk mode](https://learn.microsoft.com/en-us/hololens/hololens-kiosk?tabs=uisak%2Cautologon) - for controlling selectable applications in an end-user context

-   [Windows Update for Business](https://learn.microsoft.com/en-us/mem/intune/protect/windows-update-for-business-configure) – for automation and customization of the OS update process

-   [Windows Hello for Business](https://learn.microsoft.com/en-us/windows/security/identity-protection/hello-for-business/hello-overview) – for strong two-factor authentication on devices.

However, make sure to adhere to your organization's requirements regarding security and end-user experience.

It is recommended to utilize Windows Autopilot and Intune to ensure a proper governance for deploying HoloLens devices and the Guides app. With these management tools, you can control when an update should be pushed to the devices. In some instances, it might be beneficial to delay an update to a HoloLens and/or PC until a proper risk assessment and test has been conducted or a required upgrade to the Power Platform environment has been performed.

## User-based versus device-based setup 

Depending on use case, cost, operation, and organizational policies, HoloLens as well as Guides can be operated in a user-based or [device-based](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/device-license) setup. In the former setup, individuals have their own Guides account, while a single device is used by multiple individuals under a shared user account in the latter setup.  
  
Usually, due to regulatory requirements, all authors and approvers of guides need to have individual users, meaning the licensing structure must be user-based for these personas. If your organization has operators who will be regular users of guides, these are recommended to have individual usage accounts as well.

For sporadic guides operators, a device-based setup can make sense from an operational and cost perspective but the regulatory requirements you are subject to might demand a user-based setup to ensure traceability.

In general, however, the user-based setup is recommended within regulated industries. Together with [Power BI](https://learn.microsoft.com/en-us/power-bi/) statistics, a user-based setup enables logging of actions and ensures complete traceability in relation to auditing.  
  
If you choose this setup and operate within EU, you must ensure that any personal data that is processed or analyzed in reports is done so in compliance with [General Data Protection Regulation](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) (GDPR). This includes but is not limited to policies such as 1) only collecting and processing the minimum amount of personal data necessary to achieve the intended purpose, and 2) informing users of the purpose and scope of data processing activities and their rights under GDPR. Always consult with a legal counsel or a GDPR specialist to ensure that your logging of actions comply with all relevant GDPR policies.

If you prefer to run a device-based setup without sacrificing traceability, your organization has the option to utilize digital signatures whenever an action is completed.**  
**

## Maintain HoloLens devices

Maintenance of the HoloLens devices helps to ensure that the device is running efficiently and effectively. Regular maintenance can prevent equipment failure and prolong the lifespan of the equipment. Best practices for maintaining devices include: 

-   [<u>Charge the HoloLens</u>](https://learn.microsoft.com/en-us/hololens/hololens2-charging) 

-   [<u>Clean the HoloLens</u>](https://learn.microsoft.com/en-us/hololens/hololens2-maintenance)

-   [<u>Restart, reset, or recover HoloLens</u>](https://learn.microsoft.com/en-us/hololens/hololens-recovery) - if experiencing issues with devices

-   Check if your organization is covered by [<u>warranty</u>](https://support.microsoft.com/en-us/warranty) - if your device is broken. 

A charged, clean, and functional device is always important for individual safety as well as for instant availability of specific guides for operation. However, if you run a device-based setup where a HoloLens device is shared among employees, your organization can't rely on best practices but will also need a governance model for the operation of devices. This includes but is not limited to information on how to book HoloLens devices, register them as unavailable due to software errors or hardware damage, and where to store or charge them. 

## Store HoloLens devices in cabinets with charging capabilities

For a more seamless daily use of HoloLens devices, it is recommended to store devices in cabinets with charging capabilities. Benefits of doing so include:

- **Organization**: The devices of your unit, factory, or department are organized in one place, making it easier to find and utilize them.   
     

- **Instant availability**: Charging capabilities in the cabinet ensures that devices are always charged and ready to use when they are needed. At worst, devices with empty battery can result in production downtime, if guides are used for following SOPs and no back-up solutions, like paper-based instructions, are available. 

- **Safety**: Cabinets with charging capabilities can help keep cords out of sight, meaning clutter is reduced and the risk of tripping reduced. In this way, workplace safety is improved.   
      

- **Life span extension**: When HoloLens devices are stored in a cabinet, your organization protects devices from being taken, knocked over, or damaged, extending the life span of devices. 

## Track your HoloLens devices

Your organization can use small Bluetooth or GPS trackers placed on a device or in its protective carrying case to keep track of the location and movement of your devices. Trackers can mitigate the risk of: 

 

- **Misplacement**: Devices are easily lost or forgotten if they are frequently moved between production stations and sites. This is particularly true if governance around who brings what, when, and where is unclear.   
     

- **Theft**: HoloLens is a valuable mobile device with a weight of only 566 grams. This makes it easy and attractive to steal.   
     

- **Equipment damage**: Extend the life span of your HoloLens devices by ensuring they are not left in hazardous places potentially damaging the device.


