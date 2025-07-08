---
layout: single
title: Runtime Settings
permalink: /docs/plugin-settings/runtime-settings
toc: true
sidebar:
  nav: "docs"
---

The settings can be found under Project Settings -> Plugin -> VNM Settings.

## Data Tables

| Name | Type | Description |
| --- | --- | --- |
| Character Definitons Table | UDataTable* | Data table containing all character definitions |
| Cg Definitons Table | UDataTable* | Data table containing all CG (Computer Graphics) image definitions |
| Scene Background Definitons Table | UDataTable* | Data table containing all scene background image definitions |
| Dialog Scene Definitions Table | UDataTable* | Data table containing all 3D dialog scene definitions |
| Dialog Audio Definitions Table | UDataTable* | Data table containing all audio definitions (BGM, SFX, voice over) |
| Dialog Definitons Table | UDataTable* | Data table containing all dialog scene definitions |

## General

| Name | Type | Description |
| --- | --- | --- |
| In Game Level Name | FString | The name of the level used for in-game visual novel scenes |
| Main Menu Level Name | FString | The name of the level used for the main menu |

## Save System

| Name | Type | Description |
| --- | --- | --- |
| Save Game Class | TSubclassOf\<UVNMBaseSaveGame\> | The class used for creating save game objects |
| Persistant Save Game Class | TSubclassOf\<UVNMBasePersistantSaveGame\> | The class used for creating persistent save game objects (settings, etc.) |
| Generate Save File Name | bool | Whether to automatically generate save file names or let user specify them |
| Confirm Before Deleting Save File | bool | Whether to show a confirmation dialog before deleting save files |

## Dialog Scene

| Name | Type | Description |
| --- | --- | --- |
| Camera Class | TSubclassOf\<ACameraActor\> | The camera actor class used in dialog scenes |

## Character

| Name | Type | Description |
| --- | --- | --- |
| Character Position Values | TMap\<ECharacterPositioning, float\> | Predefined character positioning values (0.0 to 1.0 across screen width) |
| Custom Character Position Values | TMap\<FName, FVector2D\> | Custom character positioning values with 2D coordinates |

## Dialog

| Name | Type | Description |
| --- | --- | --- |
| Typewriter Effect Active | bool | Whether to enable typewriter effect for dialog text |
| Type Writing Speed | float | Speed of the typewriter effect in seconds per character |
| Auto Forward Time | float | Time to wait before auto-advancing dialog (0 disables auto-forward) |
| Autostart Dialog | bool | Whether to automatically start dialog when entering a dialog scene |
| Autostart First Dialog If No Dialog Is Found | bool | Whether to start the first dialog if no specific dialog is found |

## Auto Save

| Name | Type | Description |
| --- | --- | --- |
| Auto Save Type | EAutoSaveType | The type of auto-save system to use (MANUAL or AUTOMATIC) |
| Auto Save Interval In Seconds | float | Interval between automatic saves in seconds (default: 5 minutes) |