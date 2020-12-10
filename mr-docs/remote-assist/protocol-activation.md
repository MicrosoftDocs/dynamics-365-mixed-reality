---
author: bencorn
description: Launch Dynamics 365 Remote Assist from another app (protocol activation)
ms.author: bencorn
ms.date: 10/01/2019
ms.service: crm-online
ms.topic: article
title: Launch Dynamics 365 Remote Assist from another app
ms.reviewer: v-brycho
---

# Launch Dynamics 365 Remote Assist from another app (protocol activation)

You can embed code in your HoloLens, iOS, or Android application to switch to [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] and begin a call using a Uniform Resource Identifier (URI).

For example, let’s say you’re creating a helicopter maintenance app. You can add
a button that a maintenance engineer can use to call an expert if they get
stuck. The button will launch [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] and call the designated expert.

## HoloLens Protocol Activation

The Dynamics 365 Remote Assist HoloLens application supports two methods for protocol activation: 

-   “ms-voip-video” is for video-enabled calling.

-   “ms-voip-call” is for audio-only calling.

Both methods use the same argument schema, which accepts a “contactID” field.
The URI would look something like this:

`
ms-voip-video:?contactids=\<contactID\>
`

The contact ID is the user’s [!include[pn-azure-active-directory](../includes/pn-azure-active-directory.md)] ([!include[pn-azure](../includes/pn-azure.md)] AD) object ID.

### Code example

You’ll need to embed the code in your [!include[pn-hololens](../includes/pn-hololens.md)] app. The following code example is
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

### Return to your app at the end of a call

An additional "returnto" field can be included to have Dynamics 365 Remote Assist return to your application when a call ends. This enables users to both start and end their experience in your app without having to manually switch between them.

To support the "returnto" field, you need to register your app with a custom URI (see [Register an app with a custom URI](<https://docs.microsoft.com/windows/uwp/launch-resume/handle-uri-activation#step-1-specify-the-extension-point-in-the-package-manifest>)).

Then include the optional "returnto" field along with the registered app name you completed in the previous step. In the example below, "helicoptor-maintenance-app" is the registered URI:

`
ms-voip-call:?contactids=<CONTACT_ID>&returnto=helicoptor-maintenance-app");
`

#### Example of launching Dynamics 365 Remote Assist from your app with optional returnto field

The following code example is written in C++, but can be easily adapted to another language.

```
Platform::String^ id = objectId->Text;
auto uri = ref new Windows::Foundation::Uri("ms-voip-video:?contactids=" + id + &returnto=helicoptor-maintenance-app");
resultText->Text = uri->AbsoluteUri; 

concurrency::task<bool> launchUriOperation(Windows::System::Launcher::LaunchUriAsync(uri));
launchUriOperation.then([this](bool success)   
{         
    if (success)         
    {             
        // URI launched  
        resultText->Text += " (URI Launched)"; 
    } 
    else         
    {             
        // URI launch failed             
        resultText->Text += " (FAILED)";
    }     
});  
```

### Place a call to test your code

1.  Run your app on the [!include[pn-hololens](../includes/pn-hololens.md)].

2.  Initiate the call from your app.

3.  The [!include[pn-hololens](../includes/pn-hololens.md)] will appear to close the app, open [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] if it isn’t
    already open, and sign in.

4.  After the contacts panel is loaded, [!include[pn-remote-assist](../includes/pn-remote-assist.md)] will place a call to the
    specified contact.
    
For more information on launching an app with a URI, see [Launch an app with a URI](https://docs.microsoft.com/windows/uwp/launch-resume/launch-app-with-uri).

## iOS and Android protocol activation

The Dynamics 365 Remote Assist mobile application supports two methods for protocol activation: 

-   “ramobile” is for video-enabled calling.

The argument schema accepts an optional contactSearch field, which is a JSON-formatted array of strings to use for finding a contact.

    { "contactSearch":[ "supportContact@microsoft.com"] }

### Example

For this example, we will perform a contact search. We need to include the "contactSearch" parameter, which is an array of search strings.

1. First we form a JSON string:
```
	{
      "contactSearch":[
        "Jill Smith",
        "jillsmith@microsoft.example"
      ]
    }
```    
2. Encode this in base-64.
    ```ewogICJjb250YWN0U2VhcmNoIjpbCiAgICAiSmlsbCBTbWl0aCIsCiAgICAiamlsbHNtaXRoQG1pY3Jvc29mdC5leGFtcGxlIgogIF0KfQo=```

3. Append the base-64 encoded string to "ramobile:" to form the new URI.
   ```"ramobile:ewogICJjb250YWN0U2VhcmNoIjpbCiAgICAiSmlsbCBTbWl0aCIsCiAgICAiamlsbHNtaXRoQG1pY3Jvc29mdC5leGFtcGxlIgogIF0KfQo=";```
    
When this link is selected, Remote Assist mobile will launch and search for the provided contact details and provide results to the user.
