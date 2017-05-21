Archipelago
===========

This project is a collection of floating islands for use with the Minecraft plugin [TerrainControl](https://github.com/MCTCP/TerrainControl). The islands come in a variety of shapes and sizes.

Note that using these islands in your world requires working knowledge of how to install, use, and configure TerrainControl. If you're not familiar with this plugin or how it works, then it's recommended that you browse [the TerrainControl wiki](https://github.com/MCTCP/TerrainControl/wiki) to learn about it.

Installation
------------

Installing the islands is as simple as dropping the files and folders in this directory into your `GlobalObjects` folder or into the `WorldObjects` folder of the world you intend to use them in. The islands are defined as BO3's which will be made available to TerrainControl for use in your custom biomes.

Use
---

The islands can be spawned in a number of ways. Depending on your use case, you can either spawn islands by class or by their individual shapes.

### Island classes

A number of island "classes" are defined that provide a simple way to spawn a variety of islands. As their names suggest, they roughly correlate to the size of the island you want to spawn. These are listed below.

 * `island_large`
 * `island_medium`
 * `island_small`
 * `island_tiny`

The BO3's for these island classes can be found in [the island_classes folder](https://github.com/EmptyStar/Archipelago/tree/master/island_classes).

### Island shapes

Each island is defined by its size -- approximately its grid size in chunks -- and its shape. The smallest size is 1x1, and the largest is 4x4. Each of these islands is configured to rotate randomly, and the larger islands (3x3, 4x3, and 4x4) have various shapes that give them more natural variety.

Each shaped island is denoted with a capital letter that roughly mimics the island's shape. For instance, a `3x3_L` island is an island that is three square chunks in size (48 square blocks) and is shaped like the letter 'L'. Likewise a `4x4_T` island is four square chunks (64 square blocks) and is shaped like the letter 'T'. Note that the lettering system isn't an exact science and only serves as a simplistic approximation of the island's shape.

The individual islands can be found in the sub-directories within [the island_shapes folder](https://github.com/EmptyStar/Archipelago/tree/master/island_shapes), and they're also listed for convenience in [shapes.txt](https://github.com/EmptyStar/Archipelago/tree/master/island_shapes/shapes.txt).

Filled Islands
--------------

In addition to the normal islands, most islands have a "filled" counterpart. These islands are identical to the normal islands with the exception of being filled with STRUCTURE_VOID blocks. These are useful if you want to spawn an island filled with some other block such as water or lava. It's expected that you use the `ReplacedBlocks` setting in your custom biome to replace all STRUCTURE_VOID blocks with the block of your choice.

Development Components
----------------------

Included under [the dev folder](https://github.com/EmptyStar/Archipelago/tree/master/dev) are versions of the islands' components that include markers for accurately capturing the components using [WorldEdit](http://wiki.sk89q.com/wiki/WorldEdit). As the folder name suggests, these components are intended for _development_ and aren't meant to be used in actual terrain generation. These are meant to be used if you want to modify a component or create a new component. All of the names of the BO3's are prefixed with `dev_`.

If you want to capture a component using WorldEdit, use the two-point selection tool to set your first point to the _orange_ wool block and your second point to either the _blue_ wool block or the farthest corner opposite the orange wool block in lieu of a blue wool block.

Known Issues
------------

Below are the known issues for this version of Archipelago.

 * No filled islands or components exist for 1x1 islands
 * `landmass_2` and `landmass_3` are unused
 * No development BO3's exist for edge boulders and floating boulders
 * The BO3 settings of the development components do not closely match those of their production counterparts
 * Some filled components are missing a STRUCTURE_VOID block

License and Authors
-------------------

Created by EmptyStar. License MIT; see [LICENSE](https://github.com/EmptyStar/Archipelago/tree/master/LICENSE) for more info.
