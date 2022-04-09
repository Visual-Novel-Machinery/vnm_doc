---
layout: default
title: Runtime Settings
parent: Plugin Settings
nav_order: 1
---

## Runtime Settings

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