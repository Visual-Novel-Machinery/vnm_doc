---
layout: single
title: Dialog Memory Get
permalink: /docs/nodes-references/dialog-memory-get
toc: true
sidebar:
  nav: "docs"
---


![Dialog Memory Get Node Visual]({{ site.baseurl }}/assets/images/NodeReference/dialog-memory-get.png)

## Pins

### Output

| Name | Type | Description |
| --- | --- | --- |
| Value | Wildcard | The value of the memory (Type depends on what has been configured) |

## On-Node Properties

| Name | Description |
| --- | --- |
| Dialog | The Id of the dialog from whom to get a memory value |
| Memory | The Id of the memory which value should be used |

## Script Reference
```
<variable name>=dialog.memory.get <dialog id> <dialog memory id>
```