---
author: BryceHo
description: Covers Guides Analytics--Power BI reports you can use in Dynamics 365 Guides to improve process efficiencies.
ms.author: cynielse
ms.date: 02/02/2021
ms.service: crm-online
ms.topic: article
title: Overview of Guides Analytics, Power BI reports for Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Analyze guides created with Dynamics 365 Guides

![Video camera graphic](media/video-camera.PNG "Video camera graphic") [Watch a video on analyzing your guides with Power BI reports](https://aka.ms/guidesanalyze)<br>
 
Guides Analytics is part of the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] application suite that includes the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] PC authoring app and the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] [!include[pn-hololens](../includes/pn-hololens.md)] app. Use Guides Analytics to analyze the usage of guides across your organization. Guides Analytics consists of [!include[pn-power-bi](../includes/pn-power-bi.md)] visual reports that are populated with [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] session data stored securely in your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] environment. 

> [!NOTE]
> Guides Analytics is intended to help supervisors and managers derive insights regarding operational efficiencies and usage of Dynamics 365 Guides. This feature is not intended for use in making (and should not be used to make) decisions that affect the employment of an employee or group of employees, including compensation, rewards, seniority, or other rights or entitlements. Customers are solely responsible for using Dynamics 365, this feature, and any associated feature or service in compliance with all applicable laws, including laws relating to accessing individual employee analytics and monitoring. Customers are encouraged to have a mechanism in place to inform their users that analytics relating to their guides usage is collected.

## What data is collected and used in Guides Analytics? 

When an operator uses the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] [!include[pn-hololens](../includes/pn-hololens.md)] app in Operate mode, each interaction that moves the operator forward, backward, or out of the guide is recorded, together with the date and time of the interaction. Each operation of a guide in [!include[pn-hololens](../includes/pn-hololens.md)] Operate mode, whether completed from beginning to end of the guide or involving just a few steps, is called a *guide session*. Information about the guide session, such as time spent on a step, step number, task number, total operating time, and different options to define completion (was the completion step visited or what percentage of steps did the operator visit) are also recorded. This data is stored in your private and secure [!include[pn-dyn-365](../includes/pn-dyn-365.md)] environment.  

## What can you do with the data? 

One way to interact with the data is to utilize the Guides Analytics reports, and another way is to use [Microsoft Power Automate to automate workflows](https://docs.microsoft.com/power-automate/), for example when a new guide session starts or ends.  

The Guides Analytics reports are designed to help you answer high-level questions about guides usage. For example: 

- How many guides have been used to date? 
 
- Is the number of times a guide is operated per day increasing, decreasing, or remaining stable over time? 

- Which guides take the most time to complete? 

- Are operators completing the guide or only going through half the steps?

You can also use Guides Analytics to drill into detailed time-tracking information at the task and step levels. For example, answer questions such as: 

- Which step of a guide takes the most time? 

- Which step of a guide has the most variability in operator time? 

- Is the amount of operation time equally distributed between tasks?

These reports provide information about operator adoption and usage and give guide authors a data-driven way to improve their 
guides. For example, an author could focus their editing efforts on steps that take a long time to execute or show a high 
degree of variability among operators. These reports are also valuable in training scenarios for both trainers and trainees 
to better understand performance and improvement over time.  


 

 
## See also

![Video camera graphic](media/video-camera.PNG "Video camera graphic") [Analyze your guides](https://aka.ms/guidesanalyze)<br>
![Doc graphic](media/doc-icon.PNG "Doc graphic") [Overview of authoring a guide](authoring-overview.md)</br>
![Doc graphic](media/doc-icon.PNG "Doc graphic") [Overview of operating a guide](operator-overview.md)</br>
![Doc graphic](media/doc-icon.PNG "Doc graphic") [FAQ](faq.md)



