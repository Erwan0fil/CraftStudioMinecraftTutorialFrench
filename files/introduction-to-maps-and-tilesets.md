[< Introduction to Models and Animations](introduction-to-models-and-animations.md)  
<div class="text-align-right next-tutorial-link">
<p>Introduction to Scenes and Scripts ></p>
</div>

---

# Introduction to Maps and TileSets

A character is great but it needs a world to evolve in, right.  
Lets create that with two more assets : a Map and the TileSet

A map is really like a Minecraft level : it is composed of blocks of different kinds. The map asset define which kind of block are where.  
The tile set define how those blocks looks, how they are shaped and textured.

In the project's home, go to the `Maps` tab and create a new map asset.

The new maps opens. If you look closely, the interface is not so different than the model's : there is a `Save` button, there is the chat, there is a black main window and a left column. In this column, you can find familiar terms like `Sheet size` or `Unwrap mode`.  
Some of what you learned during the creation of Steve's model and animation will also be useful with maps and tile set.

## Building levels, Minecraft-style

First we need to create a new tile set, we will proceed exactly like for the animation. Click on the `+/-` button, then create the new tile set with the name you want and a tile size of 16.  
As for the model block, a tile size of 16 means that the map blocks texture will be 16 pixels wide (when they have the shape of a cube).

Here is how the interface should looks like now :

![Map interface, with tile set](https://dl.dropboxusercontent.com/u/51314747/CraftStudio/MinecraftTutorial/img/intro-maps-tilesets/interface.png "Map interface, with tile set")

One white block has appeared in the map. 
If you focus the main window, a purple cube outline follow the mouse and outline any cubes the mouse hovers.

Building a map will sounds familiar because it works exactly like Minecraft : left click and a block appears inside the purple outline, right click over a block and it disappear. Left click over a block and a new one appear just next to the face the mouse hovered.

This is how you place blocks one by one. Don't forget you can move in the main window with WASDQE/middle mouse.  
We will see later a way to fill whole areas but for now we will mostly work on the tile set.

Be sure to be in the `Blocks` tab.  
The `Sheet size` is the texture size, you don't need to update it for now.  
As said, the `Tile size` is the same as the block's size. You can change it now to observe the blocks in the main window changing too.

The window below is the tile set's list of blocks (you can scroll up/down) because a tile set is always composed of 255 blocks which ID range from 0 to 254.

The blocks are cube by default but you can select any of the shapes in the `Shape` drop-down list. The shape updates in the blocks list, in the main window as wall as on the texture.  
Since we are building a Minecraft-like, cubes are fine.


## Painting

No surprise here, it's exactly the same principle as for models.  
You can change each block's `Unwrap mode` from the `Blocks` tab and paint them from the `Paint` tab.

Fro now we will paint three blocks : grass, dirt and stone.  
Stone and dirt are easy to do : it's the same grayish and brownish texture on all six faces of the cube.  
The dirt is a little different since the top face is greenish, the bottom as the same dirt texture and all side faces have the same dirt texture too but some green at the top.

The first block with ID 0 will be our grass block. This block uses three different textures, so set the unwrap mode to custom.  
We need the top and bottom face to use their own space on the texture. The front, left, back and right faces use together a third space.

Select the first block in the blocks list the set its unwrap mode to `Full` then to `Custom` then dispatch the outlines as needed.

![Grass block unwraps](https://dl.dropboxusercontent.com/u/51314747/CraftStudio/MinecraftTutorial/img/intro-maps-tilesets/grass-block-unwraps.png "Grass block unwraps")

Before setting the other blocks unwraps, I suggest we paint these first so that we easily see which part of the texture is dedicated to which block.  

As for Steve's face, you can try to reproduce the block's texture with the paint tools or find the texture online and copy/paste it.  
Here is my take on Minecraft's texture :

![Grass block texture](https://dl.dropboxusercontent.com/u/51314747/CraftStudio/MinecraftTutorial/img/intro-maps-tilesets/grass-block-texture.png "Grass block texture")

You can see (back in the `Blocks` tab) that two other blocks (ID 1 and 2) already got a texture. That's just because we actually painted under their texture unwrap.

The next block to texture is the dirt block. And I have actually nothing to do because the second block's (with ID 1) unwraps are already over the dirt texture (which is also used for the bottom of the grass block). That's why I painted the texture there and put the bottom face of the grass block in the middle.

If it's not your case, all you have to do is select the second block, keep the unwrap mode to `Collapsed` and move the unwraps over the dirt texture.

Painting the stone block should just require you to select the block with ID 2, move the unwraps to a blank space and paint.

![Grass, dirt and stone blocks](https://dl.dropboxusercontent.com/u/51314747/CraftStudio/MinecraftTutorial/img/intro-maps-tilesets/grass-dirt-stone.png "Grass, dirt and stone blocks")


## Mapping

One last thing you have to learn to master map building in CraftStudio is how to rotate blocks and how to create or remove big chunks of blocks. 

Go to the `Mapping` tab.

In addition to the blocks texture and shape, you can set one of the four the block orientation among the four available orientations : `North`, `East`, `South` and `West`.  
Click on one of the buttons with the initial of the orientation then lay the blocks in the main window as usual.

Placing blocks one by one is simple and it works, but it's long even with a team effort (something that CraftStudio allow you to do, remember ?).  
CS allows you to create an area that you can completely fill or empty at the push a single button.

Click on the button that looks like a dotted square.


---

[< Introduction to Models and Animations](introduction-to-models-and-animations.md)  
<div class="text-align-right next-tutorial-link">
<p>Introduction to Scenes and Scripts ></p>
</div>