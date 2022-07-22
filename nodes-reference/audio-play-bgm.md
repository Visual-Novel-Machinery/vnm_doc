---
layout: default
title: Dialog Audio Play Background Music
parent: Nodes Reference
---
# Dialog Audio Play Background Music

![Dialog Audio Play Background Music Visual]({{ site.baseurl }}/assets/images/NodeReference/audio-play-bgm.png)

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
| Background Music Id | The Id of the background music to play |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Volume | float | The volume at which the background music should play (0.0-1.0) |
| Pitch | float | The pitch at which the background music will be played |
| Start Time | float | The time in seconds at which to start in the background music. Default is 0.0 seconds. |
| Wait for Audio To Finish | bool | If true the system will wait for the background music to finish before moving on to the next node. Is incompatible with property "Is Looping" |
| Is Looping | bool | If true the background music will loop until stopped |