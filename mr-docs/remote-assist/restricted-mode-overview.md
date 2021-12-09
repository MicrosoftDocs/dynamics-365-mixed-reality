

# Protect company information by restricting capabilities in Dynamics 365 Remote Assist

[!INCLUDE[Private preview banner](includes/private-preview.md)]

In some cases, to protect company information, you might want to restrict capabilities in Microsoft Dynamics 365 Remote Assist. For example, you might provide HoloLens devices installed with Dynamics 365 Remote Assist to other businesses as part of your customer support system. You don't want these users to have access to your company information, but you do want them to be able to join meetings and receive meeting notifications so they can troubleshoot issues. This article and the linked articles below show you how to restrict calling, restrict access to contacts, files, and asset records, and keep Dynamics 365 Remote Assist users from signing into a different account.

Learn how to:

- [Restrict calling and the ability to access contacts](restricted-mode-calling.md)

- [Restrict the ability to access OneDrive files](restricted-mode-files.md)

- [Restrict the ability to access asset records](restricted-mode-assets.md)

- [Restrict the ability to change user accounts](restricted-mode-signout.md)

## Which restrictions are available on HoloLens vs. the mobile app?

The following table shows which restrictions are available for Dynamics 365 Remote Assist on HoloLens vs. the mobile app. 

|Restriction|HoloLens|Mobile app|
|-----------------------------------------------|-----------|----------|
|Calling and contacts|Yes|No, but you can set up [one-time-calling](one-time-call.md) for mobile app users|
|OneDrive files|Yes|Yes|
|Asset records|Yes|Yes|
|Change user accounts|Yes|No|
