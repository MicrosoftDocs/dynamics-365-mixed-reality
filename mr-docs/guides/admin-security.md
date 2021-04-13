---
author: Mamaylya
description: Learn how to use security groups to control which users can access which environments in Microsoft Dynamics 365 Guides.
ms.author: mamaylya
ms.date: 04/14/2021
ms.service: crm-online
ms.topic: article
title: Restrict access to an environment in Dynamics 365 Guides by using security groups
ms.reviewer: v-bholmes
---

# Restrict access to an environment in Dynamics 365 Guides by using security groups

If your company has multiple Microsoft Dynamics 365 Guides environments, you can use security groups to control which users can access each environment. A security group restricts access to the environment to people in the security group. If a Microsoft Dataverse environment does not have an associated security group, all users with a Dataverse license (Dynamics 365 Guides, Power Automate, Power Apps, and so on) will be created as users and enabled in the environment. 

Each environment can have just one security group. For example, you could create three security groups to control access to the following environments.

| Environment                    | Security group  | Purpose |
|--------------------------------|-----------------|---------|
| Coho Manufacturing Sales       | Sales\_SG       | Provide access to the organization that creates sales opportunities, handles quotations, and closes deals. |
| Coho Manufacturing Maintenance | Maintenance\_SG | Provide access to the organization that does service and machinery maintenance. |
| Coho Manufacturing Dev         | Developer\_SG   | Provide access to the sandbox environment that is used for development and testing. |

[Learn more about controlling user access to environments with security groups](https://docs.microsoft.com/power-platform/admin/control-user-access). 

> [!NOTE]
> Environments are sometimes referred to as "organizations" or "instances." Each of these terms refers to the same concept. 

## Create a user and assign a license

Use this procedure if you haven't already created users and assigned licenses. If you've already completed those tasks, you can skip ahead to the next procedure.

1. Sign in to the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home#/homepage).

2. In the left pane, select **Users** \> **Active users**, and then select **Add a user** to open the **Add user** wizard.

    ![Add a user](media/add-user-3.PNG "Add a user")

3. On the **Set up the basics** page, enter the user's first name, last name, display name, and user name.

    ![Set up the basics page with user details](media/set-up-basics.PNG "Set up the basics page with user details")

4. Under **Password settings**, follow these steps:

    1. Select whether the password should be automatically generated, or whether you want to create it yourself.

    2. Select whether the user will be required to change the password the first time that he or she signs in.

    3. Select whether you want to send the password by email.

    When you've finished, select **Next**.

5. On the **Assign product licenses** page, select a location, select the **Dynamics 365 Guides** check box if it isn't already selected, and then select **Next**.

    ![Dynamics 365 Guides check box](media/guides-check-box.PNG "Dynamics 365 Guides check box")

6. On the **Optional settings** page, add any roles or profile information that you want to add, and then select **Next**.

7. On the last page, review the settings, select **Finish adding**, and then select **Close** to close the wizard.

    > [!TIP]
    > You can also [add several users at the same time](https://docs.microsoft.com/office365/enterprise/add-several-users-at-the-same-time?redirectSourcePath=%252farticle%252fAdd-several-users-at-the-same-time-to-Office-365-Admin-Help-1f5767ed-e717-4f24-969c-6ea9d412ca88).

## Create a security group and add members (users) to it

1. In the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home#/homepage), in the left pane, select **Groups** \> **Groups**, and then select **Add a group** to open the **Add group** wizard.

    ![Add a group](media/add-group-command.PNG "Add a group")

2. On the **Choose a group type** page, select **Security**, and then select **Next**.

    ![Choose a group type page](media/choose-group-type.PNG "Choose a group type page")

3. On the **Set up the basics** page, enter a name and description for the group, and then select **Next**.

    ![Set up the basics page with group name](media/set-up-basics-2.PNG "Set up the basics page with group name")

4. On the **Review and finish adding group** page, review your changes, select **Create group**, and then, on the next page, select **Close** to close the wizard.

    ![Review and finish adding group page](media/review-group.PNG "Review and finish adding group page")

5. On the **Groups** page, select **Refresh** if you don't see your new group.

6. Select the group that you created, and then, in the pane that appears on the right, select the **Members** tab.

    ![Members tab](media/members-tab.PNG "Members tab")

7. On the **Members** tab, select **View all and manage owners**.

    ![View all and manage members button](media/view-members.PNG "View all and manage members button")

8. In the dialog box that appears, select **Add members**.

    ![Add members button](media/add-members-2.PNG "Add members button")

9. Select the users to add to the security group, select **Save**, and then select **Close** two times to return to the **Groups** page.

> [!NOTE]
> To remove users from a security group, repeat this procedure, but select the **X** next to any member that you want to remove.
>
> ![Remove a member](media/remove-members-2.PNG "Remove a member")

## Associate a security group with an environment

1. In the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home#/homepage), in the left pane, select **All admin centers**, and then select **Power Apps**.

    ![Open the Dynamics 365 admin center](media/all-admin-centers.PNG "Open the Dynamics 365 admin center")

2. In the **Environments** page, select the environment to edit by clicking the environment name.  

3. In the Power Platform admin center, in the **Details** section, select **Edit**.

    ![Edit button in Power Platform admin center](media/security-groups-edit-details.PNG "Edit button in Power Platform admin center")

4. In the **Edit details** pane, select the pencil button, select the security group, and then select **Save**.

    ![Pencil button on Edit details tab](media/security-groups-select-group.PNG "Pencil button on Edit details tab")

## Additional information about security groups

Note the following points about security groups:

- When users are added to a security group, they are added to the environment.

- When users are removed from a security group, they are disabled in the environment.

- When a security group is associated with an existing environment that has users, any users in that environment who aren't members of the security group will be disabled.

- If no security group is associated with an environment, all users who have a license will be created as users and enabled in that environment.

- If a security group is associated with an environment, only users who have a license and who are members of the security group will be created as users in that environment.

- When you remove a security group that is associated with an environment, either by editing the environment and removing the security group, or by deleting the security group, licensed users who were members of that security group will have the same access to model-driven apps in Dynamics 365.

- When you assign a security group to an environment, the environment appears on the **Instances** tab in the Dynamics 365 admin center only for users who are members of the group.

- If you don't assign a security group to an environment, the environment appears on the **Instances** tab in the Dynamics 365 admin center even for users who haven't been assigned a security role in that environment.

- Nested security groups aren't supported.

> [!NOTE]
> All licensed users, regardless of whether they are members of security groups, must be assigned security roles to access model-driven apps in Dynamics 365. You assign security roles in the web application. Users can't access environments until they are assigned at least one security role for that environment. For more information, see [Grant users access](https://docs.microsoft.com/power-platform/admin/grant-users-access).

## See also

[Add several users at the same time](https://docs.microsoft.com/office365/enterprise/add-several-users-at-the-same-time?redirectSourcePath=%252farticle%252fAdd-several-users-at-the-same-time-to-Office-365-Admin-Help-1f5767ed-e717-4f24-969c-6ea9d412ca88)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
