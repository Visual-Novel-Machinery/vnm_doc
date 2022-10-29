---
layout: single
title: Dialog Audio Play Dialog Voice Over
permalink: /docs/nodes-references/audio-play-dialog-voice-over
toc: true
sidebar:
  nav: "docs"
---


![Dialog Audio Play Dialog Voice Over Visual]({{ site.baseurl }}/assets/images/NodeReference/audio-play-dialog-voice-over.png)

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
| Voice Over Id | The Id of the Dialog Voice Over to play |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Volume | float | The volume at which the Dialog Voice Over should play (0.0-1.0) |
| Pitch | float | The pitch at which the Dialog Voice Over will be played |
| Start Time | float | The time in seconds at which to start in the Dialog Voice Over. Default is 0.0 seconds. |
| Wait for Audio To Finish | bool | If true the system will wait for the Dialog Voice Over to finish before moving on to the next node. |

## Script Reference
```
audio.play.dialog.voiceover -dialog=<dialog id> -id=<voice over id> [-volume=<volume level>] [-pitch=<pitch level>] [-starttime=<start time>] [-wait]
```