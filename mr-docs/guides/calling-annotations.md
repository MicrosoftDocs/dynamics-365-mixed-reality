# Work with annotations in Dynamics 365 Guides on HoloLens

If you're using Dynamics 365 Guides on HoloLens, and you're on a call with a remote collaborator using Teams desktop or Teams mobile, you and the remote collaborator can both annotate your shared environment. Annotations are useful for pointing out different parts of your space, including parts that may be difficult or dangerous to reach. All call participants can see each others’ additions, and can make annotations of their own. Once an annotation is placed, it will remain anchored in your space until the person who placed the annotation deletes it. Adding annotations to files works the same way.

At this time, a HoloLens user can draw in their environment but can't place arrows. The remote expert on Teams desktop or Teams mobile can draw **and** place arrows.

Any user on Teams desktop, Teams Mac, or Dynamics 365 Remote Assist mobile can annotate the environment of the Dynamics 365 Guides user on HoloLens. Teams mobile users can only annotate in one-to-one calls, however, not group calls. Annotations are not supported for users on Teams Web. 

> [!NOTE]
> To use annotations, you must enable the appropriate permissions in Dynamics 365 Guides. [Learn more](hololens-permissions.md)

## Annotate your space in Dynamics 365 Guides on HoloLens

### Draw in your space

> [!NOTE]
> Annotations don't work well on black or reflective surfaces.

1. Select the **Ink** tool on the **Annotate** toolbar.

    SCREENSHOT GOES HERE

2. Use your hand ray to place the cursor where you want to start drawing.

    > [!NOTE
    > If hand rays are turned off in the HoloLens app, they're automatically turned back on again when you select the **Ink** tool.

3. Air tap, keep your index finger and thumb together, and start drawing in your space. Release the air tap to stop drawing. 

    > [TIP]
    > To use a voice command, select the **Ink** tool by saying "Guides, Ink." Then say "Guides, Start inking" and "Guides, Stop inking" to start and stop inking.

### Change ink color

- Select the **Color** tool on the **Annotate** toolbar, and then select the color you want. The next drawing that you do will be that color.

    SCREEN SHOT GOES HERE
    
### Erase your annotations

- To erase all drawings, select **Erase all**.

- To undo your most recent action, including the Erase all action, select **Undo**. 


## Add annotations in Microsoft Teams that appear in the Dynamics 365 Guides HoloLens user's space

When you join a call in Microsoft Teams, you'll see your collaborator’s space, including holograms, and can use the Mixed Reality toolbar in Teams to add annotations.

![Screenshot of the mixed reality toolbar.](media/mixed-reality-toolbar.PNG)

> [!NOTE]
> -	The toolbar appears only when the video on stage is from the Dynamics 365 Guides user.
> -	The toolbar will appear but will be disabled if the Dynamics 365 Guides user is not ready to receive annotations and files (for example, the  user's outgoing video feed is disabled, the user temporarily lost tracking, or Dynamics 365 Guides is not in the foreground because the user did the bloom gesture).
> -	The toolbar will not appear if the same Dynamics 365 Guides user is connected from Teams and Dynamics Guides at the same time, regardless of the device used.
> - The toolbar will not appear if you have not turned on the [new Microsoft Teams meeting experience](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/new-meeting-and-calling-experience-in-microsoft-teams/ba-p/1537581).

### Start annotating

To start annotating, first do one of the following to pause the video stream and enter edit mode:

-   Select anywhere in the Meeting window.

-   Select one of the items on the **Mixed Reality** toolbar.

-   Select **Start editing**.

In edit mode, you'll see a live stream of the call in the corner of the app window, including the annotations that other call participants add.

### Add arrows, ink, and files

Use the **Mixed Reality** toolbar to place arrows, draw, or add files in the HoloLens user's space. The following table describes the buttons in the **Mixed Reality toolbar.

|Button|Description|
|---------|----------------------------------------------------|
|![Graphic showing the place arrow icon.](media/6584f4b7932378aa23f6efbf460b304c.png)|Add an arrow.|
|![Graphic showing the ink icon, which looks like a pen.](media/187307e30fd713f5ae67aba854b78bc4.png)|Add ink (draw).|
|![Graphic showing the insert files icon.](media/insert-document-button.png)|Insert a file in the HoloLens user's space. You can select an image or PDF file from OneDrive or from your device.|
|![Graphic showing the pick a color icon.](media/5d9d3c70cf19ed175a8dc1ad71a60fc5.png)|Change the arrow or ink color.|

### Finish editing

When you're annotating, do one of the following:

-   Select **Stop editing**.

-   Select the live video feed in the corner of your screen.

### Make changes to your edits

To make changes to your edits:

- While in edit mode, select **Undo** to undo the last action.

- While in edit mode, select **Erase all** (![Graphic showing the Erase icon, which looks like a trashcan.](media/3aab547aa81003ad181eceadc2c83a47.png "Erase all")) to erase all of the annotations made during that editing session.

- While in live mode, select **Erase all** (![Graphic showing the Erase icon, which looks like a trashcan.](media/3aab547aa81003ad181eceadc2c83a47.png "Erase all")) to erase all of the annotations made during that call.

> [!Note]
> - Specific drawings or arrows can’t be removed.
> 
> - Each call participant can only remove the annotations that they add.

### Minimize the Mixed Reality toolbar

The Mixed Reality toolbar appears by default whenever you join a new call with a Dynamics 365 Guides user. 

![Screenshot of the Mixed Reality toolbar.](media/mixed-reality-toolbar.PNG "Screenshot of the Mixed Reality toolbar")

If you want to focus on the video stream from the HoloLens user, you can minimize the toolbar by selecting the **MR Toolbar** button. 

![Screenshot of HoloLens button.](media/minimize-MR-toolbar.jpg "Screenshot of HoloLens button")

> [!NOTE]
> The toolbar remains minimized if you switch to a different Dynamics 365 Guides user's video feed. 

To restore the toolbar, select the **MR Toolbar** button again. 
