---
layout: default
title: Setting up Data Tables
parent: Project Setup
grand_parent: Get Started
nav_order: 2
---

# Setting up Data Tables
1. Go to the Data folder and create data tables of the following types
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

## DT_CharacterDefinitions
This data table will hold all the information that the plugin needs about every single character that will appear in the game. This could be the name of the character, or also the visual appearance of the character. More details on characters can be found [here]({{ site.baseurl }}{% link features/characters/index.md %}).

## DT_DialogDefinitions
This data table will hold all the information about the scene. This includes the actual dialog object, the name of the scene, and much more. More details on dialogs can be found [here]({{ site.baseurl }}{% link features/Dialogs.md %}).

## DT_CgDefinitions
If you intend to display CGs in your visual novel, this data table will hold the information about each of them, specifically which image to display. More details on CGs can be found [here]({{ site.baseurl }}{% link features/Cgs.md %}).

## DT_SceneBackgroundDefinitions
If you intend to display images in the background during scenes in your visual novel, this data table will hold the information about each of them, specifically which image to display. More details on scene backgrounds can be found [here]({{ site.baseurl }}{% link features/scene-backgrounds.md %}).

After having set up the data tables, we can now move on to [setting up the dialog UI]({{ site.baseurl }}{% link get-started/project-setup/setup-dialog-box-ui.md %}).