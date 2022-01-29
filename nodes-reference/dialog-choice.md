---
layout: default
title: Dialog Choice
parent: Nodes Reference
---
# Dialog Choice

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