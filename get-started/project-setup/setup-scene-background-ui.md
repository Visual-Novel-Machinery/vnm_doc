---
layout: default
title: Setting up the Scene Background UI
parent: Project Setup
grand_parent: Get Started
nav_order: 6
---

# Setting up the Scene Background UI
1. Go to the Blueprint folder into the folder UI, and in there in the folder called InGame
2. Create a blueprint class that is based on BaseSceneBackgroundDisplayWidget and call it W_SceneBackgroundDisplayWidget.
    1. Open the widget
    2. Design the widget however you like
        - Add a image block to the widget named SceneBackgroundImage.
        - Add a image block to the widget named SceneBackgroundImageForTransition.
3. Open the blueprint BP_InGameHud.
    1. Select the component Dialog Image Controller
    2. In the settings of the component set the Scene Background Display Widget Class to W_SceneBackgroundDisplayWidget

Everytime a scene background is displayed, the above created widget will be used to display the scene background. If you intend to always display something additional with a scene background, this can be used to set this up as well.

Next up is [setting up the player interaction]({{ site.baseurl }}{% link get-started/project-setup/setup-player-interaction.md %}), so that a player can navigate through the story with keyboard/gamepad input.