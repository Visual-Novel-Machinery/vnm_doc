---
layout: single
title: Yarn Spinner
permalink: /docs/integrations/yarn-spinner
toc: true
sidebar:
  nav: "docs"
---

If the node-based approach is nothing for you, then you can also use Yarn Spinner to write you visual novels, and then import the yarn files.

## Basics

If you want to use yarn, the language used for Yarn Spinner, you can check out the docs [here](https://docs.yarnspinner.dev/getting-started/writing-in-yarn).

This documentation will only explain the special extras that you can use in yarn spinner to generate Visual Novel Machinery specific nodes.

Writing dialog, choices, and using variables is integrated out of the box. For all the other nodes, they can be created using commands in yarn spinner.

## Commands

The following commands spawn the following Visual Novel Machinery Nodes:

### Dialog Nodes

| Node | Command |
| --- | --- |
| [Dialog Window Node]({{ site.baseurl }}{% link docs/nodes-reference/dialog-window-control.md %}) | \<\<dialog window \<should hide (true/false)\> \<set to automatic (true/false)\> \[\<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\> |
| [Dialog Widget Show Node]({{ site.baseurl }}{% link docs/nodes-reference/dialog-widget-show.md %}) | \<\<dialog widget show \<widget blueprint name (ex: W_TestWidget)\> \[\<Wait for widget to close again (true/false)\>\] \>\> |
| [Dialog Widget Hide Node]({{ site.baseurl }}{% link docs/nodes-reference/dialog-widget-hide.md %}) | \<\<dialog widget hide \<widget blueprint name (ex: W_TestWidget)\> \>\> |
| [Dialog Memory Get Node]({{ site.baseurl }}{% link docs/nodes-reference/dialog-memory-get.md %}) | \<\<dialog memory get \<dialog id\> \<memory id\> \<variable name to save the memory value to (\$\<variablename\>) \> \>\> |
| [Dialog Memory Set Node]({{ site.baseurl }}{% link docs/nodes-reference/dialog-memory-set.md %}) | \<\<dialog memory set \<dialog id\> \<memory id\> \<variable name to save the memory value to (\$\<variablename\>) \> \>\> |

### Character Nodes

| Node | Command |
| --- | --- |
| [Character Show Node]({{ site.baseurl }}{% link docs/nodes-reference/character-show.md %}) | \<\<character show \<character id\> \<emotion id\> \[\<character positioning\> \<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\> |
| [Character Hide Node]({{ site.baseurl }}{% link docs/nodes-reference/character-hide.md %}) | \<\<character hide \<character id\> \[\<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\> |
| [Character Move Node]({{ site.baseurl }}{% link docs/nodes-reference/character-move.md %}) | \<\<character move \<character id\> \<character positioning\> \[\<MoveWithAnimation (true/false)\] \>\> |
| [Character Rename Node]({{ site.baseurl }}{% link docs/nodes-reference/character-rename.md %}) | \<\<character rename \<character id\> \<new character name\> \> \>\> |
| [Character Interactive Rename Node]({{ site.baseurl }}{% link docs/nodes-reference/character-interactive-rename.md %}) | \<\<character rename interactive \<character id\> \> \>\> |
| [Character Add Layer Node]({{ site.baseurl }}{% link docs/nodes-reference/character-add-layer.md %}) | \<\<character layer add \<character id\> \<layer id\> \<image id\> \> \>\> |
| [Character Add Layer Node]({{ site.baseurl }}{% link docs/nodes-reference/character-remove-layer.md %}) | \<\<character layer remove \<character id\> \<layer id\> \> \>\> |
| [Character Memory Get Node]({{ site.baseurl }}{% link docs/nodes-reference/character-memory-get.md %}) | \<\<character memory get \<character id\> \<memory id\> \<variable name to save the memory value to (\$\<variablename\>) \> \>\> |
| [Character Memory Set Node]({{ site.baseurl }}{% link docs/nodes-reference/character-memory-set.md %}) | \<\<character memory set \<character id\> \<memory id\> \<variable name to save the memory value to (\$\<variablename\>) \> \>\> |

### Character 3D Nodes

| Node | Command |
| --- | --- |
| [Character 3D Show Node]({{ site.baseurl }}{% link docs/nodes-reference/character-3d-show.md %}) | \<\<character3D show \<character id\> \<emotion id\> \<dialog scene id\> \<spawn location\> \>\> |
| [Character 3D Hide Node]({{ site.baseurl }}{% link docs/nodes-reference/character-3d-hide.md %}) | \<\<character3D hide \<character id\> \>\> |

### CG Nodes

| Node | Command |
| --- | --- |
| [CG Show Node]({{ site.baseurl }}{% link docs/nodes-reference/cg-show.md %}) | \<\<cg show \<cg id\> \[\<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\> |
| [CG Hide Node]({{ site.baseurl }}{% link docs/nodes-reference/cg-hide.md %}) | \<\<cg hide \[\<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\> |
| [CG Add Layer Node]({{ site.baseurl }}{% link docs/nodes-reference/cg-add-layer.md %}) | \<\<cg layer add \<cg id\> \<layer id\> \<image id\> \> \>\> |
| [CG Remove Layer Node]({{ site.baseurl }}{% link docs/nodes-reference/cg-remove-layer.md %}) | \<\<cg layer remove \<cg id\> \<layer id\> \> \>\> |

### Scene Background Nodes

| Node | Command |
| --- | --- |
| [Scene Background Show Node]({{ site.baseurl }}{% link docs/nodes-reference/scene-background-show.md %}) | \<\<scenebackground show \<scenebackground id\> \[\<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\> |
| [Scene Background Hide Node]({{ site.baseurl }}{% link docs/nodes-reference/scene-background-hide.md %}) | \<\<scenebackground hide \[\<transition event\> \<DontWaitForTransitionToFinish (true/false)\> \<CustomTransitionName\>\] \>\> |
| [Scene Background Add Layer Node]({{ site.baseurl }}{% link docs/nodes-reference/scene-background-add-layer.md %}) | \<\<scenebackground layer add \<scenebackground id\> \<layer id\> \<image id\> \> \>\> |
| [Scene Background Remove Layer Node]({{ site.baseurl }}{% link docs/nodes-reference/scene-background-remove-layer.md %}) | \<\<scenebackground layer remove \<scenebackground id\> \<layer id\> \> \>\> |

### Dialog Scene Nodes

| Node | Command |
| --- | --- |
| [Dialog Scene Show Node]({{ site.baseurl }}{% link docs/nodes-reference/dialog-scene-show.md %}) | \<\<dialogscene show \<dialog scene id\> \<camera name\> \>\> |
| [Dialog Scene Hide Node]({{ site.baseurl }}{% link docs/nodes-reference/dialog-scene-hide.md %}) | \<\<dialogscene hide \>\> |
| [Dialog Scene Switch Camera Node]({{ site.baseurl }}{% link docs/nodes-reference/dialog-scene-switch-camera.md %}) | \<\<dialogscene camera \<dialog scene id\> \<camera name\> \[\<DontWaitForTransitionToFinish (true/false)\>\] \>\> |

### Audio Nodes

| Node | Command |
| --- | --- |
| [Dialog Audio Play Background Music Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-play-bgm.md %}) | \<\<audio play bgm \<background music id\> \[\<volume\> \<pitch\> \<start time\> \<WaitForAudioToFinish (true/false)\> \<IsLooping (true/false)\>\] \>\> |
| [Dialog Audio Play Sound Effect Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-play-sfx.md %}) | \<\<audio play sfx \<sfx id\> \[\<volume\> \<pitch\> \<start time\> \<WaitForAudioToFinish (true/false)\>\] \>\> |
| [Dialog Audio Play Character Voice Over Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-play-character-voice-over.md %}) | \<\<audio play charactervo \<character id\> \<voice over id\> \[\<volume\> \<pitch\> \<start time\> \<WaitForAudioToFinish (true/false)\>\] \>\> |
| [Dialog Audio Play Dialog Voice Over Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-play-dialog-voice-over.md %}) | \<\<audio play dialogvo \<dialog id\> \<voice over id\> \[\<volume\> \<pitch\> \<start time\> \<WaitForAudioToFinish (true/false)\>\] \>\> |
| [Dialog Audio Stop Background Music Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-stop-bgm.md %}) | \<\<audio stop bgm \>\>> |
| [Dialog Audio Stop Sound Effect Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-stop-sfx.md %}) | \<\<audio stop sfx \>\>> |
| [Dialog Audio Stop Voice Over Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-stop-voice-over.md %}) | \<\<audio stop vo \>\>> |

### Custom commands

If you want to add custom commands you can do so by following the steps below:

1. Create a blueprint from the class YarnCommandBlueprintLibrary
2. Add a function to this blueprint called "MyCustomCommand"
3. Add any amount of string/float/boolean variables to the input parameters. For example: (boolean test1, float test2, string test3)
4. **Do not** add any output parameters.
5. Navigate to to Project Settings -> Plugins -> VNM Yarn Settings
6. Set the Yarn Command Library to your blueprint
7. Use your custom command in your yarn file. Using the above example the result would be: \<\< MyCustomCommand true 0.0 "test" \>\>

## Functions

The yarn spinner integration supports all functions found in this [documentation](https://docs.yarnspinner.dev/getting-started/writing-in-yarn/functions).

There are two exceptions: "visited" and "visited_count".

### Custom functions

If you want to add custom commands you can do so by following the steps below:

1. Create a blueprint from the class YarnFunctionBlueprintLibrary
2. Add a function to this blueprint called "MyCustomFunction"
3. Add any amount of string/float/boolean variables to the variable inputs. For example: (boolean test1, float test2, string test3)
4. You **need to** add one output parameter of type float called **ReturnValue**. The import of the yarn file will **fail**, if the output parameter is not called **ReturnValue**. Don't add more than one output parameter.
5. Navigate to to Project Settings -> Plugins -> VNM Yarn Settings
6. Set the Yarn Function Library to your blueprint
7. Use your custom function in your yarn file. Using the above example the result would be:

```
Cube: My custom function result is: {MyCustomFunction(true, 0.0, "test")}
```

## Important Notes

You **cannot** jump to nodes outside of the currently imported yarn file.

You **cannot** at the moment use the "visited" or "visited_count" function.

You need to **add** all the scene backgrounds/cgs/characters/memories to the definiton data tables before importing yarn, or Visual Novel Machinery will be confused, because it can't find the specified scene backgrounds/cgs/characters/memories in the definition data tables.