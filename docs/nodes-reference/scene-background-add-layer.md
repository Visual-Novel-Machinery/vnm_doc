---
layout: single
title: Scene Background Add Layer
permalink: /docs/nodes-references/scene-background-add-layer
toc: true
sidebar:
  nav: "docs"
---


![Scene Background Add Layer Node Visual]({{ site.baseurl }}/assets/images/NodeReference/scene-background-add-layer.png)

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
| Scene Background | The Id of the Scene Background to which to add the layer |
| Layer | The Id of the layer that will be added/modified |
| Image | The Id of the image that will be displayed in the layer |

## Script Reference
```
scenebackground.addlayer -id=<scene background id> -layer=<layer id> -image=<image id>
```