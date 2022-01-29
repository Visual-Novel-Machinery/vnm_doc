---
layout: default
title: Character Move
parent: Nodes Reference
---
# Character Move

![Character Move Node Visual]({{ site.baseurl }}/assets/images/NodeReference/character-move.png)

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
| Character | The Id of the character to be moved |
| Character Position | The new position of the character (LEFT/CENTER/RIGHT/TRUECENTER) |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Move With Animation | Boolean | If set to true then the character will slide to its new position instead of teleporting to it |