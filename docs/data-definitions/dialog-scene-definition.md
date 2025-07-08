---
layout: single
title: Dialog Scene Definition
permalink: /docs/data-definitions/dialog-scene-definition
toc: true
sidebar:
  nav: "docs"
---

The class name for this definition is **FDialogSceneDefinition**. It is used with a Data Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Dialog Scene Id | FName | The unique identifier for this dialog scene |
| Dialog Scene | TSoftObjectPtr\<UWorld\> | The 3D level/world that represents this dialog scene (must be added as sublevel) |
| Dialog Camera Names | TArray\<FActorIdentifier\> | Array of camera actors available in this dialog scene |
| Dialog Spawn Location Names | TArray\<FActorIdentifier\> | Array of spawn location actors for placing 3D characters in this scene |

## Related Structures

### FActorIdentifier
- **Actor Internal Name**: The internal name used to identify the actor in the system
- **Actor Label**: The user-friendly label displayed for the actor

## Important Notes

- **IMPORTANT**: You have to add this level to your in-game level as a sublevel, otherwise it can't be streamed in
- Camera actors and spawn location actors are identified using FActorIdentifier structures that contain both internal names and user-friendly labels
- This allows for better organization and identification of actors within the dialog scene system