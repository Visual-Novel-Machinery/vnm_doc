---
layout: single
title: Dialog Widget Hide
permalink: /docs/nodes-references/dialog-widget-hide
toc: true
sidebar:
  nav: "docs"
---


![Dialog Widget Hide Node Visual]({{ site.baseurl }}/assets/images/NodeReference/dialog-widget-hide.png)

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
| Activatable Widget Class | The class of the widget to show |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Wait For widget to close again | Boolean | If set to false, then the dialog will automatically continue. |

## Script Reference
```
widget.show <widget blueprint name (ex: W_TestWidget)>
```