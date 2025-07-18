---
layout: single
title: Dialog Window Show
permalink: /docs/nodes-references/dialog-window-show
toc: true
sidebar:
  nav: "docs"
---


![Dialog Window Show Node Visual]({{ site.baseurl }}/assets/images/NodeReference/dialog-window-show.png)

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

This node has no on-node properties.

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Transition Event | Transition Event | How should the dialog window be transitioning |
| Custom Transition Event Name | FString | The name of the animation to use if Transition Event is set to Custom |
| Dont Wait For Transition To Finish | Boolean | If set to true then the dialog will automatically continue, while the dialog window finishes its transition |

## Script Reference
```
dialog.window.show
```