---
title: Set up and use Microsoft Teams with Remote Assist to collaborate on a call
---

# Set up and use Microsoft Teams with Remote Assist to collaborate on a call

A Microsoft Dynamics 365 Remote
Assist user on HoloLens can
work collaboratively with a colleague (typically an expert in a particular
field) during a video call by using Microsoft Teams. The expert can see
everything that the Remote Assist user sees, and they can holographically draw
and annotate together. For example, let’s say a first-line worker is servicing a
very complex machine and isn’t sure how to solve a problem. The first-line
worker can call an expert anywhere in the world and have the expert assist with
the servicing using annotations or files.

Setting up this collaboration using Teams is simple and it’s free for the
expert.

Need more help? [Check out Remote Assist FAQ](faq.md) for answers to common questions.

[Watch how-to videos](videos.md) about Remote Assist.

## What you’ll need

The Remote Assist user (first-line worker) needs:

-   [A subscription to Remote Assist.](../licensing/buy-and-deploy.md)

-   A HoloLens running the [Windows 10 April 2018
    Update](https://support.microsoft.com/en-us/help/12643) (or later).

-   An Azure Active Directory account.

-   A work or school account with an [Office 365](https://products.office.com/business/office) Premium or Essentials
    subscription.

The expert needs:

-   A PC running Windows 10 with the latest version of [Microsoft Teams.](https://products.office.com/microsoft-teams/group-chat-software)

    Microsoft Teams is available [as a free download](https://teams.microsoft.com/downloads).

-   A free Microsoft account. The expert might already have a Microsoft account
    if they signed up for the Microsoft App Store, Skype, Xbox, Hotmail, or
    Outlook.com. If the expert doesn’t already have a Microsoft account, they
    can sign up for one by going to [https://account.microsoft.com/account](https://account.microsoft.com/account).

## Setup

You can onboard an expert and collaborate using Teams in three easy steps:

| **Step** | **Description**                                                                  | **Who does this step?**           |
|----------|----------------------------------------------------------------------------------|-----------------------------------|
|    1.      | Enable guest access for Teams                                                    | Administrator                     |
|    2.      | Invite the expert to join a team as a guest using the expert’s Microsoft account | Administrator or Remote Assist user and expert (to download Teams) |
|    3.      | Place a call                                                                     | Remote Assist user or expert     |

### Step 1: Enable guest access for teams

1.  If you’re the admin for the main Azure tenant, go to
    <https://portal.office.com/adminportal/> to open the Office Admin portal,
    and then sign in.

2.  From the menu on the left, select **Show More** \> **Settings** \> **Service
    & add-ins**.

    ![](media/bf81ea48e3ccd560b6f44dbc72a73eb5.png)

1.  Select **Microsoft Teams** from the list of applications.

    ![](media/ad846431f181b1c6df362bc2e0e03167.png)

1.  Select **Settings by user/license type**.

2.  In the drop-down list next to **Select the user/license type you want to
    configure**, select **Guest**.

3.  Set **Turn Microsoft Teams on or off for all users of this type** to **On**,
    and then choose **Save**.

    ![](media/9f095e7553a4af03ff13ea6a29a9343a.png)

4.  Wait an hour for the settings to propagate.

### Step 2: Invite the expert to join a team

1.  In Teams, select **Join or create a team** to create a team if it doesn’t
    already exist. The Remote Assist user and the expert must be on the same
    team to communicate.

    ![](media/16e00f809d210dcb3b1e8c8e859b73da.png)

1.  When asked to add members, enter the expert’s Microsoft account.

    ![](media/71e9276273f8f47b786f743416a2cb64.png)

    > [!NOTE]
    > If you don’t see the option to add a guest by typing an email address, it’s likely that guest access isn’t enabled on your company’s Azure tenant for Teams. Enable guest access as described earlier in this topic.

1.  The expert will immediately receive an email message and can click the link
    in the message to open (or download) Microsoft Teams. This version of Teams
    is free and is not a trial version.

### Step 3. Place a call

1.  The expert launches the Teams app and the Remote Assist user on the HoloLens
    signs in to their account as usual.

    > [!IMPORTANT]
    > If this is the first time the expert has launched Teams and the expert has not been invited to any other teams, Teams will automatically take the expert to the correct place. If the expert has been invited to other teams, the expert might need to switch to the appropriate tenant.  
    >     
    > To switch tenants, in the drop-down menu in the upper-right corner of the window, select the appropriate guest tenant:
    
    ![](media/55237a5359fb66daf7bbb9413adab6b9.png)
       
    > [!NOTE]
    > Teams might take a few seconds to reload.
    
1.  Either party can make the call. You might need to search contacts to find
    the right person.

    > [!NOTE]
    > The guest can call any member on the same team. To extend this functionality, invite any other members within your company who would benefit from being able to access this new expert.

## Working with annotations

Once Teams is installed, the expert can make video calls to (and receive them
from) contacts using Remote Assist on a HoloLens.

When in a call, the expert will see the contact’s space—including the
holograms—and can use the Mixed Reality toolbar in the video call window to add
holograms.

![](media/071f358ab6bbf7c2072b15d9203a1593.png)

## Draw and annotate

### Edit mode

To start annotating a contact’s space, first do one of the following to pause
the video stream and enter edit mode**:**

-   Select anywhere in the call window.

-   Select one of the items on the Mixed Reality toolbar.

-   Select **Start editing**.

In edit mode, the expert will still see a live stream of the call in the corner
of the app window.

### Add arrows, ink, and files

Use the Mixed Reality toolbar to place arrows, draw, or add files:

-   To add arrows, select **Place arrow** ![](media/6584f4b7932378aa23f6efbf460b304c.png) .

-   To add ink, select **Ink** ![](media/187307e30fd713f5ae67aba854b78bc4.png) .

-   To change the arrow or ink color, select **Pick a color** ![](media/5d9d3c70cf19ed175a8dc1ad71a60fc5.png) .

-   To add a file, select **Insert files** ![](media/41aa538d3be8e163215f7d9374abe90e.png), and then add an image file or a PDF file.

    > [!NOTE]
    > After adding them, images can’t be moved, deleted, or resized by the expert.

### Finish editing

When done annotating, do one of the following to finish editing and return to
live mode:

-   Select **Stop editing**.

-   Select the live video feed in the corner of your screen.

### Make changes to edits

To make changes to edits, do one of the following:

-   While in edit mode, select **Undo** to undo the last action.

-   While in edit mode, select **Erase all** ![](media/3aab547aa81003ad181eceadc2c83a47.png) to erase all of the annotations made during that editing session.

-   While in live mode, select **Erase all** ![](media/3aab547aa81003ad181eceadc2c83a47.png) to erase all of the annotations made during that call.

> [!NOTE]
> Specific drawings or arrows can’t be removed. Only the HoloLens user can make changes to or delete pictures added by an expert.

### See also
[User Guide](user-guide.md)<br/>
[How-to videos](videos.md)<br/>
[FAQ](faq.md)<br/>
