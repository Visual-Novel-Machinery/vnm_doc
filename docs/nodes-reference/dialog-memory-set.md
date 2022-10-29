---
layout: single
title: Dialog Memory Set
permalink: /docs/nodes-references/dialog-memory-set
toc: true
sidebar:
  nav: "docs"
---


![Dialog Memory Set Node Visual]({{ site.baseurl }}/assets/images/NodeReference/dialog-memory-set.png)

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
| dialog | The Id of the dialog from which to override the memory value |
| Memory | The Id of the memory which value should be overriden |

## Script Reference
```
dialog.memory.set <dialog id> <dialog memory id> <variable name>
```