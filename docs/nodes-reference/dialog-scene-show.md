---
layout: single
title: Dialog Scene Show
permalink: /docs/nodes-references/dialog-scene-show
toc: true
sidebar:
  nav: "docs"
---


![Dialog Scene Show Node Visual]({{ site.baseurl }}/assets/images/NodeReference/dialog-scene-show.png)

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
| Dialog Scene Id | The Id of the Dialog Scene to show |
| Camera Name | The camera to switch to after entering the dialog scene |

## Script Reference
```
dialogscene.show -id=<scene background id> -camera=<camera name>
```