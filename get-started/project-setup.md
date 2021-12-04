---
layout: default
title: Project Setup
parent: Get Started
nav_order: 2
---

## Initial Setup
1. Download the plugin from Gumroad or the Unreal Marketplace
2. Create a Project in Unreal Engine 4. Use the blank template.
3. Copy the plugin in the Plugins folder in the root folder of the project.
    - Path should then be \<path to root\>/Plugins/VisualNovelMachinery/
4. Compile and start up the project.
5. Create the following folders in the root folder: Art, Blueprints, Data, Dialogs, Maps
    - You don't need to use the proposed structure mentioned above, the rest of the guide will however use it.

## Setup of Data Tables
1. Go to the Data folder and create data tables of hte following type
    - CharacterDefinition (Named DT_CharacterDefinitions for future reference)
    - DialogDefinition (Named DT_DialogDefinitions for future reference)
    - DialogImageDefinition (Named DT_CgDefinitions for future reference)
    - DialogImageDefinition (Named DT_SceneBackgroundDefinitions for future reference)
2. Go to the project settings and navigate to Visual Novel Machinery in the plugins category
3. Set the following settings
    - CharacterDefinitonsTable to DT_CharacterDefinitions
    - DialogDefinitonsTable to DT_DialogDefinitions
    - CgDefinitonsTable to DT_CgDefinitions
    - SceneBackgroundDefinitonsTable to DT_SceneBackgroundDefinitions

## Setup of the Dialog Box UI
1. Go to the Blueprint folder and create a folder called UI, and in there a folder called InGame
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
    3. In the settings of the component set the Dialog Box Widget Class to W_ChoiceWidget
6. Create a blueprint class that is based on BaseGameMode and call it BP_InGameGameMode
    1. Set the default hud class to W_InGameHud
7. Create a new blank map and call it InGameMap
    1. Open the level
    2. Open the World Settings Panel
    3. Set the Game Mode Override to BP_InGameGameMode
8. Create a new blank map and call it MainMenu
9. Go to the project settings and navigate to maps & modes
    - Set the Game Default Map to MainMenu
10. Navigate to the Visual Novel Machinery in the plugins category
    - Set the Main Menu Level Name field to MainMenu

## Additional setup
If you intend to use other features like characters/CGs/scene backgrounds, check the basic instruction in the respective categories.

You can now move on to the introduction about [dialogs]({{ site.baseurl }}{% link features/Dialogs.md %}).