---
author: Mamaylya
description: Upgrade the Dynamics 365 Guides (Preview) solution 
ms.author: mamaylya
ms.date: 10/01/2019
ms.service: crm-online
ms.topic: article
title: Upgrade the Dynamics 365 Guides (Preview) solution
ms.reviewer: v-brycho
---

# Upgrade the Dynamics 365 Guides solution (for admins)

This topic is for [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365](../includes/pn-dyn-365.md)] administrators. Some releases of [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] require an update to the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution. When an update is required, the user will see a notification in the **What's new** panel.

> [!IMPORTANT]
> Keep the following in mind:<br><br>- Before updating the solution in the [!include[pn-dyn-365](../includes/pn-dyn-365.md)] Administration Center, make sure that the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps have been updated to the latest version from the [!include[cc-microsoft](../includes/cc-microsoft.md)] Store.<br><br>- Updates to the solution must be done when the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps are not in use.  

To upgrade the solution:

1. Go to the Dynamics 365 Administration Center and sign in with the user credentials that have admin permissions for [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. 

   > [!NOTE]
   > To go to the Dynamics 365 Administration Center, go to the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home), and then select **Admin centers** > **Dynamics 365** as shown below.
   
   ![Microsoft Admin Center](media/microsoft-admin-center.PNG "Microsoft Admin Center") 

2. Select the **Instances** tab, and then choose an instance that has the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution installed.

3. Select the small edit button next to **Solutions** to see the list of solutions. 
 
   ![Solutions button](media/solutions.PNG "Solutions button")
 
4. In the list of solutions, select **[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]**, and then select **Upgrade**.  
 
   ![Upgrade button](media/upgrade.PNG "Upgrade button")
   
   > [!IMPORTANT]
   > If you're currently using the public preview version of [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)], to get the October 2019 release, you'll need to search for the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution, and then select **Install** instead of **Upgrade**. This will install the GA version of the solution and remove the public preview solution.
   
5. Review the Terms of service, and then select **Accept** if you're ready to start the upgrade. 

   The status of the solution changes to **Installation pending,** and then changes to **Installed** when the upgrade is complete. 
 
For more information on upgrading a [!include[pn-dyn-365](../includes/pn-dyn-365.md)] solution, [see Install, update, or remove a preferred solution](https://docs.microsoft.com/dynamics365/customer-engagement/admin/install-remove-preferred-solution).
