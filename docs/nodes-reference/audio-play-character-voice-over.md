---
layout: single
title: Dialog Audio Play Character Voice Over
permalink: /docs/nodes-references/audio-play-character-voice-over
toc: true
sidebar:
  nav: "docs"
---


![Dialog Audio Play Character Voice Over Visual]({{ site.baseurl }}/assets/images/NodeReference/audio-play-character-voice-over.png)

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
| Character Id | The Id of the character whose voice over will play |
| Voice Over Id | The Id of the Character Voice Over to play |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Volume | float | The volume at which the Character Voice Over should play (0.0-1.0) |
| Pitch | float | The pitch at which the Character Voice Over will be played |
| Start Time | float | The time in seconds at which to start in the Character Voice Over. Default is 0.0 seconds. |
| Wait for Audio To Finish | bool | If true the system will wait for the Character Voice Over to finish before moving on to the next node. |