

# Control user access to instances: security groups and licenses

If your company has multiple instances, you can use security groups to control which licensed users can be a member of a 
particular instance.

Consider the following example scenario:

Table 1
Instance
Security Group
Purpose
Coho Winery Sales
Sales_SG
Provide access to the organization that creates sales opportunities, handles quotes, and closes deals.
Coho Winery Marketing
Marketing_SG
Provide access to the organization that drives marketing efforts through marketing campaigns and advertising.
Coho Winery Service
Marketing_SG
Provide access to the organization that processes customer cases.
Coho Winery Dev
Developer_SG
Provide access to the Sandbox instance used for development and testing.

In this example, four security groups provide controlled access to a specific organization.

Note the following about security groups:

When users are added to the security group, they are added to the instance.

When users are removed from the group, they are disabled in the instance.

When a security group is associated with an existing instance with users, all users in the instance that are not members of the 
group will be disabled.

If an instance does not have an associated security group, all users with a license will be created as users and enabled in the 
instance.

If a security group is associated with an instance, only users with licenses that are members of the instance security group will 
be created as users in the instance.

When you remove a security group that is associated with a instance, either by editing the instance and removing the security 
group or by deleting the security group, licensed users who were members of the security group will have the same access to 
model-driven apps in Dynamics 365.

When you assign a security group to an instance, that instance will not show up in the Instances tab (instance picker) in the 
Dynamics 365 admin center for users not in the group.

If you do not assign a security group to an instance, the instance will show up in the Instances tab (instance picker) in the 
Dynamics 365 admin center even for those who have not been assigned a security role in that instance.
Nested security groups are not supported.
