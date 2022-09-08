---
layout: single
title: Dialog Window Control
permalink: /docs/nodes-references/dialog-window-control
toc: true
sidebar:
  nav: "docs"
---


![Dialog Window Control Node Visual]({{ site.baseurl }}/assets/images/NodeReference/dialog-window-control.png)

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
| Visibility | Wether to show or hide the dialog window |
| Mode | **Auto**: Automatically show and hide the dialog window at the end of the dialog. **Manual**: The dialog window will only show or hide when using this node for visibility |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Transition Event | Transition Event | How should the dialog window be transitioning |
| Custom Transition Event Name | FString | The name of the animation to use if Transition Event is set to Custom |
| Dont Wait For Transition To Finish | Boolean | If set to true then the dialog will automatically continue, while the dialog window finishes its transition |