---
layout: single
title: Character Persistant Memory Get
permalink: /docs/nodes-references/character-persistant-memory-get
toc: true
sidebar:
  nav: "docs"
---


![Character Persistant Memory Get Node Visual]({{ site.baseurl }}/assets/images/NodeReference/character-persistant-memory-get.png)

## Pins

### Output

| Name | Type | Description |
| --- | --- | --- |
| Value | Wildcard | The value of the persistant memory (Type depends on what has been configured) |

## On-Node Properties

| Name | Description |
| --- | --- |
| Character | The Id of the character from whom to get the persistant memory value |
| Memory | The Id of the persistant memory which value should be used |

## Additional Properties

This node has no additional properties.

## Script Reference
```
<variable name>=character.memory.persistant.get <character id> <character persistant memory id>
```