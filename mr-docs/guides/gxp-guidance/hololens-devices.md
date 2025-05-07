---
title: HoloLens devices
description: Learn about setting up and maintaining HoloLens devices in a regulated industry.
ms.date: 03/21/2023
ms.topic: article
author: prashantyvr
ms.author: prashan
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# HoloLens devices

Use of Dynamics 365 Guides in regulated industries requires two types of devices to run the relevant software: PCs and HoloLens devices. We recommend that the business maintains tight control over these devices. If Good \{industry\} Practice (GxP) requirements apply, work with the appropriate quality assurance (QA) staff to determine what level of validation is required for those devices.

Because we assume that your organization already has PCs enrolled in your IT infrastructure, this article discusses only HoloLens devices.

## HoloLens device setup

Familiarize yourself with the hardware:

- [Introduction to HoloLens](/hololens/hololens2-hardware)
- [Choose the right HoloLens edition](/hololens/hololens2-options) – Will the devices be used in standard, regulated, or safety-controlled physical environments?
- [Procure HoloLens](/hololens/hololens2-purchase) – Find an authorized reseller that is relevant to your implementation plans and that supports the countries or regions that are involved.

To enroll HoloLens devices, your mobile device management (MDM)/endpoint management specialists must:

- Decide which [HoloLens deployment scenario](/hololens/hololens-requirements#scenario-a) is relevant to your situation and organization, and follow the related deployment guide.
- [Deploy and manage endpoints (HoloLens devices) through Microsoft Endpoint Manager](/hololens/hololens-mdm-configure): [Intune](/mem/endpoint-manager-overview). In Intune, you can enable and disable device settings and features, and automatically add devices to a group so that they inherit a specific configuration profile.
- Consider the connectivity method for HoloLens devices, and the potential coverage. Will [Wi-Fi certificates](/hololens/hololens-certificates-network) be part of the deployment, or will other means of network control be established?

Your organization should consider the relevance and effectiveness of:

- [Windows Autopilot](/hololens/hololens2-autopilot), to deploy devices at scale.
- [Kiosk mode](/hololens/hololens-kiosk), to control selectable applications in a user context.
- [Windows Update for Business](/mem/intune/protect/windows-update-for-business-configure), for automation and customization of the operating system update process.
- [Windows Hello for Business](/windows/security/identity-protection/hello-for-business/hello-overview), for strong two-factor authentication on devices.

However, be sure to adhere to your organization's requirements for security and user experience.

We recommend that you use Windows Autopilot and Intune to ensure proper governance for the deployment of HoloLens devices and the Guides app. With these management tools, you can control when an update is pushed to the devices. In some cases, it might be beneficial to delay an update to a HoloLens device or PC until a proper risk assessment and test areconducted, or until a required upgrade to the Microsoft Power Platform environment is done.

## User-based versus device-based setup

Depending on use case, cost, operation, and organizational policies, HoloLens and Guides can be operated in a user-based or [device-based](../device-license.md) setup. In a user-based setup, individuals have their own Guides account. In a device-based setup, multiple individuals use a single device under a shared user account.

Usually, because of regulatory requirements, all authors and approvers of guides must have individual users. In other words, the licensing structure must be user-based for those personas. In addition, if your organization has operators who will be regular users of guides, we recommend that you have individual usage accounts.

For operators who will be only occasional users of guides, a device-based setup can make sense from an operational and cost perspective. However, the regulatory requirements that you're subject to might demand a user-based setup to ensure traceability.

In general, a user-based setup is recommended in regulated industries. Together with [Power BI](/power-bi/) statistics, a user-based setup enables logging of actions and ensures complete traceability in relation to auditing.

If you choose a user-based setup and operate in the European Union (EU), ensure that any processing or analysis of personal data in reports complies with [General Data Protection Regulation](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) (GDPR) through policies such as:

- Collecting and processing only the minimum amount of personal data that is necessary to achieve the intended purpose.
- Informing users about the purpose and scope of data processing activities and their rights under GDPR.

Always consult legal counsel or a GDPR specialist to ensure that your logging of actions complies with all relevant GDPR policies.

If you prefer to run a device-based setup but don't want to sacrifice traceability, your organization can use [digital signatures](electronic-records-and-electronic-signature.md) whenever an action is completed.

## HoloLens device maintenance

Maintenance of HoloLens devices helps ensure that they are running efficiently and effectively. Regular maintenance can prevent equipment failure and prolong the lifespan of the equipment. Best practices for maintaining devices include:

- [Charging the HoloLens](/hololens/hololens2-charging).
- [Cleaning the HoloLens](/hololens/hololens2-maintenance).
- [Restarting, resetting, or recovering the HoloLens](/hololens/hololens-recovery) if users experience issues with it.
- Checking whether your organization is covered under [warranty](https://support.microsoft.com/warranty) if the device is broken.

A charged, clean, and functional device is always important for individual safety and for instant availability of specific guides for operation. However, if you run a device-based setup where a HoloLens device is shared among employees, your organization can't rely on best practices alone. It also needs a governance model for the operation of devices. Such a governance model includes but isn't limited to information about how to book HoloLens devices, how to register them as unavailable because of software errors or hardware damage, and where to store and charge them.

## HoloLens device storage in cabinets with charging capabilities

For seamless daily use of HoloLens devices, we recommend that you store devices in cabinets that have charging capabilities. The benefits of doing so include:

- **Organization**: The devices of your unit, factory, or department are organized in one place. Therefore, they are easier to find and use.
- **Instant availability**: Charging capabilities in the cabinet ensure that devices are always charged and ready to use when they are needed. In a worst-case scenario, devices that have an empty battery can lead to production downtime if guides are used to follow standard operating procedures (SOPs), and no back-up solutions, such as paper-based instructions, are available.
- **Safety**: Cabinets that have charging capabilities can help keep cords out of sight. In this way, they help reduce clutter and the risk of tripping. Therefore, workplace safety is improved.
- **Life span extension**: By storing HoloLens devices in a cabinet, your organization helps protect them from being taken, knocked over, or damaged. Therefore, the life span of devices is extended.

## HoloLens device tracking

Your organization can use a small Bluetooth or GPS tracker that is placed on each device or in its protective carrying case to keep track of the location and movement of the device. Trackers can mitigate the risk of:

- **Misplacement**: Devices are easily lost or forgotten if they are frequently moved between production stations and sites. The risk is particularly high if there isn't clear governance about who brings what, when, and where.
- **Theft**: HoloLens is a valuable mobile device that weighs only 566 grams. Therefore, it's easy and attractive to steal.
- **Equipment damage**: Extend the life span of your HoloLens devices by ensuring that they aren't left in hazardous places where they could be damaged.

## Next steps

- [Microsoft Power Platform environments](power-platform-environments.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
