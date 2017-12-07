In *Red Eclipse* (and other *Cube 2* engine games) all map geometry is based on octrees. Understanding the basics of this approach is useful when [editing](editing "wikilink") or creating new [maps](official_Maps "wikilink").

## What is an octree?

In essence, the volume is represented by cubes that can be subdivided recursively and adaptively. This means that

-   each cube can be split into *2x2x2* child cubes,
-   child cubes can be split as well, up to a minimal cube size,
-   child cubes can be merged back into parent cubes and
-   various grid sizes (powers of 2) can be used in the same map.

[thumb|Octree: Cubes of different grid sizes are pushed and pulled](file:octree.gif "wikilink")

## Material volumes

Map [materials](materials "wikilink") allow to add water, clipping or other volumetric properties to a map. These materials are always defined for the entire volume of a cube unit. Therefore, the material boundaries or surfaces are always horizontal or vertical. Each cube can have multiple material properties.

## Cube geometry

Every cube unit can hold a block of solid geometry that consists of 8 vertexes and 6 cube faces. So far, this is no surprise, however, the vertexes can be moved to create more complicated geometry. This is done on a grid with a spacing of 1/8 of the cube unit's size (9x9x9 grid points). Each cube face can have its own texture, and the same texture is used when a cube face is folded to form two triangles. For instructions how to manipulate geometry, move vertexes and apply textures, see [editing Controls](editing_Controls "wikilink"), [height Mapping](height_Mapping "wikilink") and [texturing](texturing "wikilink").

[thumb|A vertex is moved along an edge. Note how the texture gets deformed.](file:Vertex.gif "wikilink")

## Grid sizes and loss of geometry

When editing a map, players are free to change the grid size for their editing actions (default bind: G and mouse wheel). When manipulating cube units that use a different grid size (edge length) than the player's current grid (cursor size), the cube units will be split into child cubes or merged into parent units as needed. So for example, if the player wants to [move](Editing_Controls "wikilink") a piece of geometry or apply a [material](materials "wikilink") property, it is recommended to use a grid size larger or equal to the coarsest geometry unit of the current selection. Otherwise, it is possible that some geometry information will be lost as the cube units are rearranged. For example, some slopes cannot be reproduced automatically when shifting a cube unit by half of its size, such that it has to be split into 8 child cubes.

[thumb|Some slope geometry is broken as a smaller cube is pushed.](file:broken.gif "wikilink")
