---
layout: default
title: Creating your first dialog
parent: Get Started
nav_order: 3
---

# Creating your first dialog

The dialog blueprints are the core of the Visual Novel Machinery plugin. They make everything work. Compared to many other visual novel solutions, Visual Novel Machinery uses a node-based approach to creating branching dialogs.

One important thing is, that the dialog blueprint still allows you to call other blueprint functions, meaning you are able to for example increment a player score during a dialog.

## Setting up the dialog blueprint
1. Navigate to the Dialogs folder in your project.
2. Right-click in the content browser, navigate to the VNM category, and select Dialog Blueprint.
3. Name the blueprint DI_MyFirstDialog.
4. Open the dialog blueprint.
    - As you can see, the dialog blueprint editor is very similar to the normal blueprint editor with a small difference. The toolbar at the top center includes a few more buttons. These spawn a node of that type right behind the last added node.
    - An other option to spawn the Visual Novel Machinery Nodes is using the same way as spawning other nodes, right-clicking in the Event Graph and searching for them.
    - **IMPORTANT:** A dialog blueprint may only have one Event Graph and one [Dialog Start Node]({{ site.baseurl }}{% link nodes-reference/dialog-start.md %}). Adding more will break the system.
5. Add a [Dialog Text Node]({{ site.baseurl }}{% link nodes-reference/dialog-text.md %}).
    - Leave the character as None for now. In general you shouldn't be able to select a character yet, unless you set some up in the DT_CharacterDefinitions data table.
    - Set the Text field to "Hello World!"
6. A dialog is only counted complete, when the [Dialog End Node]({{ site.baseurl }}{% link nodes-reference/dialog-end.md %}) is called. So add one [Dialog End Node]({{ site.baseurl }}{% link nodes-reference/dialog-end.md %}).
7. Connect all execution lines.
8. Compile the dialog blueprint.
9. Save the dialog blueprint.
10. Navigate to the DT_DialogDefinitions data table and open it.
11. Add a new row to the data table.
    - Set the row name to my-first-dialog
    - Set the dialog id to my-first-dialog. **IMPORTANT**: Row name and dialog id need to be the same.
    - Set the dialog object class to DI_MyFirstDialog.
12. Ensure that the first row is the row you just created in case there is already a row in the data table. In general, unless loading a save game, the game will start with the first dialog blueprint in the data table.
13. Save DT_DialogDefinitions
14. Open the InGame Map.
15. Press Play
16. You should now see your "Hello World!" message on screen. Once pressing the next dialog button, the dialog will end and navigate to your main menu level.

**Congratulations! You have created your first dialog.**

You can now move on to the features documentation and add in the [features]({{ site.baseurl }}{% link features/index.md %}) that you need. 

