---
layout: single
title: Character 3D Show
permalink: /docs/nodes-references/character-3d-show
toc: true
sidebar:
  nav: "docs"
---


![Character 3D Show Node Visual]({{ site.baseurl }}/assets/images/NodeReference/character-3d-show.png)

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
| Character 3D | The Id of the character to show |
| Emotion | The Id of the emotion of the character to show |
| Dialog Scene Id | The Id of the Dialog Scene in which the spawn location is |
| Spawn Location Name | The name of the location where the character will be spawned at |

## Script Reference
```
character3d.show -id=<character id> -emotion=<emotion id> -dialogscene=<dialog scene id> -spawnlocation=<spawn location id>
```