---
layout: single
title: Scene Background Definition
permalink: /docs/data-definitions/scene-background-definition
toc: true
sidebar:
  nav: "docs"
---

The class name for this definition is **FDialogImageDefinition**. It is used with a Data Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Dialog Image Id | FName | The unique identifier for this dialog image |
| Dialog Image | FImageDefinition | The image definition containing the actual texture and display properties |
| Dialog Image Group Id | FName | Group identifier for organizing related images together |
| Dialog Image Layers | TMap\<FName, FImageLayerDefinition\> | Map of image layers for complex multi-layered images |

## Related Structures

### FImageDefinition
- **Image**: The image asset (Texture2D or Material) to display
- **Image Size**: The size of the image in pixels (zero vector uses original size)
- **Color And Opacity**: The color tint and opacity applied to the image

### FImageLayerDefinition
- **Layer Id**: The unique identifier for this image layer
- **Layer Index**: The rendering order of this layer (0-10, higher values render on top)
- **Layer Image Per Id**: Map of image definitions per ID for this layer