| **Statistic** | **Definition**  | **Recommend limit per step** |
| ------------- | --------------- | ---------------------------- |
| Triangles     | Number of mesh triangles across all parts in a 3D object | 250,000 |
| Parts         | Number of nodes in a 3D object's scene hierarchy | 500 |
| Vertices*      | Number of mesh vertices in a single part of a 3D object | 815,000 per part |
| Textures      | Number of pixels, in megapixels, across all textures referenced by parts and materials in a 3D object | 48  |
| Texture size*  | Number of pixels, in megapixels, contained in a single texture | 16 per texture (4096 x 4096 or equivalent) |

> [!NOTE]
> Triangles, parts, and texture limits are guidelines. Any step containing content which nears the limits of all values might exceed the recommended memory limits for a single step. Higher complexity steps might result in longer load times.
>
> *Vertices and texture size limits are enforced. Exceeding these limits means content won't load on HoloLens.