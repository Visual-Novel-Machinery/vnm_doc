---
layout: single
title: Choice Graph
permalink: /docs/features/choice-graph
toc: true
sidebar:
  nav: "docs"
---


When you have a game with a lot of branches, you might want to show the player which branches they might have missed in the game. For this purpose Visual Novel Machinery offers a Choice Graph. It basically shows the player in a graph all choices in a specific dialog scene. To ensure that the player will not get spoilered too much the widget will only show the choice texts of choices the player has seen in the game. In the widget designer it will always display all choice texts.

To use this feature make sure you click the "Build Choice Data" Button in the Dialog Blueprint Editor, to ensure that the data has been built for display later on.

![Choice Graph Example]({{ site.baseurl }}/assets/images/ChoiceGraph/ChoiceGraph.png)

## Setup
1. Create a new widget and call it W_ChoiceWidget.
2. Add a scroll box to the widget
    - Set the Orientation Field to Horizontal in the Scroll category
    - Set the Consume Mouse Wheel option to never
    - Set the Scroll Bar Visibility to collapsed (Optional)
3. Add a scroll box to the previously added scroll box as a child
    - Set the Orientation Field to Vertical in the Scroll category
    - Set the Consume Mouse Wheel option to never
    - Set the Scroll Bar Visibility to collapsed (Optional)
4. Add the choice graph found in the VNM category in the Palette to the scroll box added in Step 3.

## Customization
The choice graph widget allows a wide range of customizations, to make it looks just the way you want it to look. It also supports multiple different types of nodes that can be customized:
- Choice
    - The choice a player can make in the game
- Branch
    - A branch node in default Unreal Engine blueprint. If both execution lines of the branch node lead to the same next node, it will not be displayed in the choice graph.
- End
    - An end in the dialog scene
- Start
    - The start of the dialog scene
- Loop Portal Start
    - If your dialog has rather complex loops in the story, the choice graph will display a node to signal the beginning of a portal leading to a previous position. It has the same color as the end portal node.
- Loop Portal End
    - If your dialog has rather complex loops in the story, the choice graph will display a node to signal the exit of a portal leading to a previous position. It has the same color as the beginning portal node.
- Scene
    - A node displaying that there is a sub dialog occuring in this dialog.

The following options can be customized:
- Font of the Choices Text
- Outline of the Choices Text
- Customization of the visualization of the different nodes mentioned above.
- Layout of the nodes displayed
    - Margin
    - Padding
- Style of the connection lines
    - Line Thickness
    - Line Color
    - Line Outline
    - Line Outline Color
    - Line Shadow
    - Line Shadow Offset
    - Line Shadow Color

## Events
The choice graph also allows clicking on choices. If a player clicks on a choice an event is triggered, to which you can react inside the previously created widget. This could be used to display additional information when clicking on a choice node, or to make the choice graph swith to a different scene because the pressed node is a scene node.