---
layout: default
title: Setting up the Dialog UI
parent: Project Setup
grand_parent: Get Started
nav_order: 3
---

# Setting up the Dialog UI
1. Go to the Blueprints folder and create a folder called UI, and in there a folder called InGame. Enter that folder.
2. Create a blueprint class that is based on BaseDialogBoxWidget and call it W_DialogBoxWidget.
    1. Open the widget
    2. Design the widget however you like
        - Add a text block to the widget named DialogText
        - Add a text block to the widget named CharacterNameText
3. Create a blueprint class that is based on BaseChoiceButton and call it W_ChoiceButton.
    1. Open the widget
    2. Design the widget however you like
        - Add a button to the widget named ChoiceButton
        - Add a text block to the widget named ChoiceText
4. Create a blueprint class that is based on BaseChoiceWidget and call it W_ChoiceWidget.
    1. Open the widget
    2. Design the widget however you like
        - Add a vertical/horizontal/... box to the widget named ChoiceButtonsList
    3. In the settings of the widget set the Chocie Button Class to W_ChoiceWidget
5. Create a blueprint class that is based on HUD and call it BP_InGameHud.
    1. Open the blueprint
    2. Add the component Dialog Controller
    3. In the settings of the component set the Dialog Box Widget Class to W_DialogBoxWidget
    4. In the settings of the component set the Dialog Box Widget Class to W_ChoiceWidget
6. Navigate back up to the Blueprints folder and create a folder called Core. Enter that folder.
7. Create a blueprint class that is based on BaseGameMode and call it BP_InGameGameMode
    1. Open the blueprint.
    1. Set the default hud class to W_InGameHud
8. Create a new blank map and call it InGameMap
    1. Open the level
    2. Open the World Settings Panel
    3. Set the Game Mode Override to BP_InGameGameMode
9. Create a new blank map and call it MainMenu
10. Go to the project settings and navigate to maps & modes
    - Set the Game Default Map to MainMenu
11. Navigate to the Visual Novel Machinery in the plugins category
    - Set the Main Menu Level Name field to MainMenu

Next up is [setting up the character UI]({{ site.baseurl }}{% link get-started/project-setup/setup-character-ui.md %}).