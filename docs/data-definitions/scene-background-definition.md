---
layout: single
title: Scene Background Definition
permalink: /docs/data-definitions/scene-background-definition
toc: true
sidebar:
  nav: "docs"
---



The class name for this definition is **DialogImageDefinition**. It is used with a Data Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Dialog Image Id | FName | The internal ID identifying the scene background |
| Dialog Image | UTexture2D* | The actual scene background texture |
| Dialog Image Layers | TMap\<FName, FImageLayerDefinition\> | Array of Layer information for this specific scene background |
