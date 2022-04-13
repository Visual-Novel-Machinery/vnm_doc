---
layout: default
title: Characters
parent: Features
nav_order: 5
---

# Characters

The core of every story are the characters. They make or break everything about a story. So what does Visual Novel Machinery offer in terms of characters?

First of all, characters need to be defined in the Character Definitions Data Table. Details about what is contained in a character definition can be found [here]({{ site.baseurl }}{% link data-definitions/character-definition.md %}). If the character is not added to that data table, it doesn't exist for the plugin.

The are two ways characters can be used in the Visual Novel Machinery, visual and non-visual. 

Non-visual means that we just have the name of the character in the dialog box. Nothing else is displayed for that character (Unless you are using CGs to display all moments of the story). You can also change the color of the character name displayed in the dialog box. It is the most basic form of using characters in Visual Novel Machinery. This type is already taken care of with the [Dialog Text Node]({{ site.baseurl }}{% link nodes-reference/dialog-text.md %}).

Visual means that the character themselves are displayed as images on screen. This also means that you can display the character in different emotional states. 

## Basics
There are two different ways of displaying a character. The first one is to use the [Character Show Node]({{ site.baseurl }}{% link nodes-reference/character-show.md %}). With this node you can select the character and the emotion of the character. An alternative option is to use the [Dialog Text Node]({{ site.baseurl }}{% link nodes-reference/dialog-text.md %}). This is the short-hand version to save on a node. You can also specify an emotion directly in this node, which will also show the character in that emotional state. If the character is already visible, both nodes with transition the character to a new emotional state.

Once a character is done talking you will also want to hide that character again. For this purpose the [Character Hide Node]({{ site.baseurl }}{% link nodes-reference/character-hide.md %}) exists. This node will hide the character of the specified character id. This is especially useful when having multiple characters on screen, and one of them leaves.

![Base Character System]({{ site.baseurl }}/assets/images/Characters/BaseCharacterSystem.png)

On that note, how would one deal with multiple characters on screen? Per default they would all spawn in the center of the screen on top of each other. For this there are multiple options on moving the characters. The first option for newly displayed characters is to move them by specifying the position of the character in the [Character Show Node]({{ site.baseurl }}{% link nodes-reference/character-show.md %}) or the [Dialog Text Node]({{ site.baseurl }}{% link nodes-reference/dialog-text.md %}). For characters that are already visible, it is also an option to use the [Character Move Node]({{ site.baseurl }}{% link nodes-reference/character-move.md %}). This one can move a character to the left/right/center/true-center.

![Character Movement System]({{ site.baseurl }}/assets/images/Characters/CharacterMovementSystem.png)

