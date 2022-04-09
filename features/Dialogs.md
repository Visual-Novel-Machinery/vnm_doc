---
layout: default
title: Dialog System
parent: Features
nav_order: 1
---

# Dialog System
Dialogs in the Visual Novel Machinery are created by creating a Dialog Blueprint in the editor.

To create a dialog blueprint, right-click in the content browser in a folder of your choice and select "Dialog Blueprint" in the VNM category.

## Anatomy of a Dialog
A dialog generally consists of a beginning and an end. What is important is that there can only ever be one start point, but infinite endings for a dialog object.

![Base Dialog Anatomy]({{ site.baseurl }}/assets/images/DialogSystem/BaseAnatomy.png)

The start point of the dialog is represented in the Graph Editor with the [Dialog Start Node]({{ site.baseurl }}{% link nodes-reference/dialog-start.md %}). 

An ending is represented in the Graph Editor with the [Dialog End Node]({{ site.baseurl }}{% link nodes-reference/dialog-end.md %}). If a dialog sequence does not end with a [Dialog End Node]({{ site.baseurl }}{% link nodes-reference/dialog-end.md %}), then the dialog will just halt at this point and never end. Additionally, if you don't select a follow-up dialog, then Visual Novel Machinery will send the player to the Main Menu Level specified in the project settings.

Between the start and the end, you can add all of the nodes.

## Basics - Linear Dialog
The most basic node that you will always need with a Dialog System is a node to display text. For this the Visual Novel Machinery offers the [Dialog Text Node]({{ site.baseurl }}{% link nodes-reference/dialog-text.md %}). In its most basic form, this node will display a text on screen in the dialog box. The text specified in the node is of data type Text, meaning they can be localized.

However, this is most likely not enough. The node can also display the name of the character talking. To have characters available for selection, you'll need to add a character to the Character Definitions Data Table that is set in the project settings. In there you can specify the display text and color of the text. the other settings are for now not important to us. For more details on those, check the [character feature documentation]({{ site.baseurl }}{% link features/characters.md %}).

Now add multiple [Dialog Text Node]({{ site.baseurl }}{% link nodes-reference/dialog-text.md %}) in sequence, and you have created a simple short linear dialog using Visual Novel Machinery.

![Linear Dialog Example]({{ site.baseurl }}/assets/images/DialogSystem/LinearDialog.png)

## Basics - Branching Dialog
Sometimes a linear story is not enough and you want to go ahead and branch it with user choices. For this the dialog system supports player choices. These can be created using [Dialog Choice Nodes]({{ site.baseurl }}{% link nodes-reference/dialog-choice.md %}). To add choices to it, click on the node and specify them in the Details Panel. The most basic choice could be a yes/no or up/down choice. It is up to you to decide which options the player has. These options will then be displayed as buttons for the user to click. Each choice added is internally of data type Text, meaning they can be localized.

![Branching Dialog Example]({{ site.baseurl }}/assets/images/DialogSystem/BranchingDialog.png) 

But, sometimes the player has to work for certain choices to be available. For this reason the [Dialog Choice Node]({{ site.baseurl }}{% link nodes-reference/dialog-choice.md %}) supports making all choices conditional. This means only if a certain condition is met, then the choice is displayed to the player. For example, if the player hasn't opened a door, then the choice to close it would be hidden. Alternatively, if the player has already viewed something, then the option to view the object is hidden.

![Branching Dialog Example with Conditions]({{ site.baseurl }}/assets/images/DialogSystem/BranchingDialogConditional.png) 

## Advanced - Dialog Window Controls
From time to time it can happen that you want to do something special with the dialog window. For this reason there is a [Dialog Window Control Node]({{ site.baseurl }}{% link nodes-reference/dialog-window-control.md %}). This node can be use to play animations on the window widget, or to hide and show it. In general if the node is never used, then the dialog window is set to automatic mode, meaning it will automatically show at the beginning of the dialog, or hide at the end of the dialog. This could be useful for example if your character becomes deaf during a dialog sequence, and therefore you want to hide the dialog box.

## Advanced - Dialog Text Stylization
There might potentially be a need that you want to highlight part of the text in a different color. For this reason the plugin uses a RichTextBlock in the UI. With this you can use tags like **\<green\>\</\>** as an example. To create these tags, the blank project template has a data table called DT_DialogTextStyling. In this data table it is possible to create these tags for styling the dialog text. Unreal Engine offers also the usage of RichTextBlockDecorators that can be used to do even more customization, like displaying images in text. This however is not setup by default in the project template.

![Dialog Text Stylization Example]({{ site.baseurl }}/assets/images/DialogSystem/TagSystem.png) 