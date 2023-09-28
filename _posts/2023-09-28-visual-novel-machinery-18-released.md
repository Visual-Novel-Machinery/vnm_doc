---
layout: posts
title:  "Visual Novel Machinery 1.8 Released"
excerpt: Visual Novel Machinery 1.8 has been released
categories:
  - release
tags:
  - release
---

Changelog:
- Added Cg Play Animation Node
- Added Scene Background Play Animation Node
- Added Character Play Animation Node
- Added Dialog Window Play Animation Node
- Character Hide Node Button in the VNM Tab will now actually spawn a character hide node and not a character show node
- Beta: Integrated support for importing yarnspinner yarn files and generate dialog blueprints from them
	- You need to download the yarn spinner console (ysc.exe) and set the path to it in the VNM Yarn Editor Setting found in Project Settings -\> Plugins
		- https://github.com/YarnSpinnerTool/YarnSpinner-Console/releases
	- Create a blueprint from the class YarnFunctionBlueprintLibrary to create your own yarn functions
		- These functions need to use an output parameter named "ReturnValue" and can only be of type boolean/string/float
		- Input parameters can only be boolean/string/float
		- Set the blueprint in VNM Yarn Settings to make sure it is found
	- Create a blueprint from the class YarnCommandBlueprintLibrary to create your own yarn commands
		- These functions or events should not have any return value
		- Input parameters can only be boolean/string/float
		- Set the blueprint in VNM Yarn Settings to make sure it is found
	- It does not support the \<\<jump \<node name\>\>\> command, if the node is not inside the same yarn file
	- Special commands for your yarnspinner scripts that spawn the equivalent VNM node when importing the yarn script:
		- Dialog Nodes:
			- \<\<dialog window \<should hide (true/false)\> \<set to automatic (true/false)\> \[\<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\>
			- \<\<dialog widget show \<widget blueprint name (ex: W_TestWidget)\> \[\<Wait for widget to close again (true/false)\>\] \>\>
			- \<\<dialog widget hide \<widget blueprint name (ex: W_TestWidget)\> \>\>
			- \<\<dialog memory get \<dialog id\> \<memory id\> \<variable name to save the memory value to (\$\<variablename\>) \>\>\>
			- \<\<dialog memory set \<dialog id\> \<memory id\> \<variable name to save the memory value to (\$\<variablename\>) \>\>\>
		- Character Nodes:
			- \<\<character show \<character id\> \<emotion id\> \[\<character positioning\> \<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\>
			- \<\<character hide \<character id\> \[\<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\>
			- \<\<character move \<character id\> \<character positioning\> \[\<MoveWithAnimation (true/false)\] \>\>
			- \<\<character rename \<character id\> \<new character name\> \>\>\>
			- \<\<character rename interactive \<character id\> \>\>\>
			- \<\<character layer add \<character id\> \<layer id\> \<image id\> \>\>\>
			- \<\<character layer remove \<character id\> \<layer id\> \>\>\>
			- \<\<character memory get \<character id\> \<memory id\> \<variable name to save the memory value to (\$\<variablename\>) \>\>\>
			- \<\<character memory set \<character id\> \<memory id\> \<variable name to save the memory value to (\$\<variablename\>) \>\>\>
		- Character 3D Nodes:
			- \<\<character3D show \<character id\> \<emotion id\> \<dialog scene id\> \<spawn location\> \>\>
			- \<\<character3D hide \<character id\> \>\>
		- CG Nodes:
			- \<\<cg show \<cg id\> \[\<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\>
			- \<\<cg hide \[\<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\>
			- \<\<cg layer add \<cg id\> \<layer id\> \<image id\> \>\>\>
			- \<\<cg layer remove \<cg id\> \<layer id\> \>\>\>
		- Scene Background Nodes:
			- \<\<scenebackground show \<scenebackground id\> \[\<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\>
			- \<\<scenebackground hide \[\<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\>
			- \<\<scenebackground layer add \<scenebackground id\> \<layer id\> \<image id\> \>\>\>
			- \<\<scenebackground layer remove \<scenebackground id\> \<layer id\> \>\>\>
		- Dialog Scene Nodes:
			- \<\<dialogscene show \<dialog scene id\> \<camera name\> \>\>
			- \<\<dialogscene hide \>\>
			- \<\<dialogscene camera \<dialog scene id\> \<camera name\> \[\<DontWaitForTransitionToFinish (true/false)\>\] \>\>
		- Audio Nodes:
			- \<\<audio play bgm \<background music id\> \[\<volume\> \<pitch\> \<start time\> \<WaitForAudioToFinish (true/false)\> \<IsLooping (true/false)\>\] \>\>
			- \<\<audio play sfx \<sfx id\> \[\<volume\> \<pitch\> \<start time\> \<WaitForAudioToFinish (true/false)\>\] \>\>
			- \<\<audio play charactervo \<character id\> \<voice over id\> \[\<volume\> \<pitch\> \<start time\> \<WaitForAudioToFinish (true/false)\>\] \>\>
			- \<\<audio play dialogvo \<dialog id\> \<voice over id\> \[\<volume\> \<pitch\> \<start time\> \<WaitForAudioToFinish (true/false)\>\] \>\>
			- \<\<audio stop bgm \>\>
			- \<\<audio stop sfx \>\>
			- \<\<audio stop vo \>\>