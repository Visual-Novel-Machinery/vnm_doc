---
layout: single
title: Dialog Definition
permalink: /docs/data-definitions/dialog-definition
toc: true
sidebar:
  nav: "docs"
---



The class name for this definition is **DialogDefinition**. It is used with a Data Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Dialogue Id | FName | The internal ID identifying this dialog scene |
| Dialog Title | FText | The friendly name of the dialog scene |
| Dialogue Object Class | TSubclassOf\<UDialogObject\> | The actual Dialog Blueprint |
| Dialogue Description | FText | Text to describe what is happening in the scene, or even your notes about this scene |
| DialogMemoryDefinitions | TArray\<FMemoryDefinition\> | Array of Memories that are relevant to this dialog scene |