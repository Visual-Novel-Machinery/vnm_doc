---
layout: single
title: Character Show
permalink: /docs/nodes-references/character-show
toc: true
sidebar:
  nav: "docs"
---


![Character Show Node Visual]({{ site.baseurl }}/assets/images/NodeReference/character-show.png)

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
| Character | The Id of the character to show |
| Emotion | The Id of the emotion of the character to show |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Character Positioning | The position of the character (LEFT/CENTER/RIGHT/TRUECENTER) |
| Transition Event | Transition Event | How should the character be shown |
| Custom Transition Event Name | FString | The name of the animation to use if Transition Event is set to Custom |
| Dont Wait For Transition To Finish | Boolean | If set to true then the dialog will automatically continue, while the character finishes its transition |

## Script Reference
```
character.show -id=<character id> -emotion=<emotion id> [-position=<CENTER/LEFT/RIGHT/CUSTOM>] [-transition=<transition name>] [-dontwait] [-customtransition=<Animation name>]
```