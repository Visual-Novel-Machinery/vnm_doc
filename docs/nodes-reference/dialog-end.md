---
layout: single
title: Dialog End
permalink: /docs/nodes-references/dialog-end
toc: true
sidebar:
  nav: "docs"
---


![Dialog End Node Visual]({{ site.baseurl }}/assets/images/NodeReference/dialog-end.png)

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
| Next Dialog | The next dialog to start. If set to None, the game will return to the Main Menu level specified in the Project Settings |

## Script Reference
```
dialog.end [-nextdialog=<next dialog id>]
```