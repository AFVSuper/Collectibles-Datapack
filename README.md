![Collectibles Header (Default and 4 different customizations)](https://cdn.modrinth.com/data/cached_images/b34a517a85634a9acfa268511db6767d3c939bca.png)
# Collectibles Datapack
This datapack adds customizable collectibles for servers or lobbies for example. Each player can collect them.<br>
You can hide them or turn them into parkour objectives.<br>
There is also a ScoreBoard that shows each player collectibles.<br>
When a player collects one, a title is displayed to show how much progress has been made, showing how many collectibles they have found and how many exist.<br>
![Title image (With Purple Text Palette)](https://cdn.modrinth.com/data/cached_images/f1bd95154c5cfb10b18ee861124063abedf9daef.png)<br>
_(This title is not default, it is the Purple Text Palette preset)_

# How to use the Datapack
The first step after you enable the datapack in game is to perform this command: ``/function collectibles:setup``
This will enable other functions and features.<br><br>
After this you can access the items with: ``/function collectibles:adminitems``<br>
![Ingame Admin Items image](https://cdn.modrinth.com/data/cached_images/3412688c34350a640d72896840171e1c09256ebd.png)<br><br>
The first item is the Collectible Spawner. It will spawn a collectible on the block you use it.<br><br>
The second one is the Collectible Remover. It removes all collectibles around the block you use it. **IMPORTANT: If you remove a collectible, but someone already found it, the max number of collectibles is lowered by 1 but the player who had found it will retain the point.**<br><br>
The third item is the Cutomization Guide, with some explainations on how to customize the collectibles skin and particles.

## Some useful Functions and Commands
### ScoreBoard
The ScoreBoard can be activated with the command ``/scoreboard objectives setdisplay sidebar Collectibles``<br>
If you are familiar with commands you can modify how the scoreboard looks using them.<br>
The default appearance:<br>![Default Scoreboard](https://cdn.modrinth.com/data/cached_images/030205d9549a9f1353500f494ea8facdc5eab3ce.png)
### Reset Collectibles
Using ``/function collectibles:resetcolls`` you can delete all Collectibles, but only the ones that are in charged chunks due to Minecraft limitations and as happens when you use the remover, the players' points are not removed, so only use this if you know what you are doing.<br>
![All Collectible Remove (Text in image: All collectibles THAT WERE INSIDE CHARGED CHUNKS were removed)](https://cdn.modrinth.com/data/cached_images/2a66dd4a6119c88a1492921345baea6ba944c1ea.png)
### Reset Player Collectibles
Using ``/function collectibles:resetplayercolls`` you can delete all ONLINE players' Collectibles points making it possible to get the ones they already got. This is a testing feature and I do not recommend using it, but if you know how to do it without problems, it exists.<br>![Player Collectible Reset (Text in image: All collectibles were removed to ONLY the current online players.)](https://cdn.modrinth.com/data/cached_images/55beb32ac0a43503aebbf6e9513c1ad785c8dbbf.png)
### Uninstall
If you want to disable this datapack, I recommend using the command ``/function collectibles:uninstall``. This function removes the ScoreBoards and some data before disabling the datapack with ``/datapack disable "file/Collectibles-V1.0.zip"`` (maybe the datapack name changes)
# Collectible Customization
With the Customization Guide you can change the skin, particles and text colors. The book has explanations on how to do it and some presets. Anyways, I see how the complete customization of the skin is the most difficult part to understand, so here is an explanation with images:
### Skin/Head Full Customization
If you want to use a head from [Minecraft Heads](https://minecraft-heads.com) you first have to choose a head, (for example this Carved Pumpkin):<br>![Carved Pumpkin Head Photo](https://cdn.modrinth.com/data/cached_images/e906d578f340363481621bdde71ad1b49d6dc00a.png)<br>
Then you need to find at the bottom the "Value" of the head in the "For Developers" section:<br>![Head Value Photo](https://cdn.modrinth.com/data/cached_images/560ff3d5bf251d4c497df9e5489920e911ebdf64.png)<br>
That is the text you have to copy and then paste in the next command replacing <value>:<br>
``/data merge storage collectibles:id {HeadValue:"<value>"}``<br>
After this, all the collectibles should have this head as the skin.<br>![Custom Carved Pumpkin Collectible](https://cdn.modrinth.com/data/cached_images/acf85dc4840bef9f44f3c3d7802c7a5dc8fd49d6.png)
