---
layout: default
title: Dialog Scenes Graph
parent: Features
nav_order: 10
---

# Dialog Scenes Graph
Similar to the Choice Graph, you can show the player which scenes lead to which scene. It functions exactly the same as the Choice Graph. One important note here is that when clicking a scene node, the choice id given by the event is the name of the dialog as defined in the Dialog Definitions Data Table.

The Dialog Scenes Graph will start with the first row in the Dialog Definitions Data Table and will construct its visualization taking the first row as the starting point. It will parse all the Dialog Start Nodes and Dialog End Nodes to construct an accurate representation of the dialog scene sequence.