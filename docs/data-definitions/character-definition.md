---
layout: single
title: Character Definition
permalink: /docs/data-definitions/character-definition
toc: true
sidebar:
  nav: "docs"
---



The class name for this definition is **CharacterDefinition**. It is used with a Data Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Character Id | FName | The internal ID identifying the scene background |
| Character Display Name | FText | The friendly name of the character |
| Character Display Color | FSlateColor | The color of the character name text in the dialog box widget |
| Character Description | FText | A friendly description of the character, or your notes about the character |
| Character Image per Emotion | TMap\<FName, UTexture2D*\> | The actual texture used by the character for a specific emotion ID |
| Character Image Layers | TMap\<FName, FImageLayerDefinition\> | Array of Layer information for this specific character |
| Character Mesh | USkeletalMesh* | Skeletal Mesh displayed in 3D world |
| Character Animation Per Emotion | TMap\<FName, UAnimationAsset*\> | Animation asset used with skeletal mesh in 3D world |
| Character Memory Definitions | TArray\<FMemoryDefinition\> | Array of Memories that are relevant to this character |