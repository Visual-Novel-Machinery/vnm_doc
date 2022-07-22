---
layout: default
title: Dialog Audio Play Sound Effect
parent: Nodes Reference
---
# Dialog Audio Play Sound Effect

![Dialog Audio Play Sound Effect Visual]({{ site.baseurl }}/assets/images/NodeReference/audio-play-sfx.png)

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
| Sound Effect Id | The Id of the Sound Effect to play |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Volume | float | The volume at which the Sound Effect should play (0.0-1.0) |
| Pitch | float | The pitch at which the Sound Effect will be played |
| Start Time | float | The time in seconds at which to start in the Sound Effect. Default is 0.0 seconds. |
| Wait for Audio To Finish | bool | If true the system will wait for the Sound Effect to finish before moving on to the next node. |