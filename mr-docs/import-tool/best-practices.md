

# Best practices for real-time 3D models

This topic covers best practices for preparing 3D models to work with Dynamics 365 mixed reality applications.

## Reduce materials and surfacing

- Depending on the 3D model source and how you want to present the content, you may want to use the full capabilities of a physically based rendering (PBR) system. PBR systems allow for colors, roughness, and bumpiness to be visually represented by creating texture maps as opposed to having a multitude of different materials and surface complexities in the 3D model.

- If the asset only needs to be present and does not need the details provided by a PBR system, a significant increase in performance can be gained by only applying a single color. This will leave out extra texture data and surface information, like multiple colors, reflections and bumpiness.

PBR Screenshot goes here

A.	High performance single color 3D model with no PBR system
B.	3D model using the PBR system for higher-quality representation

## Reduce textures

- You can decrease the roughness map to increase the performance of the model.

roughness-map Screenshot goes here

A.	Model with roughness map texture of 2048 x 2048
B.	Model with roughness map texture of 1024 x 1024

- Reducing the resolution and the amount of textures will have the largest impact on memory consumption and file size.

- Reduce textures based on their visual impact. For example, metallic roughness maps can often be half the resolution of the base color and normal maps with no discernable quality reduction.

- JPG compression and PNG quantization will further reduce file size, but it will have no impact on the memory required at runtime when the asset is loaded.

## Remove hidden and unused data

- Be sure to remove any data that’s not required to represent your 3D models. Extra nodes, meshes, materials, and textures can add up quickly. For example, in the following 3D model, removing any hidden motor parts will lower the triangle count and simplify the hierarchy, resulting in a more performant 3D model.

remove-hidden-data Screenshot goes here

*Wireframe and shaded model visualized in [Autodesk Inventor](https://aka.ms/AutodeskInventorSoftware)*

