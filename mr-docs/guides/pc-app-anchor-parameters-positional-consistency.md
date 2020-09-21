

# Things that can affect positional consistency when anchoring a guide with the Dynamics 365 Guides PC app

The following things can affect positional consistency when anchoring a guide with the Microsoft [Dynamics 365 Guides PC app](pc-app-anchor.md).

## Eye calibration and Interpupillary Distance (IPD) setting

IPD is the distance between the center of the user's pupils. Because different users might have different IPDs, it's crucial that the appropriate IPD is set, so that HoloLens can adapt its display. An incorrect IPD setting can cause inaccurate perception of hologram position. 

- To calibrate the device eye-tracking and IPD on HoloLens 2, make sure to use the eye calibration app when prompted. This will not only calibrate IPD but will also enable HoloLens 2 to auto-correct hologram position in case the device moves on the operator's head.

- To calibrate IPD on HoloLens 1, use the HoloLens Calibration app.

## Pre-scanning the environment

HoloLens actively scans its environment for visible features to map its surroundings. This scan occurs whenever the device is turned on and a user is signed in. It occurs regardless of whether you're in the HoloLens shell or running apps. HoloLens constantly improves the accuracy of these maps as it scans the environment from different viewpoints and stores the maps on the device. Holograms are placed in relation to these maps. The more accurate the map, the more accurate the hologram placement.

Before Dynamics 365 Guides is used on a HoloLens that hasn't been used in a particular environment, have the operator put on the HoloLens, sign in to the device, and walk around the space where hologram instructions have been placed or will be placed. Although the operator can do this step from the HoloLens shell, we recommend hiding the **Start** menu, so the operator can see the space as they walk around. By walking at a leisurely pace while slowly looking up and down, the operator will give the device an opportunity to find features and construct accurate maps. This process is called "pre-scanning," because it's done before running Dynamics 365 Guides. You only need to complete this process once for each environment, because HoloLens stores the maps that it creates on the device and remembers the spaces that it has scanned.

## Surface type

Environments that include very reflective surfaces (mirrors), dark surfaces, or featureless surfaces, negatively affect the ability of HoloLens to recognize the space. If HoloLens can't correctly recognize the space, hologram position and stability are affected in turn.

## Lighting conditions

Lighting conditions have an impact on how HoloLens perceives the environment and recognizes the space. Environments with unstable lighting conditions are prone to hologram instability. If the light changes significantly, HoloLens might consider the space as a new environment and build a new map for it. Previously visible features might be invisible and features that weren’t visible might be visible. In addition, HoloLens doesn’t map very bright or dark areas well. 

## Feature patterns

HoloLens builds maps of its surroundings, and tracks its position and hologram position based on visible features in the environment. If the space in which HoloLens is operating has a low number of visible features (mostly white walls for example), or very repetitive patterns (textured surfaces), this will impact hologram position and stability as HoloLens won’t be able to properly identify and track uniquely specific points in the environment. 

## Device wear (HoloLens 1 only)

HoloLens uses a novel display technology to project holograms in the operator's field of view. On HoloLens 1, the way that operators wear a device on their head has a huge impact on the perceived position of the holograms. The best way to understand this is to adjust the device positioning while aligning holograms to their physical counterparts in Dynamics 365 Guides. Notice how the alignment of holograms is affected when you shift the device left and right, up and down, or forward and backward. Operators should wear the device in a consistent way, and they should understand that subtle shifts in device positioning might not feel different but can cause significant changes in perceived hologram locations. On HoloLens 2, issues with device positioning are addressed through eye tracking.

