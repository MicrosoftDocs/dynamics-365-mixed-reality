# About the Author and Operator roles in Dynamics 365 Guides

If you're a Microsoft Dynamics 365 Guides admin, you can assign an Author or Operator role to users to limit what they can do in the apps. The Restricted Author and 
Restricted Operator roles provide an extra layer of control by limiting access to guides. Users who are assigned the Restricted Author and Restricted Operator roles 
**do not** inherit access to any guides or guide content (3D models, images, or videos) created in the environments that they are permitted to access. 

The following table describes the privileges that each role grants.

| Role | Description |
|---|---|
| Author | Use the PC app and HoloLens app to create, edit, and operate guides. Users who have the Author role can also rename and deactivate existing guides. |
| Operator | Use the HoloLens app to view and operate a guide. Users who have the Operator role can also save time by skipping the **Select Mode** dialog box when they open a guide. |
|Restricted Author| Use the PC app and HoloLens app to create, edit, and operate guides or use guides content that:<br><br>- The user created<br>- Were explicitly shared with them or shared with an owner team they are a member of<br>- Were assigned to the user or assigned to an owner team that the user is a member of|
|Restricted Operator|  Use the HoloLens app to view and operate a guide or access guides content that: <br><br>- The user created<br>- Were explicitly shared with them or shared with an owner team they are a member of<br>- Were assigned to the user or assigned to an owner team that the user is a member of |

For more information on using the Restricted Author and Restricted Operator roles in access teams, see 
[Share guides or guide content in Dynamics 365 Guides to expand access](admin-access-teams.md#assign-the-restricted-security-role).

> [!IMPORTANT]
> If you followed the instructions in the [Try or buy, and deploy Dynamics 365 Guides](setup-step-one.md) topic when you set up Dynamics 365 Guides, any users that you added were 
> automatically assigned the **Author** role. You must explicitly assign the **Operator** role to specific users if you don't want them to have **Author** role privileges.

## See also

[Assign a role to an individual user](assign-role.md)<br>
[Assign a role through Azure Active Directory groups](admin-assign-role-groups.md)<br>
[Restrict access to an environment by using security groups](admin-security.md)<br>
[Assign or share a guide by changing ownership](admin-access-assign.md)<br>
[Assign or share a guide through an access team](admin-access-teams.md)
