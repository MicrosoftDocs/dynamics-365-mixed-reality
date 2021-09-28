---
title: Integrate Dynamics 365 Remote Assist with Power Automate
author: dhgoelmsft
description: Learn how to create a Power Automate flow based on Dynamics 365 Remote Assist entities
ms.author: dhgoel
ms.date: 06/10/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Integrate Dynamics 365 Remote Assist with Power Automate

The asset capture feature in Remote Assist leverages Common Data Service (CDS). This enables you to create Power Automate flows based on this data to streamline various processes, including getting notifications, modifying other entities, and generating reports. In this article, you'll create a flow to get an email notification whenever a new asset attachment is created.

## Prerequisites

To complete this article, you need:

- **Access to the environment Dynamics 365 Remote Assist is installed in**.
- **License and access to [Power Automate](/power-automate/)**.

## Create Flows with Power Automate

1. Go to [make.powerapps.com](https://make.powerapps.com) and sign in.
2. Select the appropriate environment where you installed the Dynamics 365 Remote Assist model-driven app.
![Screenshot of the Power Automate landing page.](media/PowerAutomate001-landingPage.png)
3. Select **Flows** from the left navigation. Select **+ New** to start creating a new flow. Select **"Automated-from blank"**
![Screenshot of the Power Automate start new flow screen.](media/PowerAutomate002-StartNewFlow.png)
4. To begin creating a new automated flow, you must select a trigger that initiates the flow. In this case, search for and select the **"When a record is created"** trigger from Common Data Service. You may also name your flow on this screen. After filling out all the details, select **Create**.
![Screenshot of the Power Automate select trigger.](media/PowerAutomate003-SelectTrigger.png)
5. Provide the details of the trigger. Here, we will select the environment and scope in which the flow will apply. For the entity name, search for and select **Customer Asset Attachment**. After that, select **+ New Step**.
![Screenshot of the Power Automate provide trigger details step.](media/PowerAutomate004-ProvideTriggerDetails.png)
6. In the **"Choose an action"** dialog box, search for mail and select the **"Send an email notification"** action.
![Screenshot of the Power Automate select email notification step.](media/PowerAutomate005-SelectEmailNotification.png)
7. Enter the email address you want to send the notification to. In the body, dynamic content within Power Automate allows us to easily craft a message including the name of the customer asset attachment entity whose creation triggered the flow.
![Screenshot of the Power Automate fill email details step.](media/PowerAutomate006-FillEmailDetails.png)
8. In the subject, we want to include the name of the customer asset entity with which the asset attachment is associated. To get the attributes (such as name) associated with the asset entity, first we'll have to fetch that entity. Select the **+ (plus icon)** between the trigger and the email notification action. Then select **"Add an action"**.
![Screenshot of the Power Automate add action in between step.](media/PowerAutomate007-AddActionInBetween.png)
9. Select **Get Record** from CDS from the actions. Select the appropriate environment and the **Customer Assets** entity. The dynamic content and CDS relationship helps you pick the customer asset associated with attachment.
![Screenshot of the Power Automate get record from CDS step.](media/PowerAutomate008-GetRecordFromCDS.png)
![Screenshot of the Power Automate get record from CDS details step.](media/PowerAutomate009-GetRecordFromCDSDetails.png)
10. Now we can go back to the **"Send an email notification"** step. This time, when searching for name in the dynamic content, we have the option of selecting the customer entity name, because we fetched the associated customer entity in the previous step. Go ahead and include that in the subject. Select **Save**. Your flow is now complete!
![Screenshot of the Power Automate email subject step.](media/PowerAutomate010-EmailSubject.png)
11. You can use the **Flow Checker** and **Test** options to validate your newly created flow.
![Screenshot of the Power Automate flow checker.](media/PowerAutomate011-flowChecker.png)

## Test your flow

1. Follow the steps in **[capture asset conditions](./asset-capture-photos.md)** to create a new asset capture entity record.
2. Go to the **Flows** page again to select the flow you created. On this page, you can see recent runs of the flow. Select most recent run to see its details.
![Screenshot of the Power Automate Test Run Flow.](media/PowerAutomate012-TestRunFlow.png)
3. If there are errors in the flow, you can select **Edit** to modify the flow. You can then resubmit the previous run to test your flow again, without having to create a new asset capture entity.
![Screenshot of the Power Automate Resubmit Flow.](media/PowerAutomate013-resubmitFlow.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
