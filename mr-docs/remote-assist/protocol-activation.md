---
author: ReneeW-CPub
description: Launch Dynamics 365 Remote Assist from another app (protocol activation)
ms.author: renwe
ms.date: 09/21/2018
ms.service: crm-online
ms.topic: article
title: Launch Dynamics 365 Remote Assist from another app
---

# Launch Dynamics 365 Remote Assist from another app (protocol activation)

You can embed code in your HoloLens application to switch to Microsoft Dynamics
365 Remote Assist and begin a call using a Uniform Resource Identifier (URI).
For example, let’s say you’re creating a helicopter maintenance app. You can add
a button that a maintenance engineer can use to call an expert if they get
stuck. The button will launch Remote Assist and call the designated expert.

Remote Assist supports two methods for protocol activation: 

-   “ms-voip-video” is for video-enabled calling.

-   “ms-voip-call” is for audio-only calling.

Both methods use the same argument schema, which accepts a “contactID” field.
The URI would look something like this:

`
ms-voip-video:?contactids=\<contactID\>
`

The contact ID is the user’s Azure Active Directory (Azure AD) objectID.

## Code sample

You’ll need to embed the code in your HoloLens app. The following code sample is
written in C++, but can be easily adapted to another language.

```
Platform::String\^ id = objectId-\>Text;
auto uri = ref new Windows::Foundation::Uri("ms-voip-video:?contactids=" + id);
resultText-\>Text = uri-\>AbsoluteUri; 

concurrency::task\<bool\> launchUriOperation(Windows::System::Launcher::LaunchUriAsync(uri));
launchUriOperation.then([this](bool success)   
{         
    if (success)         
    {             
        // URI launched  
        resultText-\>Text += " (URI Launched)"; 
    } 
    else         
    {             
        // URI launch failed             
        resultText-\>Text += " (FAILED)";
    }     
});  
```

To place an audio-only call instead of video, use URI: “ms-voip-call:?contactids=”

## Place a call to test your code

1.  Run your app on the HoloLens.

2.  Initiate the call from your app.

3.  The HoloLens will appear to close the app, open Remote Assist if it isn’t
    already open, and sign in.

4.  After the contacts panel is loaded, Remote Assist will place a call to the
    specified contact.

### See also

For more details on launching an app with a URI, see [Launch an app with a URI](<https://docs.microsoft.com/en-us/windows/uwp/launch-resume/launch-app-with-uri>).
