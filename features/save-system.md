---
layout: default
title: Save System
parent: Features
nav_order: 7
---

# Save System
Unless your story is really short, there comes the moment in a player's playthrough where they might want to take a break. As you don't want to them to lose their progress (if you want them to lose progress, skip this category), Visual Novel Machinery supports saving data for a playthrough, but also permanently in the persistant save file. This is then persistant over all playthroughs of your story.

## Player Save File
The player save file holds multiple pieces of information: character/CG/scene background currently displayed, Text currently displayed, choices currently display (if any), and all values for the memory system. It also saves all member variables in the currently running dialog blueprint, so that when you load the game the next time, it will restore the state of all member variables again on load, ensuring that the dialog continues properly.

But this doesn't have to be the only data that can be saved into it. You can easily extend the data that is saved to it by creating a blueprint using the UVNMBaseSaveGame class as its parent. After you have created the blueprint, make sure you override the default blueprint class in the project settings. For this navigate to Project Settings -> Plugins -> Visual Novel Machinery. There set the Save Game Class to your created class, in this case BP_VNMExampleSaveGame. In this blueprint you can now add variables that you can write on saving/read on loading.

![Player Save File]({{ site.baseurl }}/assets/images/SaveFile/Overriden_Save_File_Project_Settings.png)

To save or load the game, Visual Novel Machinery offers the Game Save Subsystem. This subsystem can be found in the blueprint editor in the node browser, simply search for "Game Save Subsystem". 

To save the player data there are two steps necessary. The first step is a call to the Prepare Save Game Object, which will prepare the save game object for you so you can add in your values, which you defined in your custom save game. After you have written your variable, you can now call the Save Game function, which will save your data and the plugin's save data to the save file on the disk.

To load the player data, you simply have to call the Load Game function from the Game Save Subystem. After this the save file gets loaded into the subsystem. After the loading is complete travel to your InGame Map. After traveling to your InGame map, all the controllers will take the save file data from the subsystem and return the player to their last known point in the story. If you have customized the save file data, you can also get the save game from the Game Save Subsystem in the InitializeComponent function to set up your components.

This system has been implemented to be triggered in the InGameController (Save/Load), and also in the W_MainMenuWidget when pressing the Load Game button in the Blank Project Template.

![Player Save File]({{ site.baseurl }}/assets/images/SaveFile/Example_Load_Save.png)

## Persistant Save File
The persistant save file is used to save data peristantly over all playthroughs. You could for example use this to display a different background in the main menu, depending on where the player currently is in the storyline. You can easily extend the data that is saved to it by creating a blueprint using the UVNMBasePersistantSaveGame class as its parent. After you have created the blueprint, make sure you override the default blueprint class in the project settings. For this navigate to Project Settings -> Plugins -> Visual Novel Machinery. There set the Persistant Save Game Class to your created class, in this case BP_VNMExamplePersistantSaveGame. In this blueprint you can now add variables that you can write on saving/read on loading.

![Persistant Save File]({{ site.baseurl }}/assets/images/SaveFile/Overriden_Save_File_Project_Settings.png)

The persistant data is automatically loaded into the Game Save Subsystem on starting the game. It will always hold the most up to date version of the data. If you want to write new values to the persistant save file, you can get the Persistant Save Game variable from the Game Save Subsystem and modify it. After modification make sure you call the "Save Peristant Data" function. Otherwise it is not saved to file, which means at the next game start up you changes are not there.