---
author: Mamaylya
description: Add additional user accounts to a Dynamics 365 Guides license
ms.author: mamaylya
ms.date: 01/28/2020
ms.service: crm-online
ms.topic: article
title: Add additional user accounts to Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Add additional user accounts to Dynamics 365 Guides

If you want to add additional users to [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)], you need to assign the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] license to them in the Microsoft 365 admin center, and then configure the roles they will have access to (Author, Operator, or administrator) in the Power Platform admin center.

## Add a user account

1. Go to the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home).

2. In the left pane, select **Users**, and then select **Active users**. 

3. On the **Active users** page, select **Add a user**.

   ![Add a user command](media/add-additional-user.png "Add a user command") 

4. On the **Set up the basics** page, fill in the information for the new user. Select **Next** when you're done.

   ![Set up the basics page](media/setup-basics.png "Set up the basics page")

   > [!NOTE]
   > By default, an auto-generated password will be generated for the user. The user is required to change the password the first time they sign in with this account. If you want to change the password to a permanent password instead of using the auto-generated password, select the **Let me create the password** option, and then clear the **Require this user to change their password when they first sign in** check box. 
 
5. Select the location for this user, and then under **Licenses**, select the **Dynamics 365 Guides** check box. 

    ![Dynamics 365 Guides check box](media/assign-license-user.png "Dynamics 365 Guides check box") 

     Select **Next** when you're done.
   
6. On the **Optional settings** page, leave the **User (no administrator access)** box selected unless this new user will be an administrator. In that case, select the **Global administrator** check box. 

   ![Optional settings page](media/user-optional-settings.png "Optional settings page") 
   
7. To fill out the new user's profile info, scroll down, and then expand **Profile info**. Select **Next** when you're done.
   
   ![Expanded Profile info](media/expanded-profile-info.png "Expanded Profile info")
   
8. Review the information on the last page. To make changes, select the **Edit** button below each section. Select **Finish Adding** when you're done.

   ![Review page with Edit buttons](media/review-page.png "Review page with Edit buttons")

8. If you selected **Auto-generate password** in step 4, make note of the password. The user will need this password to sign in.

   ![Auto-generated password](media/review-user-settings.png "Auto-generated password") 
   
9. Select **Close**.

After adding user accounts, the next step is to assign the **Author**, **Operator**, or **Admin** user roles for the solution. For more information, [Assign user roles](assign-role.md).

## What's next?

[Assign user roles](assign-role.md)
      

