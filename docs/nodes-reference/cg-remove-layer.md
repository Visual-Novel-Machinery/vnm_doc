---
layout: single
title: CG Remove Layer
permalink: /docs/nodes-references/cg-remove-layer
toc: true
sidebar:
  nav: "docs"
---


![CG Remove Layer Node Visual]({{ site.baseurl }}/assets/images/NodeReference/cg-remove-layer.png)

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
| Cg | The Id of the CG to which to remove the layer from |
| Layer | The Id of the layer that will be removed |

## Script Reference
```
cg.removelayer -id=<cg id> -layer=<layer id>
```
