---
layout: single
title: Dialog Scene Definition
permalink: /docs/data-definitions/dialog-scene-definition
toc: true
sidebar:
  nav: "docs"
---



The class name for this definition is **DialogSceneDefinition**. It is used with a Data Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Dialog Scene Id | FName | The internal ID identifying the scene |
| Dialog Scene | TSoftObjectPtr\<UWorld\> | The actual level **IMPORTANT: YOU HAVE TO ADD THIS LEVEL TO YOUR INGAME LEVEL AS A SUBLEVEL, OTHERWISE IT CAN'T BE STREAMED IN** |
| Dialog Camera Names | TArray\<FName\> | Cameras in the dialog scene |
| Dialog Spawn Location Names | TArray\<FName\> | Spawn Locations for 3D characters in the dialog scene |