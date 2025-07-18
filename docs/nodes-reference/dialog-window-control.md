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
| Mode | **Auto**: Automatically show and hide the dialog window at the end of the dialog. **Manual**: The dialog window will only show or hide when using this node for visibility |

## Additional Properties

This node has no additional properties.

## Script Reference
```
dialog.window.control [-automatic/manual]
```