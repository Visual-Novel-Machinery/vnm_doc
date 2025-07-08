---
layout: single
title: Dialog Audio Definition
permalink: /docs/data-definitions/dialog-audio-definition
toc: true
sidebar:
  nav: "docs"
---

The class name for this definition is **FDialogAudioDefinition**. It is used with a Data Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Dialog Audio Id | FName | The internal ID identifying the audio |
| Audio Type | EDialogAudioType | The audio type |
| Audio Object | USoundBase* | The actual audio object |

## Related Enums

### EDialogAudioType
The audio type enumeration that defines what kind of audio this is:
- Background Music (BGM)
- Sound Effects (SFX)
- Voice Over
