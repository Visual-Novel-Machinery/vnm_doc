---
layout: single
title: Setting up the Character UI
permalink: /docs/project-setup/setup-character-ui/
toc: true
sidebar:
  nav: "docs"
---


1. Go to the Blueprints folder into the folder UI, and in there in the folder called InGame
2. Create a blueprint class that is based on BaseCharacterDisplayWidget and call it W_CharacterDisplayWidget.
    1. Open the widget
    2. Design the widget however you like
        - Add a canvas panel to the widget named CharacterCanvas.
        - Add a image block as a child of CharacterCanvas named CharacterImage.
3. Open the blueprint BP_InGameHud.
    1. Add the component Character Controller
    2. In the settings of the component set the Character Display Widget Class to W_CharacterDisplayWidget

Everytime a new character is spawned, the above created widget will be used to display the character. If you intend to always display something additional with a character, this can be used to set this up as well. An example would be that you display only character portraits in the visual novel. You could then setup the border of the portrait in here as well.

Next up is [setting up the CG UI]({{ site.baseurl }}{% link docs/project-setup/setup-cg-ui.md %}).