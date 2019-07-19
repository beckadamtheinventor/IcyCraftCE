IcyCraft version 2.12.0 (TI-84+CE)
by beckadamtheinventor
June 2019


--!IMPORTANT NOTE!--
Old worlds from 2.9.1 and before will now be automatically converted to match the new naming convention


--ABOUT--
IcyCraft is similar to Minecraft, with textures I made myself, using TileMapE. (shameless self promotion)
It is made in 2D 'layers', each one stored in seperate appvars, to ensure the maximum possible world size.
All of IcyCraft's blocks/items are externally defined, meaning that all 256 IDs are customizable!
I will be adding dev info for such customization soon.


--CREDITS--
Thank you to everyone at Cemetech for their ongoing teaching and support for my various projects!
Cemetech++
Thank you TimmyTurner62, for giving me that final push of motivation for me to actually sit down and finish this project!

And of course, without Peter "PT_" Tillema, IcyCraft would never had been a thing. Thank you PT_!
ICE is an amazing language, despite what some might say against :P
PT_++ ICE++


--STUFF INCLUDED (REQUIRED)--
"ICYCRAFT.8xp" The game executable
"ICYtxp00.8xv" The default texture pack
"ICYbvr00.8xv" The default behavior pack
NOTE: The appvars are optional if you have another texture/behavior pack you want to use.
      Make sure you update all of your texture/behavior packs for every update!
      If you are planning on using a mod, make sure there is a texture pack and a behavior pack.
      Otherwise you will not be able to play the game. IcyCraft will tell you what is missing if you try.


--EXTRA STUFF (OPTIONAL)--
"ICYtxp01.8xv" The second texture pack
"ICYtxp02.8xv" The third texture pack


--MAIN MENU--
Press [y=] to play in creative mode.
Press [2nd] to play in survival mode.
Press [del] to remove all data from the selected world.

Press [zoom] to change the selected world (first 6 characters of the desired map file)
Press [trace] to change the texture pack
      This will prompt for an appvar name.
Press [graph] to change the behavior pack
      This will prompt for an appvar name.
NOTE: Characters in the input are the same as the keypad, with extra characters here and there.
      An appvar that doesn't exsist will not be accepted, and the pack will not change.
      The current packs and world are saved in the appvar "ICYpacks", so you won't have to input them every time.


--HOW TO PLAY--
Use the arrow keys to move around, and select break/place position
[y=] Upward break
[2nd] Downward break
[alpha] Upward place
[math] Downward place
[XTthetaN] Lock/Unlock player movement. Useful for placing in adjacent tiles.
[mode] Open inventory
Run into an interactable tile (like a chest, furnace, or crafting table), to interact with it.
[trace],[graph] change selected hotbar item
NOTE: any key can be pressed in any combination in the main game view.
NOTE: upward/downward placing certain tiles determines what it will look like and do when placed.
NOTE: Holes will move the player down.


--GAME HUD--
"holding x##" the block/item you are currently holding in your active hotbar slot and the amount.
"looking at" the block you are currently pointing to.
"(block)" the block you are currently standing on.
The hearts are your health.
The screen will flash red as you take damage.
"x###,y###,z###" your current position in the world. X,Z are E/W, S/N. Y is up/down.


--SURVIVAL MODE--
In this game mode, there is hunger; which saps the player's health.
You will eventually die and respawn if you don't eat.
Respawn happens immediately.
[window] Eat the currently selected hotbar item if it is edible.


--CREATIVE MODE--
No hunger in this mode
[+],[-],[*],[/] Creative inventory pages


--INVENTORY/CHEST--
Arrow keys move cursor
[2nd],[enter] select two items to switch
NOTE: this will combine items if they are the same, and switch them otherwise.
[clear],[mode] exit inventory/chest
INVENTORY ONLY:
[XTthetaN] open crafting menu


--CRAFTING/FURNACE--
Up/Down arrows select recipe to craft
[2nd],[enter],[y=] craft recipe (only works if you have the items for it)
[graph] craft 64. (will craft until there is 64 or more of the item)
[XTthetaN],[clear] exit crafting
[mode] exit crafting and inventory


--CHANGELOG--
v2.12.0:
* Added Mesa biome and 3 colors of terracotta
* Added Cobble maker: produces cobble and stores it like a chest.
* Added Harvester: produces grain if adjacent to wheat, logs if adjacent to a log, and apples if adjacent to leaves.
* Added Grain Funnel: crafts wheat from grain stored in the container directly North of it.
* Added hoppers, but they don't do anything right now, other than act like chests.
* Tweaked the world generator
! The new item-moving/producing blocks have an effect on framerate, but only when in the player view.
! All container data is stored in one variable. Use containers wisely. Maximum ~850 chests can be in a world.
! There is still a bug with overworld structures spawning underground.

v2.11.0:
* Added FPS meter
* Added "looking at"
* Added "x##" to the selected item name display
* An optimization or two
* Added display of the behavior/texture pack appvar names in the main menu
+ IcyCraft now runs between 10 and 24 FPS! :D

v2.10.2:
* Combined the two behavior pack appvars. Now you'll only need the one!
* Added another texture pack
* The crafting menu will now scroll past the items for cannot craft.
  Finding the recipe you want has never been easier! :D
* Other minor optimizations
* Some internal changes to allow for more crafting methods!

! There is currently a bug with overworld structures spawning underground.
  I hope to fix this in the near future

v2.10.0: Fifth release:
* Added support for multiple worlds
* Added texture and behavior pack switching
* Changed some things with overworld generation
* Added 3 new structures
* Made hunger act a lot slower
* Changed damage graphic to a red flash. More noticeable.
* Fixed problem with the edge of the world looping to an invalid coordinate.
  I didn't think anyone would get that far... but I did.

v2.9.1-2: Hotfix:
* Forgot to add the recipe for bread

v2.9.1: Fourh release:
* Added biomes and structures!
* Added eating and hunger
* Added creative mode
* Added bread
* Fixed some block placement and block breaking bugs
* Removed inventory editor program (it's now part of the actual game)

v2.8.3: Third release:
* Added 4 new ores, along with their items and blocks.
* Added Hard cobble, and Red cobble.
* Added Hay bales
* Added inventory editor program.
* Added Insta-Pick (only avalible through the inventory editor)

v2.4: Second release:
* Fixed chest creation occasionaly crashing
* Fixed new chests reading the same data as the previous one initialized
* Added Block Updates!
* Added tall grass (I know, it looks like a melon :P )
* Added wheat, seeds, and grain.
* Added tree saplings, that grow logs, and bush saplings, that grow leaves.
* Doubled the number of apples dropped from leaves.
* Added quartz, quartz blocks, and chiseled quartz
* Added carved logs, chiseled stone bricks, and sandstone

v2.1: Hotfix:
* Fixed concrete not dropping when broken

v2.0: Beta testing part 2:
* Fixed resetting all chests upon a crash.
* Fixed placing the same block in the same place still removing the item from the inventory.
* Placing a block in a tile that has a droppable block will now give the player that block.
* Changed block placing/breaking keys. They now use the same keys as movement
* Made any block ID placeable, as long as it is placeable.
* Added Coal, Iron, Gold, Lapis, Redstone, and Diamond blocks
* Added White, Black, Red, Blue, Light Blue, and Purple concrete
* Added gold nuggets and crafting them to ingots
* Added Crafting recipes for block->item and item->block for mineral blocks
* Added Furnace recipes for dirt->sand and gravel->gold nugget and sand->diamond and coal block->diamond
* Fixed some grammar/spelling errors in the README

v1.0: Initial beta tests


And thanks to all the troopers who read this README! It is much appreciated when all this text doesn't go unappreciated :P

