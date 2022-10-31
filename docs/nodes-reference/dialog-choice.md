---
layout: single
title: Dialog Choice
permalink: /docs/nodes-references/dialog-choice
toc: true
sidebar:
  nav: "docs"
---


![Dialog Choice Node Visual]({{ site.baseurl }}/assets/images/NodeReference/dialog-choice.png)

## Pins

### Input

| Name | Type | Description |
| --- | --- | --- |
| Execution Line In | Execution | Execution Line Input |
| Choice Option N Available (If conditional choice) | Boolean | Conditional value specifying if the option is visible to the player. One option should always be set to true, otherwise your game enters a lifelock. |

### Output

| Name | Type | Description |
| --- | --- | --- |
| Choice Option N (Name depends on properties specified below) | Execution | A potential choice |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Choices | TArray\<FText\> | The choices the player can make at this junction. When changing this, the node will regenerate all its output pins to the match the choices array. |
| Make Choice Conditional | Boolean | Makes all choices conditional. If a condition is not met the choice is hidden from the player. |
| Is Image Choice | Boolean | Check this to make the choice an image choice. If this is checked you can then set the Image Choice Widget class |
| Image Choice Widget Class | TSubclassOf\<UBaseImageChoiceWidget\> | The widget that should be displayed if this choice is an image choice |
| Is 3DChoice | Boolean | Check this if you want to make the choice a 3D choice. If this is checked then the choice system will search for ChoiceActors/ChoicePawns/ChoiceCharacters in the level instead of using the UI. |

## Script Reference
```
dialog.choice "<choice text 1>" <choice label 1> "<choice text 2>" <choice label 2> [...]
```
```
dialog.choice.conditional <choice 1 condition variable> "<choice text 1>" <choice label 1> <choice 2 condition variable> "<choice text 2>" <choice label 2> [...]
```