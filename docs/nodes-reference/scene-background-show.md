---
layout: single
title: Scene Background Show
permalink: /docs/nodes-references/scene-background-show
toc: true
sidebar:
  nav: "docs"
---


![Scene Background Show Node Visual]({{ site.baseurl }}/assets/images/NodeReference/scene-background-show.png)

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
| Scene Background | The Id of the Scene Background to show |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Transition Event | Transition Event | How should the scene background be shown |
| Custom Transition Event Name | FString | The name of the animation to use if Transition Event is set to Custom |
| Dont Wait For Transition To Finish | Boolean | If set to true then the dialog will automatically continue, while the scene background finishes its transition |