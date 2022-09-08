---
layout: single
title: Setting up Data Tables
permalink: /docs/project-setup/setup-data-tables/
toc: true
sidebar:
  nav: "docs"
---


1. Go to the Data folder and create data tables of the following types
    - CharacterDefinition (Named DT_CharacterDefinitions for future reference)
    - DialogDefinition (Named DT_DialogDefinitions for future reference)
    - DialogImageDefinition (Named DT_CgDefinitions for future reference)
    - DialogImageDefinition (Named DT_SceneBackgroundDefinitions for future reference)
    - DialogSceneDefinition (Named DT_DialogSceneDefinitions for future reference)
    - RichTextStyleRow (Named DT_DialogTextStyles for future reference)
    
    ![Table Definition Picker]({{ site.baseurl }}/assets/images/DataTableSetup/TableDefinitionPicker.png)
    
    ![Created Data Tables]({{ site.baseurl }}/assets/images/DataTableSetup/CreatedDataTables.png)
2. Go to the project settings and navigate to Visual Novel Machinery in the plugins category
3. Set the following settings
    - CharacterDefinitonsTable to DT_CharacterDefinitions
    - DialogDefinitonsTable to DT_DialogDefinitions
    - CgDefinitonsTable to DT_CgDefinitions
    - SceneBackgroundDefinitonsTable to DT_SceneBackgroundDefinitions
    - DialogSceneDefinitionsTable to DT_DialogSceneDefinitions
    
    ![Data Table Project Settings]({{ site.baseurl }}/assets/images/DataTableSetup/DataTableProjectSettings.png)

## DT_CharacterDefinitions
This data table will hold all the information that the plugin needs about every single character that will appear in the game. This could be the name of the character, or also the visual appearance of the character. More details on characters can be found [here]({{ site.baseurl }}{% link docs/features/characters.md %}).

## DT_DialogDefinitions
This data table will hold all the information about the scene. This includes the actual dialog object, the name of the scene, and much more. More details on dialogs can be found [here]({{ site.baseurl }}{% link docs/features/Dialogs.md %}).

## DT_CgDefinitions
If you intend to display CGs in your visual novel, this data table will hold the information about each of them, specifically which image to display. More details on CGs can be found [here]({{ site.baseurl }}{% link docs/features/Cgs.md %}).

## DT_SceneBackgroundDefinitions
If you intend to display images in the background during scenes in your visual novel, this data table will hold the information about each of them, specifically which image to display. More details on scene backgrounds can be found [here]({{ site.baseurl }}{% link docs/features/scene-backgrounds.md %}).

## DT_DialogSceneDefinitions
If you intend to display 3d scenes during dialogs in your visual novel, this data table will hold the information about each of them, specifically which 3d scene to display. More details on Dialog Scenes can be found [here]({{ site.baseurl }}{% link docs/features/dialog-scenes.md %}).

## DT_DialogTextStyles
This data table is needed for customizing the dialog text displayed at runtime. More details on dialog texts can be found [here]({{ site.baseurl }}{% link docs/features/Dialogs.md %}).


After having set up the data tables, we can now move on to [setting up the dialog UI]({{ site.baseurl }}{% link docs/project-setup/setup-dialog-box-ui.md %}).