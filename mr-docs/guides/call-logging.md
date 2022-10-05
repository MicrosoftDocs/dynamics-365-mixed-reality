# View calling data stored by Dynamics 365 Guides

When Microsoft Dynamics 365 Guides users make or receive calls in the HoloLens app, call information is stored in Microsoft Dataverse. Anyone who has access to make.powerapps.com or the Guides environment can view calling data in the Guides model-driven app. Users can view only their own calling data; administrators can view calling data from all users. 

Location data is only stored in Microsoft Dataverse if the user consents to store that data. Users are prompted to provide permission to store location data when they start the HoloLens app for the first time, but they're not required to store that data to use the HoloLens app. If a user chooses not to store location data, other calling information is stored, but location fields in the app will be empty. [Learn more about HoloLens app permissions](hololens-permissions.md)

> [!Note]
> This feature is intended to help supervisors and managers derive insights regarding operational efficiencies and usage of Dynamics 365 Guides. This feature is not intended for use in making — and should not be used to make — decisions that affect the employment of an employee or group of employees, including compensation, rewards, seniority, or other rights or entitlements. Customers are solely responsible for using Dynamics 365, this feature, and any associated feature or service in compliance with all applicable laws, including laws relating to accessing individual employee analytics and monitoring. End users will need to enable access from their device to phone call records and specifically consent to sharing location information before that information is shared and available. However, customers are also encouraged to have a mechanism in place to inform their users that analytics (such as call duration and location) relating to their communications are collected.

## View calling data

1. [Open the Guides model-driven app](open-model-driven-app.md).

2. On the left side of the screen, under **Analytics and insights**, select **Phone Calls**.

    ![Screenshot of model-driven app with call information.](media/call-logging-model-driven-app.JPG "Screenshot of model-driven app with call information")

3. If you're a user, you can view your own call records. If you're an administrator, to view all call records, select the **All Phone Calls** view. 

## What data is stored and when

> [!NOTE]
> Dynamics 365 Guides stores calls data to a persistent queue in Microsoft Dataverse. If the call data isn't uploaded the first time, Dynamics 365 Guides attempts to  upload data three more times at different time intervals. This increases the reliability of data uploading.

### Updated at the start of the call

The following data is updated at the start of the call: 

- CallId
- CallStart
- CallEnd - intentionally set to same value as 'CallStart' at the beginning, until we know the real time of end
- ClientType (Hololens, Hololens 2, Android, iOS)
- Subject (to 'Dynamics 365 Remote Assist Call' or localized version as appropriate OR 'Dynamics 365 Guides')
- IsOutgoing
 
### Updated soon after the call starts

The following data is updated soon (within 2-5 seconds) after the start of the call, but only if the user provided permission to store location data:

- City (city where the call was taken)
- StateOrProvince
- Country
- Latitude
- Longitude 

### Updated at the end of the call

The following data is updated at the end of the call, but only if the Dynamics 365 Guides app is in foreground:

- CallDurationMinutes (duration of the call in minutes)
- CallDurationSeconds
- CallEnd
- StateCode (to 'Completed')
- StatusCode (to 'Made' or 'Received')

## See also

- [Call a remote collaborator](calling-start-call.md)
- [Join a scheduled meeting](calling-meetings.md)
- [Chat](calling-chat-file-sharing.md)
- [Record a call](calling-record-call.md)
- [Teams users capabilities](calling-teams-users.md)

