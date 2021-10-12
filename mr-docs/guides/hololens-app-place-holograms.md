

# Place your holograms with the Dynamics 365 Guides HoloLens app

After [creating a guide with the PC app](create-guide.md) in Microsoft Dynamics 365 Guides, the next step in the authoring process is to place the holograms in your real-world 
environment. During this stage of the process, you walk through each step in your guide and place any assets that you associated with that step when you authored 
it in the PC app. For example, if you added a 3D part to help operators with a step, you'll place that part over its physical counterpart in the real world. If you 
added a 3D object from the 3D toolkit (for example, an arrow or a number), you'll place that object in an appropriate place in the real world, where it can draw the 
user's focus. You can place the same 3D part or 3D object as many times as you want.

You don't have to do anything to place an image or a video associated with a step. They automatically appear when the operator goes to the step.

## Place a 3D part

1. In the bin, air tap the 3D part that you want to place.

2. Use gaze and gestures to place the 3D part hologram over its counterpart in the real world. For information about how to manipulate holograms by using gaze and gestures, see the [Manipulating holograms](#manipulate) section later in this topic.

## Place a 3D model from the 3D toolkit

You can place a 3D model from the 3D toolkit in the same way that you place a 3D part, if you added that 3D model to the bin in the PC app. If you didn't add the 3D model in the PC app, you can also add it directly from the [!include[pn-hololens](../includes/pn-hololens.md)] app.

1. Air tap an empty box in the bin.

2. Air tap a category (for example, **Arrows** or **Hands**), and then air tap the specific 3D model that you want to add.

    ![Categories.](media/step-card-hands.PNG "Categories")

    The item is added to your bin, and you can then place it in the same way that you place a 3D part.

## Memory constraints when adding 3D models

When you author each guide step, you'll see a warning if the step complexity will likely result in a poor experience for the operator of the guide. 

ADD SCREENSHOT HERE SHOWING FIRST MESSAGE

If you see the "Warning! High step memory usage" message, the 3D models you place in the step will be displayed but the operator may have a degraded experience (the guide may have low frame rates or there may be noticeable loading times when moving between steps). 

If you continue to add 3D models and HoloLens reaches its memory limit, you'll see the "Step content failed to load" message.

ADD SCREENSHOT HERE SHOWING MESSAGE

At this point, any additional 3D model that you place will appear as an error icon. 

ADD SCREENSHOT HERE SHOWING EXAMPLE

For information on reducing step complexity, see [Optimize your 3D models to use with Dynamics 365 Guides and Power Apps](https://docs.microsoft.com/dynamics365/mixed-reality/guides/3d-content-guidelines/optimize-models).

## Best practices for working with 3D content

- Make sure that the 3D content isn't in the way of the operator who is doing the task.

- Keep the field of vision in mind when you place assets. If you put a hologram behind someone, it will be very hard to find.

- Use 3D content sparingly and for a clear purpose. Too much content can clutter the instructions and make them harder to follow.

- Remember that you can attach a tether to 3D content to make it more discoverable.
