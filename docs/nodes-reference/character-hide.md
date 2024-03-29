---
layout: single
title: Character Hide
permalink: /docs/nodes-references/character-hide
toc: true
sidebar:
  nav: "docs"
---


![Character Hide Node Visual]({{ site.baseurl }}/assets/images/NodeReference/character-hide.png)

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
| Character | The Id of the character to hide |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Transition Event | Transition Event | How should the Character be hidden |
| Custom Transition Event Name | FString | The name of the animation to use if Transition Event is set to Custom |
| Dont Wait For Transition To Finish | Boolean | If set to true then the dialog will automatically continue, while the Character finishes its transition |

## Script Reference
```
character.hide -id=<character id> [-position=<CENTER/LEFT/RIGHT/CUSTOM>] [-transition=<transition name>] [-dontwait] [-customtransition=<Animation name>]
```