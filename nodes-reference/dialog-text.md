---
layout: default
title: Dialog Text
parent: Nodes Reference
---
# Dialog Text

![Dialog Text Node Visual]({{ site.baseurl }}/assets/images/NodeReference/dialog-text.png)

## Pins

### Input

| Name | Type | Description |
| --- | --- | --- |
| Execution Line In | Execution | Execution Line Input |
| Dialog Text | Text | Dialog Text to display. Must be activated in additional properties to be displayed |

### Output

| Name | Type | Description |
| --- | --- | --- |
| Execution Line Out | Execution | Execution Line Output |

## On-Node Properties

| Name | Description |
| --- | --- |
| Character | The id of the character that is talking. If set to None, then no character name is displayed |
| Text | The text the character is saying |
| Emotion | The id of the emotion of the character to show |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Character Positioning | The position of the character (LEFT/CENTER/RIGHT/TRUECENTER) |
| Transition Event | Transition Event | How should the character be shown |
| Custom Transition Event Name | FString | The name of the animation to use if Transition Event is set to Custom |
| Dont Wait For Transition To Finish | Boolean | If set to true then the dialog will automatically continue, while the character finishes its transition |
| Use Dialog Text Pin | Boolean | If set to true then instead of writing the text into the node directly, a pin will be exposed, which value will be used instead |
| Use Voice Over | Boolean | Activates Voice Over System on Dialog Text Node |
| Use Character Voice Over | Boolean | Uses voice overs for the character specified on the node |
| Use Dialog Voice Over | Boolean | Uses voice overs for the dialog this node exists in |
| Voice Over Id | FString | The Voice Over Id to be used. It is different depending on if you are using character voice overs or dialog voice overs |
| Volume | float | The volume at which the voice over should play (0.0-1.0) |
| Pitch | float | The pitch at which the voice over will be played |
| Start Time | float | The time in seconds at which to start in the voice over. Default is 0.0 seconds. |
