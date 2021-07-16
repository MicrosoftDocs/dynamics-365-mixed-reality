
# Anchor a guide in Dynamics 365 Guides by using an Object anchor (Preview)

You can use an object anchor to align a guide to a real-world object instead of using a printed anchor (QR code or circular code). 

> [!Note]
> Object anchors are available on HoloLens 2 only. To create an object anchor, you must have the required privileges to open the Guides model-driven app. 

Since object anchors are a preview feature and are not fully supported at this time, we recommend that you use a test Microsoft Dataverse environment separate from your production environment. [Learn how to set up a test Microsoft Dataverse environment](). 

You can use any 3D model of a real-world object or you can capture the object with different scanning applications (OCap, etc., need to add examples here – mostly iOS ones).  

For more information on the ideal conditions for an object anchor candidate, see [Best practices for object anchors]()

## Overall process for converting a 3D model to use as an object anchor and assigning to a guide

Converting a 3D model into an object anchor and assigning it to a guide involves the following steps:

1. Start with the Anchor wizard in the PC app.

2. Convert the 3D model in the Guides model-driven app.

3. Go back to the Anchor wizard to assign the anchor to the guide.

4. Anchor the guide in the HoloLens app.

Each of these steps is described in detail below.

## Convert a 3D model into an object anchor  

To convert a 3D model into an object anchor, you start with the Anchor wizard to select the anchor type, and then you use the Guides model-driven app to convert the 3D model.

### Chose the anchor type in the Anchor wizard

1. In the PC app, on the **Outline** page, select **Anchor**.

    SCREEN SHOT GOES HERE

2. On the **Choose an anchor method** page, under **Object Anchor (Preview)**, select **Select**.

    SCREEN SHOT GOES HERE 

    > [!NOTE]
    > If you see **Try Preview**, contact your administrator for access. The Object anchor preview is available for all regions except the GCC region.   

3. If you haven't already done so, you'll need to update the solution to use the object anchor feature. To get instructions on updating the solution, select **Update solution**.

4. In step 1 of the wizard, to add your 3D model as an object anchor, select **Create from the Library**. ???WHERE IS THIS IN THE WIZARD??? This opens the Guides model-driven app in your web browser.   

    > [!NOTE]
    > If you're prompted for credentials, sign in with the credentials for your environment. You must be signed in as an author or administrator with the appropriate permissions to access the model-driven app. You must have the XXX privileges to access the Guides model-driven app.   
    > 
    > [screenshot of Library create/ Assign page] 

### Convert the file in the Guides model-driven app

You can use the instructions on the right in the Guides model-driven app to select and convert your 3D file.

1. Name your object anchor [screenshot of name field] 

2. Select **Save**. [screenshot of save button] 
    
   > [!NOTE]
   > You can't upload a 3D source file until you select **Save**.

3. Under **Upload**, select **Choose File**, and then browse to your 3D model and upload it. The following file types are supported:
    
      - .obj   
      - .fbx   
      - .glb   
      - .gltf   
      - .ply 

4. Under **Conversion**, enter the details. -Y is the default to set the object anchor in right orientation compared to the floor. [need to add more details/ tips for orientation and measurements]  

5. Select **Convert 3D File**. [screenshot of button] This starts the conversion process. You can use the **Conversion Status** field to check on status. You can also select **Refresh** to refresh the page status. During the conversion, you can create other object anchors or go back to the PC app to edit your guide. If the conversion fails, start the process again. 

6. When it's done, you'll see "Completed" in **Conversion Status** field. You can then go back to the Anchor wizard to complete the anchoring process.

### Assign a thumbnail to the object anchor (optional)

You can also assign a thumbnail to your object anchor in the model-driven app to make it easier to find in the PC app library. If you don't assign a thumbnail, a default object anchor thumbnail will be assigned.  

1. In the model-driven app, select the circle next to the object anchor name.

    SCREENSHOT GOES HERE

2. Select **Upload **Image**, and then select the image you want. The preview will change to the image after it has finished uploading.

    SCREENSHOT GOES HERE

## Assign the object anchor in the Anchor wizard 

Next, you'll go back to the PC app to assign the object anchor to your guide.

1. In the PC app Anchor wizard, select **Next** and then **Back** to refresh the library. ???Where is Object Anchor tab???

    SCREENSHOT GOES HERE

2. Drag and drop the object anchor to assign it to the guide, and then select **Next**. 

3. Take a photo of the target object location (optional) to make it easy for the operator to find the target object. Select **Next**. 

4. Import the photo, and then select **Next**. 

5. Add custom instructions (optional) as needed to help the operator find the target object. Select **Next**.  

6. Select **Complete**. 

## Anchor the guide in the HoloLens app 

The final step happens in the HoloLens app.

1. Open the appropriate guide in the HoloLens app.  

2. Locate the target object used for the anchor.

3. In the xxx dialog box, select **Initiate Scan**.  

4. Move around the object to scan it. The HoloLens will automatically recognize the object based on the object anchor.  

    > [!NOTE]
    > If you're prompted to XXX, continue to move around the object. ???What does error message say???

5. If the scan is successful, you'll see the following message.

    SCREEN SHOT GOES HERE

6. [Observe the object and confirm it is accurately aligned – potential here to recommend users to put arrow in first step to test alignment]  

    > [!NOTE]
    > If you have issues with object detection and content alignment, try clearing the mesh and all holograms from the HoloLens **Settings** menu (**System** > **Holograms** > **Remove all holograms**). 

    At this point, your guide should be successfully anchored to the object anchor. 

    > [!NOTE]
    > You can switch the anchoring method to a QR code, circular, or holographic anchor, but if you do so, the placement of objects within the guide will need to be re-authored.  

## Anchor the guide as an operator 

Operators can scan the target object in the same way to automatically align the guide. If the guide is misaligned, operators should rescan the target object. [example photos of misaligned object anchors?] 

## Best practices for object anchors

### Size 

To achieve accurate detection and alignment, the target object should be 1-10 meters for each dimension. 

### Scanning 

For larger objects such as cars, we recommend moving around the object while the initial detection is underway so that HoloLens is able to work with a larger span of sensed data for detection and alignment. Standing in one spot may doesn't provide very much surface information/might not go above the detection threshold. 

### Materials 

Highly reflective and dark materials are difficult to detect with HoloLens. If HoloLens is unable to detect the surface, the object anchor will not be able to use sensor data for alignment and detection. 

### Topology 

Object anchors work best on larger objects that have unique topology and asymmetric features. 

• Do not use symmetrical objects as this can cause confusion about the orientation of the object. 

• Use objects that have unique shapes and edges. 

• Do not use objects that are mainly composed of thin pipes or wires. 

• Use objects that won’t change shape across your process. An updated shape will require a new 3D model.  

## Known issues 

Object anchors are a preview feature and have the following limitations: 

- The Content Migration tool is not supported.

- The GCC region is not supported.

- [Switching anchor type does not migrate saved position information] 

- Offline mode is not supported.  

## FAQ

### What 3D file formats are supported for object anchors? 

The following 3D file formats are supported:

- .obj   
- .fbx   
- .glb   
- .gltf   
- .ply 

### What are the recommended object parameters for object anchors? 

- 1-6 meters for each dimension. 

- Non-symmetric, with sufficient variations in geometry. 

- Low reflectivity (matte surfaces) with bright color. 

- Stationary or occasional movement; no or small amounts of articulation. 

- Clear backgrounds with no or minimal clutter. 

- Object layout close to the layout of its model. 

### What is the maximum file size for the 3D model? 

The maximum file size is 1 GB. 

### How long does it take to convert a model in the Guides model-driven app?

For a .ply model, the conversion process typically takes 3-15 minutes. For other formats, the conversion process takes 15-60 minutes depending on the file size. 

### How accurate is an estimated pose? 

It depends on the object size, material, environment, and so on. For small objects, the estimated pose can be within 1-cm error. For large objects, like a car, 
the error can be up to 2-8 cm. 


