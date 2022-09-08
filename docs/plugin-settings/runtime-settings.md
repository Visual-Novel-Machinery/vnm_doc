---
layout: single
title: Runtime Settings
permalink: /docs/plugin-settings/runtime-settings
toc: true
sidebar:
  nav: "docs"
---

The settings can be found under Project Settings -> Plugin -> VNM Settings.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Character Definitons Table | UDataTable* | Data Table containing all characters |
| Cg Definitons Table | UDataTable* | Data Table containing all CGs |
| Scene Background Definitons Table | UDataTable* | Data Table containing all scene backgrounds |
| Dialog Scene Definitions Table | UDataTable* | Data Table containing all dialog scenes |
| Dialog Definitons Table | UDataTable* | Data Table containing all dialogs |
| Main Menu Level Name | FString | Name of the main menu level |
| Save Game Class | TSubclassOf\<UVNMBaseSaveGame\> | Class used for the save game system for the save file |
| Persistant Save Game Class | TSubclassOf\<UVNMBasePersistantSaveGame\> | Class used for the save game system for the persistant save file |
| Camera Class | TSubclassOf\<ACameraActor\> | Class used when searching for cameras in a dialog scene |
| Character Position Values | TMap\<ECharacterPositioning, float\> | Positioning values of the characters at LEFT/RIGHT/CENTER |
| Typewriter Effect Active | bool | Used to turn on/off the typewriter effect |
| Type Writing Speed | float | The speed of the type writing effect |