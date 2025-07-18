---
layout: single
title: Dialog Persistant Memory Get
permalink: /docs/nodes-references/dialog-persistant-memory-get
toc: true
sidebar:
  nav: "docs"
---


![Dialog Persistant Memory Get Node Visual]({{ site.baseurl }}/assets/images/NodeReference/dialog-persistant-memory-get.png)

## Pins

### Output

| Name | Type | Description |
| --- | --- | --- |
| Value | Wildcard | The value of the persistant memory (Type depends on what has been configured) |

## On-Node Properties

| Name | Description |
| --- | --- |
| Dialog | The Id of the dialog from whom to get the persistant memory value |
| Memory | The Id of the persistant memory which value should be used |

## Additional Properties

This node has no additional properties.

## Script Reference
```
<variable name>=dialog.memory.persistant.get <dialog id> <dialog persistant memory id>
```