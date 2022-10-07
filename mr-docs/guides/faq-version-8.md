
# FAQ: Dynamics 365 Guides 8.0

This FAQ addresses questions related to Dynamics 365 Guides 8.0, which includes many of the Microsoft Teams collaboration/calling features currently available in Dynamics 365 Remote Assist.  

## What licenses do I need to access collaboration functionality in Dynamics 365 Guides?

You need a Dynamics 365 Guides license and a Microsoft Teams license.

## Can I collaborate with Teams users in the same way as in Dynamics 365 Remote Assist?

Yes.

## Does Dynamics 365 Guides 8.0 store calls data the same way as Dynamics 365 Remote Assist?

Yes, it stores data in the same table and columns. In addition, Dynamics 365 Guides provides many improvements to the reliability of data collection, especially in environments where internet connections are inconsistent. 

## Does Dynamics 365 Guides 8.0 provide a Calls dashboard like Dynamics 365 Remote Assist to analyse call data?

No, Dynamics 365 Guides doesn't have a Calls dashboard but it provides a table-like view with all of the same information. And since Dynamics 365 Guides 8.0 sends call usage events to the same PhoneCall table (the default table in Microsoft Dataverse) that Dynamics 365 Remote Assist uses, calls made from Dynamics 365 Guides are displayed in the Dynamics 365 Remote Assist Calls dashboard if both apps are installed in the same environment.

## Do I need to update privileges for custom security roles to write calls data to the PhoneCall table?

???What's the answer here???

## Can I share a deep link to a guide through a HoloLens chat?

Yes, Teams desktop users can share a link to a guide directly in the chat. HoloLens users can open a guide directly by selecting the link. 

## Are there any new permissions that need to be configured?

There are two new permissions: 

- The Location permission (optional) can be enabled if you want to store location information.

- The Background spatial perception (movement) permission is required if you want to use the new annotations capabilities.

## What functionality is not supported in the Dynamics 365 Guides 8.0 October release but will be added in upcoming releases?

- Support for incoming calls on HoloLens

- Support for restricted access

- Take a photo during a call

Appendix (internal use)

## What do I need to do to ensure that call data is displayed correctly?

Summary: The first iteration of this project is to instrument the HL client app with the necessary telemetry to be able to collect data for customers to analyze. We will be adding a page in the MDA with a table that will have similar information to the dashboard Remote Assist provides today.

Background: Remote Assist sends call usage events into PhoneCall entity. This is a default entity in the dataverse which is customized in RA solution to have a few more fields.

Assumptions:

· It is assumed Guides solution is installed in the dataverse instance.

· It is assumed that a customer would be able to see Calls Data from Guides on the existing RA Dashboard if both solutions are installed in the same environment.

To log Calls data from Guides we will be using the same PhoneCall entity with similar customizations made in RA solution.

We will update the existing security roles to give read-write privileges to Phone Call table so that Guides client can safely write the data for authors and operators.

o Dynamics 365 Restricted Guides Author

o Dynamics 365 Restricted Guides Operator

o Dynamics 365Guides Author

o Dynamics 365 Guides Operator

Built in System admin role can be used if a user wants full access to Calls data.

## If I'm using both Dynamics 365 Guides and Dynamics 365 Remote Assist for a period of time, will I be able to filter calls data by app?

Yes, you can filter by subject in the Guides model-driven app. The subject value for Dynamics 365 Remote Assist calls is "Dynamics 365 Remote Assist Call".

## How do I configure roles for users who need/use calling and annotations functionality only and who are mostly using Dynamics 365 Remote Assist currently?

There’s no built-in way to limit access in Dynamics 365 Guides to just calling functionality.

To transition a specific user to Dynamics 365 Guides 8.0, you need to do two things:

1. Assign the Dynamics 365 Guides license to that user.

2. Assign one of Dynamics 365 Guides roles.

The user will be able to sign into Dynamics 365 Guides after doing these two steps.



Add - What happens if user just wants to use calling functionality? (add a matrix)

Add - What happens if user wants to use both calling and guides functionality?

## Does Guides 8.0 support HoloLens kiosk mode? 

The 8.0 release does not support kiosk mode. This will be added in an upcoming release.

## Can I send a deep link to a guide from a meeting in Dynamics 365 Guides 8.0?

The 8.0 release does not support sending a deep link from a meeting. This will be added in an upcoming release.

## Which Dynamics 365 Remote Assist features are included in Dynamics 365 Guides 8.0?

|Feature|Dynamics 365 Remote Assist|Dynamics 365 Guides 8.0|
|-------------------------------------|-------------------------------------|-------------------------------------|
|Annotations (ability for both the remote expert and HoloLens user to annotate the HoloLens user's environment)| Yes| Yes|
|Join and schedule a meeting| Significantly improved| Oct, Guides 8.0|
|Group calling| Yes| Yes|
|Call recording| Yes| Yes|
|Spotlighting| New| Yes|
|Teams policy support| Yes| Yes|
|Automatic HoloLens temperature management| New| Yes|
|Chat| Yes|Yes, and improved in Dynamics 365 Guides 8.0|
|Screen sharing| Yes| Yes|
|File access| Yes| Yes|
|Call data storage| Yes| Yes|
