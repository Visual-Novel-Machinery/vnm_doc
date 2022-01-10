---
layout: default
title: Scene Background Definition
parent: Data Definitions
nav_order: 2
---

# Scene Background Definition

The class name for this definition is **DialogImageDefinition**. It is used with a Data Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Dialog Image Id | FName | The internal ID identifying the scene background |
| Dialog Image | UTexture2D* | The actual scene background texture |
| Dialog Image Layers | TMap\<FName, FImageLayerDefinition\> | Array of Layer information for this specific scene background |
