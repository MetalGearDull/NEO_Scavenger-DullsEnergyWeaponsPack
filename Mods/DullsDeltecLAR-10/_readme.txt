How to Mod NEO Scavenger
========================
There are two types of mods in NEO Scavenger:

1 - New content
2 - Override content

New content is anything you want to add that does not already exist in the game. This content will just get added on to the list of existing content when the game is loaded.

Override content is for changing original game data. If you want to tweak hunger penalties, dogman stats, and other existing data, this is where you'd do that.

For both types of mods, you'll need to add your mod's name and URL to the getmods.php file, like so:

nRows=2&
&strModName0=SampleMod
&strModURL0=SampleModFolder
&strModName1=0
&strModURL1=SampleModFolder/0

The above lines will add two mods. The first, "SampleMod," can be found in the folder "SampleModFolder." The second, mod "0," is an override mod in a folder with the same name. "0" (note: that's number zero, not letter O) is a special ID used by the game to denote original game data. The name is important to the game, but you can call the folder anything you want.

The above "SampleMod" and "0" override data are provided in this download as an example. Simply replace the getmods.php with the provided SampleModFolder/getmods.php and then reload the game to see it in action. 

"SampleMod" and "0" adds a new "fancy shopping bag" to the default cryo hex loot. The new bag item is in "SampleMod," while the adjusted cryo hex loot values are in "0."

Also, if you're interested in seeing the game's start-up log messages. They are automatically copied to the clipboard as they appear. So if you open a text editor and paste after the game loads, you'll see the loading messages in their entirety. This is essential when debugging your mod!

For more information, check out the official modding forum:
http://bluebottlegames.com/main/forum/10

There are many tips and helpful folks there!