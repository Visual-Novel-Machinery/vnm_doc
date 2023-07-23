---
layout: posts
title:  "Visual Novel Machinery 1.6 Released"
excerpt: Visual Novel Machinery 1.6 has been released
categories:
  - release
tags:
  - release
---

Changelog:

- Made plugin compatible with Unreal Engine 5.2
- Added feature to rename characters during a dialog sequence
	- Use $c$\<characterid\>$ in your dialog texts to replace it with the character name. This will replace it with the original name or the name the player chose
	- Rename the character without player interaction using the Character Rename Node
	- Rename the character with the player deciding using the Character Interactive Rename Node
- When overwriting a save slot, the player will get a pop up displayed to ensure they are not overriding on accident. This can be disabled in the VNM Settings
- Added the ability for the player to rename the save file. If this is disabled then the save file will get a generated name
- There is now the ability to delete a save file again
- Save slots are now dynamically created, meaning you can now have an infinite amount of save slots. If there are more save slots than displayed then the save ui can now go to a second/third/... page to display the additional save slots
- Added support for a gallery system
	- To make the cg appear in the gallery, give it a cg group id
	- If multiple cgs have the same cg group id, then they will be part of the gallery display slot. This means when the player clicks on the cg, the cgs will be displayed one after another
	- gallery system supports paging as well