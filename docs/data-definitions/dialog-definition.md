---
layout: single
title: Dialog Definition
permalink: /docs/data-definitions/dialog-definition
toc: true
sidebar:
  nav: "docs"
---

The class name for this definition is **FDialogDefinition**. It is used with a Data Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Dialogue Id | FName | The unique identifier for this dialog scene |
| Dialog Title | FText | The user-friendly title of this dialog scene |
| Dialogue Object Class | TSubclassOf\<UDialogObject\> | The dialog blueprint class that contains the dialog flow logic |
| Dialogue Description | FText | Descriptive text about this dialog scene (for documentation/notes) |
| Dialog Background Override | FImageDefinition | Custom dialog box background that overrides the default for this dialog |
| Dialog Memory Definitions | TArray\<FMemoryDefinition\> | Array of memory variables specific to this dialog scene |
| Dialog Persistant Memory Definitions | TArray\<FMemoryDefinition\> | Array of persistent memory variables specific to this dialog scene |
| Voice Over Definitions | TMap\<FName, FVoiceOverDefinition\> | Map of voice over audio definitions for this dialog |

## Related Structures

### FImageDefinition
- **Image**: The image asset (Texture2D or Material) to display
- **Image Size**: The size of the image in pixels (zero vector uses original size)
- **Color And Opacity**: The color tint and opacity applied to the image

### FMemoryDefinition
- **Memory Id**: The unique identifier for this memory variable
- **Type**: The data type of the memory variable (Bool, Integer, Float, etc.)

### FVoiceOverDefinition
- **Dialog Audio Id**: The internal ID identifying the audio
- **Audio Object**: The actual audio object