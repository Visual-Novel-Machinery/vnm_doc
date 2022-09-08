---
layout: single
title: CG Hide
permalink: /docs/nodes-references/cg-hide
toc: true
sidebar:
  nav: "docs"
---


![CG Hide Node Visual]({{ site.baseurl }}/assets/images/NodeReference/cg-hide.png)

## Pins

### Input

| Name | Type | Description |
| --- | --- | --- |
| Execution Line In | Execution | Execution Line Input |

### Output

| Name | Type | Description |
| --- | --- | --- |
| Execution Line Out | Execution | Execution Line Output |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Transition Event | Transition Event | How should the CG be hidden |
| Custom Transition Event Name | FString | The name of the animation to use if Transition Event is set to Custom |
| Dont Wait For Transition To Finish | Boolean | If set to true then the dialog will automatically continue, while the CG finishes its transition |