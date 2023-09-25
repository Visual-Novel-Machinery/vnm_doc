---
layout: single
title: Character Rename
permalink: /docs/nodes-references/character-rename
toc: true
sidebar:
  nav: "docs"
---


![Character Rename Node Visual]({{ site.baseurl }}/assets/images/NodeReference/character-rename.png)

## Pins

### Input

| Name | Type | Description |
| --- | --- | --- |
| Execution Line In | Execution | Execution Line Input |

### Output

| Name | Type | Description |
| --- | --- | --- |
| Execution Line Out | Execution | Execution Line Output |

## On-Node Properties

| Name | Description |
| --- | --- |
| Character | The Id of the character to rename |
| New character name | The new name of the character |

## Script Reference
```
character.rename <character id> <new character name>
```