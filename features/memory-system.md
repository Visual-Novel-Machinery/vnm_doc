---
layout: default
title: Memory System
parent: Features
nav_order: 6
---

# Memory System
Sometimes it is necessary for a character to remember something, or save a vaue to a scene, to check later what the main character chose to do in a specific scene. For this purpose Visual Novel Machinery offers the memory system. With this system you can save data specific for a character or scene and access it later on. The values that can be saved to a memory are in general primitive data types meaning:
- Boolean
- Integer
- Integer64
- float
- String
- Byte (for saving Enums)

These values can be get/set with their respective nodes. There are [Character Memory Get Node ]({{ site.baseurl }}{% link nodes-reference/character-memory-get.md %}) and [Character Memory Set Node ]({{ site.baseurl }}{% link nodes-reference/character-memory-set.md %}) for characters and [Dialog Memory Get Node ]({{ site.baseurl }}{% link nodes-reference/character-memory-get.md %}) and [Dialog Memory Set Node ]({{ site.baseurl }}{% link nodes-reference/character-memory-set.md %}) for dialogs. You can use these to access and modify the memory values for characters/dialogs. The node's value input/output pin will automatically adapt to the datatype of the selected memory when selecting it.

![Memory Nodes]({{ site.baseurl }}/assets/images/MemorySystem/MemoryNodes.png)

You can define a memory in the Character Definitions Data Table for characters or in the Dialog Definitions Data Table for dialogs. In there each dialog/character as an array field for configuring the memory values. Each memory value will need a memory id to clearly identify the memory. This id has to be unique. After adding it there, reopen your dialog blueprint and the nodes should find them.

![Memory Nodes]({{ site.baseurl }}/assets/images/MemorySystem/CharacterMemoryDefinitions.png)
![Memory Nodes]({{ site.baseurl }}/assets/images/MemorySystem/DialogMemoryDefinitions.png)


