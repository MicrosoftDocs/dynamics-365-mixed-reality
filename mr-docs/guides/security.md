

# Restrict access to an instance

If your company has multiple instances for Dynamics 365 Guides, you can use security groups to control which users can access which instances.

Consider the following example scenario:

|Instance|Security Group|Purpose|
|-------------------|----------------------|------------------------------------------------------------------------|
|Coho Winery Sales|Sales_SG|Provide access to the organization that creates sales opportunities, handles quotes, and closes deals.|
|Coho Winery Marketing|Marketing_SG|Provide access to the organization that drives marketing efforts through marketing campaigns and advertising.|
|Coho Winery Service|Marketing_SG|Provide access to the organization that processes customer cases.|
|Coho Winery Dev|Developer_SG|Provide access to the Sandbox instance used for development and testing.|

In this example, four security groups provide controlled access to a specific organization.

Note the following about security groups:

- When users are added to the security group, they are added to the instance.

- When users are removed from the group, they are disabled in the instance.

- When a security group is associated with an existing instance with users, all users in the instance that are not members of the 
group will be disabled.

- If an instance does not have an associated security group, all users with a license will be created as users and enabled in the 
instance.

- If a security group is associated with an instance, only users with licenses that are members of the instance security group will 
be created as users in the instance.

- When you remove a security group that is associated with a instance, either by editing the instance and removing the security 
group or by deleting the security group, licensed users who were members of the security group will have the same access to 
model-driven apps in Dynamics 365.

- When you assign a security group to an instance, that instance will not show up in the Instances tab (instance picker) in the 
Dynamics 365 admin center for users not in the group.

- If you do not assign a security group to an instance, the instance will show up in the Instances tab (instance picker) in the 
Dynamics 365 admin center even for those who have not been assigned a security role in that instance.
Nested security groups are not supported.

- Nested security groups are not supported.

>[!NOTE]
>All licensed users, whether or not they are members of the security groups, must be assigned security roles to access model-driven apps in Dynamics 365. You assign the security roles in the web application. Users can’t access instances until they are assigned at least one security role for that instance. More information: Grant users access.

## Create a security group and add members to the security group

1. Sign in to the Microsoft 365 admin center.

2. Click Groups > Groups.

3. Click + Add a group.

4. Change the type to Security group, add the group Name and Description. Click Add > Close.

5. Click the group you created, and then next to Members, click Edit.

6. Click + Add members. Select the users to add to the security group, and then click Save > Close several times to return to the Groups list.

7. To remove a user from the security group, select the security group, next to Members, click Edit. Click - Remove members, and then click X for each member you want to remove.

>[!NOTE]

If the users you want to add to the security group are not created, create the users and assign to them the licenses.<br>
To add multiple users, see: bulk add users to Office365 groups.

## Create a user and assign a license

- In the Microsoft 365 admin center, click Users > Active users > + Add a user. Enter the user information, select licenses, and then click Add.

More information: Add users individually to Office 365 - Admin Help

## Associate a security group with an instance

1. In the Microsoft 365 admin center, click Admin centers > Dynamics 365.

2. Click the Instances tab, select an instance, and then click Edit.

3. In security settings, search for a specific security group, and then click Next > Save.

>[!TIP]
>To force an immediate synchronization between the Office 365 admin portal and model-driven apps in Dynamics 365, do the following:<br>
- Sign out of model-driven apps in Dynamics 365 and the Office 365 admin portal.<br>
- Close all open browsers used for model-driven apps in Dynamics 365 and the Office 365 admin portal.<br>
- Sign back in to model-driven apps in Dynamics 365 and the Office 365 admin portal.

## See also

