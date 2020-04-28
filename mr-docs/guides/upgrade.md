---
author: Mamaylya
description: Learn how to upgrade the Microsoft Dynamics 365 Guides solution when a new release requires an update.
ms.author: mamaylya
ms.date: 04/28/2020
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

## Troubleshooting: You receive a "Guide cannot be opened" error message

As a part of the update to the Dynamics 365 Guides solution that is released on April 28, 2020, all your guides should automatically be converted from schema v3 to v4. Schema v4 enables Dynamics 365 Guides content to be stored in entities instead of inside a single JavaScript Object Notation (JSON) file. Therefore, you can take advantage of the Common Data Service Web application programming interface (API) and Microsoft Power Platform functionality by using Dynamics 365 Guides content.

In rare cases, the conversion of a guide from schema v3 to v4 might be unsuccessful, for reasons that include but aren't limited to the following:

- A guide was being authored in the PC or HoloLens app when the solution was updated.

- The JSON file has been edited in a way that isn't supported. (For example, the guide doesn't have a task, or too many 3D parts have been programmatically added to the **Step Editor** bin.)

If a guide wasn't successfully converted, authors or operators will receive the following error message when they try to open it: "Guide cannot be opened."

![Guide cannot be opened message](media/guide-not-opened.JPG "Guide cannot be opened message")

### Manually update a guide from schema v3 to v4

To fix this issue, we recommend that you first try to upgrade the guide schema from v3 to v4. If that approach doesn't fix the issue, review and fix the JSON file (as described later in this topic) before you retry a schema update. 

> [!NOTE]
> You can't manually update the schema for guides that have already been updated to schema v4. The schema version number appears on the **General** tab when you open a guide in the Guides model-driven app. 

#### Update the schema

1. In the PC app, sign in to the instance that includes the guide where the issue occurs.

2. On the **Analyze** tab, select **Copy** to copy the **Instance URL** value, and then paste the value into the address bar of a web browser.

    ![Copy the Instance URL value](media/copy-instance-url.jpg "Copy the Instance URL value")

3. Sign in, and then select the **Guides** model-driven app.

    ![Guides app](media/guides-model-driven-app.jpg "Guides app")

4. Select the guide where the issue occurs.

    ![Select the guide](media/select-problem-guide.jpg "Select the guide")

5. At the top of the page, select **Flow**, and then select **Upgrade guide schema**.

    ![Update guide schema command](media/upgrade-guide-schema.jpg "Update guide schema command")

> [!NOTE]
> If the issue isn't fixed when you update the guide schema, the guide's JSON file has probably been edited in a way that isn't supported. (For example, too many 3D objects have been programmatically added to the **Step Editor** bin.) Follow the steps in the next procedure to review and replace the JSON file.

#### Review and replace the JSON file

To update the JSON file, you will download the existing file locally so that you can make any required changes, delete the JSON file that is associated with the guide, and then upload the file that you modified.

1. Select the guide where the issue occurs.

    ![Select the guide](media/select-problem-guide.jpg "Select the guide")

2. Under **Note modified by MOD Administrator**, select the JSON file to download. Then open the file in any code editor, and make any required changes. 

    ![Select the JSON file to download](media/download-JSON-file.jpg "Select the JSON file to download")

6. To remove the existing JSON file, hover over the **Note** button, select the **Edit** button, and then select the **X** button.

    ![Remove a JSON file](media/remove-JSON-file.jpg "Remove a JSON file")

7.	To upload the JSON file that you modified, select the **Attach** button.

    ![Upload a JSON file](media/upload-JSON-file.jpg "Upload a JSON file")

8. Select **Save**.

9. Manually trigger a guide schema update as described in the previous procedure.

## See also
 
For more information about upgrading a [!include[pn-dyn-365](../includes/pn-dyn-365.md)] solution, [see Install, update, or remove a preferred solution](https://docs.microsoft.com/dynamics365/customer-engagement/admin/install-remove-preferred-solution).
