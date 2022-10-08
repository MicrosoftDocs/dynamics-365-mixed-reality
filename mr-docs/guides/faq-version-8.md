
# FAQ: Dynamics 365 Guides 8.0 and Dynamics 365 Remote Assist

This FAQ addresses questions related to Dynamics 365 Guides 8.0. The Dynamics 365 Guides release includes many of the Microsoft Teams collaboration/calling features that are also available in Dynamics 365 Remote Assist.  

## Feature comparison: Dynamics 365 Remote Assist and Dynamics 365 Guides 8.0 and Dynamics 365 Remote Assist

|Feature|Dynamics 365 Remote Assist|Dynamics 365 Guides 8.0|
|-------------------------------------|-------------------------------------|-------------------------------------|
|Annotations (ability for both the remote expert and HoloLens user to annotate the HoloLens user's environment)| Yes| Yes|
|Join and schedule a meeting| Yes| Yes (significantly improved in Dynamics 365 Guides 8.0)|
|Group calling| Yes| Yes|
|Incoming calls|Yes|No. This feature will be adding in an upcoming Dynamics 365 Guides release.|
|Call recording| Yes| Yes|
|Chat| Yes|Yes (improved in Dynamics 365 Guides 8.0)|
|Screen sharing| Yes| Yes (improved in Dynamics 365 Guides 8.0)|
|Snaphots (for poor connectivity situations)|Yes|No. This feature will be adding in an upcoming Dynamics 365 Guides release.|
|Spotlighting| Yes| Yes|
|File access| Yes| Yes|
|Restricted access (calling, contacts, OneDrive files and ability to sign out of the HoloLens app)|Yes|No. This feature will be adding in an upcoming Dynamics 365 Guides release.|
|Call data storage/display| Yes| Yes (Dynamics 365 Guides does not provide a built-in Calls dashboard, however)|
|Teams policy support| Yes| Yes|
|HoloLens temperature management| Yes| Yes|

## What licenses do I need to access the new collaboration features in Dynamics 365 Guides?

You need a Dynamics 365 Guides license and a Microsoft Teams license. [Learn more about licensing requirements](requirements.md)

## Can I collaborate with Teams users in the same way as I do in Dynamics 365 Remote Assist?

Yes.

## Does Dynamics 365 Guides 8.0 store call data the same way as Dynamics 365 Remote Assist?

Yes, it stores data in the same table and columns. In addition, Dynamics 365 Guides provides many improvements to the reliability of data collection, especially in environments where internet connections are spotty. [Learn more about viewing and accessing call data in Dynamics 365 Guides](call-logging.md)

## Does Dynamics 365 Guides 8.0 provide a Calls dashboard like Dynamics 365 Remote Assist to analyse call data?

No, Dynamics 365 Guides 8.0 doesn't have a Calls dashboard but it provides a table-like view with all of the same information. And since Dynamics 365 Guides 8.0 sends call usage events to the same PhoneCall table that Dynamics 365 Remote Assist uses (which is the default table in Microsoft Dataverse), calls made from Dynamics 365 Guides are displayed in the Dynamics 365 Remote Assist Calls dashboard if both apps are installed in the same environment. [Learn more about viewing and accessing call data in Dynamics 365 Guides](call-logging.md)

## Do I need to update privileges for custom security roles?

Yes. If you have created custom security roles, you must update those roles to provide privileges to the Activity table (PhoneCall table). **Users won't be able to sign in to either app if you don't update custom security roles.** Users must have the following seven privileges to be able to sign in:

- prvAppendActivity
- prvAppendToActivity
- prvAssignActivity
- prvCreateActivity
- prvReadActivity
- prvShareActivity
- prvWriteActivity

![Screenshot of required privileges for Activity table.](media/admin-security-roles-activity-table.JPG "Screenshot of required privileges for Activity table")

> [!NOTE]
> The Delete privilege is not required. 

## Can I share a deep link to a guide through a HoloLens chat?

Yes, Teams desktop users can share a link to a guide directly in chat. HoloLens users can open a guide directly (or even a particular step in a specific guide) by selecting the link. [Learn more about creating a deep link](pc-app-copy-link-guide-step.md)

## Do I need to configure any new permissions?

There are two new permissions: 

- The Location permission (optional) can be enabled if you want to store location information in the PhoneCall table.

- The Background spatial perception (movement) permission is required if you want to use the new annotations capabilities.

[Learn more about permissions required for the HoloLens app](hololens-permissions.md)

## If I'm using both Dynamics 365 Guides and Dynamics 365 Remote Assist for a period of time, will I be able to filter call data by app?

Yes, you can filter by subject in the Guides model-driven app. The subject value for Dynamics 365 Remote Assist calls is "Dynamics 365 Remote Assist Call".

## How do I configure roles for users who need to use calling and annotations functionality only and who are mostly using Dynamics 365 Remote Assist currently?

There’s no built-in way to limit access in Dynamics 365 Guides to just calling functionality. 

To transition a specific user to Dynamics 365 Guides 8.0, you need to do two things:

1. Assign the Dynamics 365 Guides license to that user.

2. Assign one of Dynamics 365 Guides roles.

The user will be able to sign into Dynamics 365 Guides after doing these two steps.

[Learn more about assigning security roles](assign-role.md)


