---
layout: single
title: Dialog Persistant Memory Set
permalink: /docs/nodes-references/dialog-persistant-memory-set
toc: true
sidebar:
  nav: "docs"
---


![Dialog Persistant Memory Set Node Visual]({{ site.baseurl }}/assets/images/NodeReference/dialog-persistant-memory-set.png)

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
| Dialog | The Id of the dialog from whom to override the persistant memory value |
| Memory | The Id of the persistant memory which value should be overriden |

## Additional Properties

This node has no additional properties.

## Script Reference
```
dialog.memory.persistant.set <dialog id> <dialog persistant memory id> <variable name>
```