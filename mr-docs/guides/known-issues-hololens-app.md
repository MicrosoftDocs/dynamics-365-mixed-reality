

# Known Issues with the Dynamics 365 Guides HoloLens app

## I can't sign in

To sign in, you must use the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365](../includes/pn-dyn-365.md)] sign-in credentials for your organization. It will resemble: johndoe@contoso.onmicrosoft.com. You can't use a [!include[cc-microsoft](../includes/cc-microsoft.md)] account (used for Outlook.com, [!include[cc-microsoft](../includes/cc-microsoft.md)] Store, and so on) or your corporate credentials to sign in. 

If you see any of the following errors, contact your IT admin, or see the self-service documentation at <https://aka.ms/guidesdocs>:

- [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] isn't set up correctly, or you might not have permission to access it. Contact your admin, or see the [self-service documentation](https://aka.ms/guidesdocs).

- Your client app version doesn't support your [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution version. Update your client app, contact your admin, or see the [self-service documentation](https://aka.ms/guidesdocs).

- You don't have a license to use [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. Contact your admin.

## Staying on the account picker more than 25 seconds during HoloLens sign-in will make it unresponsive

When you get to the screen where you can select between different saved accounts on [!include[pn-hololens](../includes/pn-hololens.md)], choose an option within 25 seconds. After 25 seconds it will become unresponsive, and you will need to restart the app. This bug has been fixed on RS5, but still exists on RS4 if you have that installed.

## Circular code anchor method requires user's consent to use the camera

When the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] application on [!include[pn-hololens](../includes/pn-hololens.md)] is launched for the first time, the app will ask the user to provide consent to use the camera. If you plan to use circular code anchors in your guides, you will need to say **Yes** to this prompt. This is required for every device you use the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] application on. If this consent was not provided previously, you can go to the **Settings** menu on the [!include[pn-hololens](../includes/pn-hololens.md)] (operating system) and provide consent to the app. 

## "Create account" link when signing in with a new account doesn't work

When signing in with a brand new account on the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps, there is a link to create a new account:

![Sign-in screen](media/sign-in-screen.PNG "Sign-in screen") 
  
Please do not use this link to create an account–it doesn't work.

## I don't see any guides in the Guides list

If you don't see any guides, either your internet connection is unstable, or you might have signed into an instance that doesn't have any guides. First, check your internet connection. If you're connected, try signing in again, but this time make sure you sign into the instance that has the guides you were looking for. If you still don't see any guides, contact your administrator.

## I can't find the guide I created

Look for newly created guides in the **All** tab in the list of guides. The **Recents** list shows only those guides that have been previously opened on the device and does not include any guide recently created in the PC authoring application. 

## The profile picture shown in the app is incorrect 

Make sure you're signed in. To do this, select the profile picture, and then sign out and sign back in with your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] credentials. Your profile picture should appear correctly.

Signing in with the right credentials ensures that your work progress is correctly tracked in [!include[pn-dyn-365](../includes/pn-dyn-365.md)].

## The video preview on a step is blurry

The [!include[pn-hololens](../includes/pn-hololens.md)] app converts and resizes videos when they're uploaded to ensure optimal performance on [!include[pn-hololens](../includes/pn-hololens.md)]. If your video was recorded at a very high resolution, or if it's extremely large, the transcoding process might have degraded its quality. Re-record and upload a new video, keeping length and resolution in mind.

As a best practice, video clips should not be too long (**maximum of 2 minutes**). This helps operators focus on one meaningful task at a time and keeps them from getting overwhelmed. 

## Deleting an asset from a step (from the bin) in the PC app will remove all previously placed instances on HoloLens

If you're editing an existing guide, where an asset was placed in a bin in the PC app, and then instances of that asset were placed in the world on [!include[pn-hololens](../includes/pn-hololens.md)], note that deleting the asset from the bin removes all of the placed assets in space. Adding the asset again will not restore the placed instances. To restore, press the **Undo** button in the PC app to revert the change.

## Uploading glTF files with dependencies across different folders might result in upload errors

Some glTF files may have dependencies in other folders that the app may not have permissions to when uploading. This might result in errors or broken 3D models in the gallery. Please make sure you either have permissions to all dependencies, or that you have all of them in the same folder when uploading glTF models. 

## The see-through style, when applied to a 3D model might show gray areas instead of rendering textures properly

There are some problems with rendering the "see through" style on some 3D models. Some surfaces on these models will look gray. Please use another style if you see this problem, or contact customer service if this is a must-have and you need help with it.

## When moving a 3D model during authoring on HoloLens, the movement of the model may seem slow

To allow authors to place 3D models carefully and precisely, the default movement is set to be slow. To indicate this, the manipulation sphere around the model will be blue. You can move your hand faster, or wiggle the model a bit to switch it to move faster. 

## I have an issue that isn't listed in these troubleshooting steps
Please contact customer service: [https://docs.microsoft.com/dynamics365/get-started/support/](https://docs.microsoft.com/dynamics365/get-started/support/). This page can also be found by signing in to your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] account and selecting the **Support** link.

