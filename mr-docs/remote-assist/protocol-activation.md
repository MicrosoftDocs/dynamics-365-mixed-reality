---
author: MatthewJonPaul
description: Launch Dynamics 365 Remote Assist from another app (protocol activation)
ms.author: mapau
ms.date: 09/21/2018
ms.service: crm-online
ms.topic: article
title: Launch Dynamics 365 Remote Assist from another app
ms.reviewer: v-brycho
---

# Launch Dynamics 365 Remote Assist from another app (protocol activation)

You can embed code in your [!include[pn-hololens](../includes/pn-hololens.md)] application to switch to [!include[cc-microsoft](../includes/cc-microsoft.md) [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] and begin a call using a Uniform Resource Identifier (URI).
For example, let’s say you’re creating a helicopter maintenance app. You can add
a button that a maintenance engineer can use to call an expert if they get
stuck. The button will launch [!include[pn-remote-assist](../includes/pn-remote-assist.md)] and call the designated expert.

[!include[pn-remote-assist](../includes/pn-remote-assist.md)] supports two methods for protocol activation: 

-   “ms-voip-video” is for video-enabled calling.

-   “ms-voip-call” is for audio-only calling.

Both methods use the same argument schema, which accepts a “contactID” field.
The URI would look something like this:

`
ms-voip-video:?contactids=\<contactID\>
`

The contact ID is the user’s [!include[pn-azure-active-directory](../includes/pn-azure-active-directory.md)] ([!include[pn-azure](../includes/pn-azure.md)] AD) objectID.

## Code sample

You’ll need to embed the code in your [!include[pn-hololens](../includes/pn-hololens.md)] app. The following code sample is
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

1.  Run your app on the [!include[pn-hololens](../includes/pn-hololens.md)].

2.  Initiate the call from your app.

3.  The [!include[pn-hololens](../includes/pn-hololens.md)] will appear to close the app, open [!include[pn-remote-assist](../includes/pn-remote-assist.md)] if it isn’t
    already open, and sign in.

4.  After the contacts panel is loaded, [!include[pn-remote-assist](../includes/pn-remote-assist.md)] will place a call to the
    specified contact.

### See also

For more details on launching an app with a URI, see [Launch an app with a URI](<https://docs.microsoft.com/en-us/windows/uwp/launch-resume/launch-app-with-uri>).
