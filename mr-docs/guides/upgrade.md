---
author: Mamaylya
description: Learn how to upgrade the Microsoft Dynamics 365 Guides solution when a new release requires an update.
ms.author: mamaylya
ms.date: 01/28/2020
ms.service: crm-online
ms.topic: article
title: Upgrade the Dynamics 365 Guides solution
ms.reviewer: v-brycho
---

# Upgrade the Dynamics 365 Guides solution

This topic is for [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365](../includes/pn-dyn-365.md)] administrators. Some releases of [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] require an update to the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution. When an update is required, the user will see a notification in the **What's new** panel.

Keep the following in mind:

- Before you update the solution in the Power Platform admin center, make sure that the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps have been updated to the latest version from the [!include[cc-microsoft](../includes/cc-microsoft.md)] Store.

- Updates to the solution must be done when the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps are not in use.  

> [!IMPORTANT]
> If you're currently using the public preview version of [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)], to get the October 2019 release, you'll need to search for the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution, and then select **Install** instead of **Upgrade**. This installs the general availability (GA) version of the solution and removes the public preview solution. For more information, see [Transition from public preview to GA](public-preview-transition.md).

To upgrade the solution:

1. Go to the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments) and sign in with the user credentials that have admin permissions for [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. 

2. To select the environment, select the check mark, select the **More environment actions** (three dots) button, and then select **Manage Solutions**. 

   ![Manage solutions](media/manage-solutions.PNG "Manage solutions")

3. Select **[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]** in the list of solutions, and then select **Upgrade**.
 
   ![Upgrade button](media/upgrade.PNG "Upgrade button")   
  
4. Review the Terms of service, and then select **Accept** if you're ready to start the upgrade. 

   The status of the solution changes to **Installation pending,** and then changes to **Installed** when the upgrade is complete. 
   
## Troubleshooting: Manually update the schema for the April 28, 2020 release

As a part of the April 28, 2020 release, all your guides should automatically be converted from schema v3 to v4 as a part of the Dynamics 365 Guides solution update. Schema v4 allows Dynamics 365 Guides content to be stored in entities instead of inside a single JavaScript Object Notation (JSON) file so that you can take advantage of the Common Data Service Web API and Microsoft Power Platform functionality using Dynamics 365 Guides content.

In rare cases, the conversion of a guide from schema v3 to v4 may be unsuccessful, due to reasons including, but not limited to:

- A guide was being authored in the PC or HoloLens app when the solution was being updated.

- The JSON file has been edited in a way that was not supported (for example, the guide doesn’t have a task, or too many 3D parts have been added to the Step Editor bin).

If a guide wasn’t converted successfully, authors or operators will see this error message when they try to open it: “Guide cannot be opened”. 

![Guide cannot be opened message](media/guide-not-opened.PNG "Guide cannot be opened message")

### Manually update a guide from schema v3 to v4

To resolve this issue, we suggest reviewing and fixing the JSON file before doing a schema update. To update the JSON file, you’ll download the existing file locally to make any changes, delete the JSON file associated with the guide, and then upload the file you modified. 

>[!NOTE]
> You must be an administrator to modify the JSON file.

#### Review and modify the JSON file

1.	In the PC app, sign in to the instance that includes the problem guide.

2.	Select the **Analyze** tab, select **Copy** to copy the **Instance URL**, and then paste the URL into a web browser.

   ![Copy the Instance URL](media/copy-instance-url.png "Copy the Instance URL")
   
3. Sign in, and then select the **Guides** model-driven app.  

   ![Guides app](media/guides-model-driven-app.png "Guides app")
   
4. Select the guide where the problem occurs.

   ![Select the guide](media/select-problem-guide.png "Select the guide")

>[!NOTE]
>If the JSON file has not been previously edited, you can go directly to [updating the schema](ADD URL HERE!!!).

5. Under **Note modified by MOD Administrator**, select the JSON file to download, and then open the file in any code editor to make any required changes. 

   ![Download JSON file](media/download-JSON-file.PNG "Download JSON file")
   
6. To remove the existing JSON file, hover over the **Note** button, select the **Edit** button, and then select the **X**.  

   ![Remove JSON file](media/remove-JSON-file.PNG "Remove JSON file")
   
7.	Upload the JSON file you modified by selecting the **Attach** button.

   ![Upload JSON file](media/upload-JSON-file.PNG "Upload JSON file")
   
8. Select **Save**.

#### Manually update the schema

- At the top of the screen, select **Flow**, and then select **Update guide schema**.

## See also
 
For more information about upgrading a [!include[pn-dyn-365](../includes/pn-dyn-365.md)] solution, [see Install, update, or remove a preferred solution](https://docs.microsoft.com/dynamics365/customer-engagement/admin/install-remove-preferred-solution).
