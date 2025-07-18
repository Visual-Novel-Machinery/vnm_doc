---
layout: single
title: Character Persistant Memory Set
permalink: /docs/nodes-references/character-persistant-memory-set
toc: true
sidebar:
  nav: "docs"
---


![Character Persistant Memory Set Node Visual]({{ site.baseurl }}/assets/images/NodeReference/character-persistant-memory-set.png)

## Pins

### Input

| Name | Type | Description |
| --- | --- | --- |
| Execution Line In | Execution | Execution Line Input |
| Value | Wildcard | The new value of the persistant memory (Type depends on what has been configured) |

### Output

| Name | Type | Description |
| --- | --- | --- |
| Execution Line Out | Execution | Execution Line Output |

## On-Node Properties

| Name | Description |
| --- | --- |
| Character | The Id of the character from whom to override the persistant memory value |
| Memory | The Id of the persistant memory which value should be overriden |

## Additional Properties

This node has no additional properties.

## Script Reference
```
character.memory.persistant.set <character id> <character persistant memory id> <variable name>
```