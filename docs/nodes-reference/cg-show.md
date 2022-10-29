---
layout: single
title: CG Show
permalink: /docs/nodes-references/cg-show
toc: true
sidebar:
  nav: "docs"
---


![CG Show Node Visual]({{ site.baseurl }}/assets/images/NodeReference/cg-show.png)

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
| Cg | The Id of the CG to show |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Transition Event | Transition Event | How should the CG be shown |
| Custom Transition Event Name | FString | The name of the animation to use if Transition Event is set to Custom |
| Dont Wait For Transition To Finish | Boolean | If set to true then the dialog will automatically continue, while the CG finishes its transition |

## Script Reference
```
cg.show -id=<cg id> [-transition=<transition name>] [-dontwait] [-customtransition=<Animation name>]
```