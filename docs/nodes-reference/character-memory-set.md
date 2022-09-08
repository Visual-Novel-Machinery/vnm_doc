---
layout: single
title: Character Memory Set
permalink: /docs/nodes-references/character-memory-set
toc: true
sidebar:
  nav: "docs"
---


![Character Memory Set Node Visual]({{ site.baseurl }}/assets/images/NodeReference/character-memory-Set.png)

## Pins

### Input

| Name | Type | Description |
| --- | --- | --- |
| Execution Line In | Execution | Execution Line Input |
| Value | Wildcard | The new value of the memory (Type depends on what has been configured) |

### Output

| Name | Type | Description |
| --- | --- | --- |
| Execution Line Out | Execution | Execution Line Output |

## On-Node Properties

| Name | Description |
| --- | --- |
| Character | The Id of the character from whom to override the memory value |
| Memory | The Id of the memory which value should be overriden |
