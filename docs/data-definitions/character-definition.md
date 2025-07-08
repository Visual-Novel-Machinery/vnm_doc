---
layout: single
title: Character Definition
permalink: /docs/data-definitions/character-definition
toc: true
sidebar:
  nav: "docs"
---

The class name for this definition is **FCharacterDefinition**. It is used with a Data Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Character Id | FName | The unique identifier for this character |
| Character Display Name | FText | The display name shown for this character in the UI |
| Character Display Color | FSlateColor | The color of the character's name text in dialog boxes |
| Dialog Background Override | FImageDefinition | Custom dialog box background that overrides the default when this character speaks |
| Character Description | FText | Descriptive text about this character (for documentation/notes) |
| Character Image Per Emotion | TMap\<FName, FImageDefinition\> | Map of character images for different emotions/expressions |
| Character Image Layers | TMap\<FName, FImageLayerDefinition\> | Map of image layers for advanced character display with multiple elements |
| Character Mesh | USkeletalMesh* | 3D skeletal mesh for this character when displayed in 3D scenes |
| Character Animation Per Emotion | TMap\<FName, UAnimationAsset*\> | Map of animations for different character emotions when using 3D mesh |
| Character Memory Definitions | TArray\<FMemoryDefinition\> | Array of memory variables specific to this character |
| Voice Over Definitions | TMap\<FName, FVoiceOverDefinition\> | Map of voice over audio definitions for this character |

## Related Structures

### FImageDefinition
- **Image**: The image asset (Texture2D or Material) to display
- **Image Size**: The size of the image in pixels (zero vector uses original size)
- **Color And Opacity**: The color tint and opacity applied to the image

### FImageLayerDefinition
- **Layer Id**: The unique identifier for this image layer
- **Layer Index**: The rendering order of this layer (0-10, higher values render on top)
- **Layer Image Per Id**: Map of image definitions per ID for this layer

### FMemoryDefinition
- **Memory Id**: The unique identifier for this memory variable
- **Type**: The data type of the memory variable (Bool, Integer, Float, etc.)

### FVoiceOverDefinition
- **Dialog Audio Id**: The internal ID identifying the audio
- **Audio Object**: The actual audio object