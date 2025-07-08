---
layout: single
title: Dialog Play Animation
permalink: /docs/nodes-references/dialog-play-animation
toc: true
sidebar:
  nav: "docs"
---


![Dialog Play Animation Node Visual]({{ site.baseurl }}/assets/images/NodeReference/dialog-play-animation.png)

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
| Play Backwards | Boolean | If set to true, the animation will play in reverse |
| Transition Event | ETransitionEvent | The type of transition to apply during animation |
| Animation Playback Multiplier | Float | Multiplier for animation playback speed (1.0 = normal speed) |
| Custom Transition Event Name | FString | The name of the custom animation to use if Transition Event is set to Custom |
| Don't Wait For Transition To Finish | Boolean | If set to true, the dialog will automatically continue while the animation finishes |

## Script Reference
```
This node does not have a direct script equivalent.
```