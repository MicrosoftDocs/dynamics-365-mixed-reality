
# Anchor a guide in Dynamics 365 Guides by using an Object anchor (Preview)

You can use an object anchor to align a guide to a real-world object instead of using a printed anchor (QR code or circular code). 

> [!Note]
> Object anchors are available on HoloLens 2 only.  

Since object anchors are a preview feature and are not fully supported at this time, we recommend that you use a test Microsoft Dataverse environment separate from your production environment. [Learn how to set up a test Microsoft Dataverse environment](). 

You can use any 3D model of a real-world object or you can capture the object with different scanning applications (OCap, etc., need to add examples here – mostly iOS ones).  

For more information on the ideal conditions for an object anchor candidate, see [Best practices for object anchors]()

## Convert a 3D model into an object anchor  

1. In the PC app, on the **Outline** page, select **Anchor**.

    SCREEN SHOT GOES HERE

2. On the **Choose an anchor method** page, under **Object Anchor (Preview)**, select **Select**.

    SCREEN SHOT GOES HERE 

    > [!NOTE]
    > If you see **Try Preview**, contact your administrator for access. The Object anchor preview is available for all regions except the GCC region.   

3. 
In step 1 of the wizard, you can assign the Object Anchor to your guide. If you would like to add your 3D model as an Object Anchor, select Create from the Library and you will be directed to the Guides Model Driven App in a web browser.  

Note: restricted authors may not be able to access the Model Driven App  

[screenshot of Library create/ Assign page] 

 

From the Guides Model Driven App, you will be able to create a new Object Anchor.  

Graphical user interface, application, email

Description automatically generated (If you see an error message to assign to an app, select Guide Portal – need confirmation and screenshot) 

If you see an error message in your web browser for permission, sign into your browser with the credentials from your environment. Make sure you are signed in as an author or administrator with appropriate permissions to access the Model Driven App.  

 

In the Guides Model Driven App, there are instructions on the right to create new Object Anchors.  

Step 1: Name your object anchor [screenshot of name field] 

Step 2: Select ‘Save’. [screenshot of save button] 

Step 3: Upload your Source 3D file. Note: button will not appear until you select Save after naming the Object Anchor [screenshot of button] 

Note: supported file types 

Step 4: Enter the ‘Conversion’ details. Note: confirm gravity direction and length unit. -Y is default to set the Object Anchor in right orientation compared to the floor. [need to add more details/ tips for orientation and measurements]  

Step 5: Select ‘Convert 3D File’ [screenshot of button] 

The 3D model is now being converted into an Object Anchor. The status of the conversion will update from New to Requested to Started. You can also select Refresh to refresh status on the page. During conversion you can create other Object Anchors or return to the PC application to edit your guide.  

When conversion has moved to Succeeded you can return to the PC application to complete anchoring. If conversion has Failed, please try again [screenshot of + New button] 

You can also assign a thumbnail to your Object Anchor so it can be distinguished in the PC app library. If you do not assign a thumbnail, a default object anchor thumbnail will appear.  

Select the circle next to the Object Anchor name [screenshot] 

Select Upload image and select the desired image as the thumbnail from your window explorer  

The image will upload and the preview will change to the image once it has finished uploading. Confirm the image by selecting Change or cancel by selecting Cancel 

Assign Object Anchor in PC app 

Return to the PC app to assign your Object Anchor. The Library will have updated with the new Object Anchor under the Object Anchor tab [screenshot]. Note: select Next and then Back to refresh Library in the Anchor wizard 

Drag and drop the Object Anchor to assign it to the guide  

The next three steps in the Anchor wizard are optional.  

Select Next and optionally, take a photo of the target object you wish to anchor to  

Select Next and optionally, import the photo of the target object location. This will help operators preview the object.  

Select Next and add custom instructions as needed to help the operator find the target object.  

Complete the Anchor wizard on the PC app. In order to complete assignment of the Object Anchor, move to the HoloLens app.  

Assign Object Anchor in HL app 

Open your guide with the Object Anchor in the HoloLens app  

Locate your target object  

Initiate scan  

Move around the object to scan it and the HoloLens will automatically recognize the object based on the Object Anchor  

[Potential errors] 

Continue to move around the object if you are prompted to [capture of movement prompt] 

Once the scan is successful, [mesh…] 

[Observe the object and confirm it is accurately aligned – potential here to recommend users to put arrow in first step to test alignment]  

Note: If you have issues with object detection and content alignment, try clearing the mesh and all holograms from the HoloLens Settings menu. Go to System > Holograms > select the Remove all holograms button. 

Your guide is now successfully anchored to the Object Anchor 

You can also switch your anchor method between Object Anchor and QR, Circular, or Holographic, but object placements within that guide will need to be re-authored.  

Using Object Anchor as an Operator 

Operators will be able to scan the target object and use the guide automatically aligned. […] Rescan the object if alignment is not correct to the target object. [example photos of misaligned object anchors?] 

## Best practices for object anchors

### Size 

To achieve accurate detection and alignment, the target object should be 1-10 meters for each dimension. 

### Scanning 

For larger objects such as cars, it’s advisable to move around the object while the initial detection is underway so that AOA is able to work with a larger span of sensed data for its detection and alignment. Standing in one spot may give very little surface information and AOA detection might not go above the detection threshold. 

### Materials 

Highly reflective and dark materials are difficult to detect with HoloLens. If HoloLens is unable to detect the surface, AOA will not be able to use sensor data for alignment and detection. 

### Topology 

AOA works best on larger objects that have unique topology and asymmetric features. 

• Do not use symmetrical objects as this can cause confusion about the orientation of the object. 

• Use objects that have unique shapes and edges. 

• Do not use objects that are mainly composed of thin pipes or wires. 

• Use objects that won’t change shape across your process. An updated shape will require a new 3D model.  

Known Issues 

Azure Object Anchor is a preview anchor method in Guides and has certain limitations to the experience.  

Migration tool is not supported for Azure Object Anchor in Guides Preview 

Region support is limited in the preview stage [GCC region not supported, data flow to East US2?] 

[Switching anchor type will not migrate over the saved position information?] 

Offline mode not supported  

 

 

 

 

Page Break
 

For internal reference: 

FAQ 

What 3D file formats does the Azure Object Anchor service support? 

.obj   .fbx   .glb   .gltf   .ply 

What are the recommended object parameters when creating an object anchor? 

1-6 meters for each dimension. 

Non-symmetric, with sufficient variations in geometry. 

Low reflectivity (matte surfaces) with bright color. 

Stationary or occasional movement, no or small amounts of articulation. 

Clear backgrounds with no or minimal clutter. 

Object layout close to the layout of its model. 

What is the maximum file size allowed to be ingested? 

1 GB 

How long does ingestion take? 

For a ply model, typically 3-15 minutes. If submitting models in other formats, expect 

to wait 15-60 minutes depending on file size 

How accurate is an estimated pose? 

It depends on object size, material, environment, etc. For small objects, the estimated 

pose can be within 1-cm error. For large objects, like a car, the error can be up to 2-8 cm. 


