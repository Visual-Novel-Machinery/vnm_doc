---
layout: single
title: Global Persistant Memory Set
permalink: /docs/nodes-references/global-persistant-memory-set
toc: true
sidebar:
  nav: "docs"
---


![Global Persistant Memory Set Node Visual]({{ site.baseurl }}/assets/images/NodeReference/global-persistant-memory-set.png)

## Pins

### Input

| Name | Type | Description |
| --- | --- | --- |
| Execution Line In | Execution | Execution Line Input |
| Persistant Global Memory Id | Name | The ID of the global persistant memory variable to set (only shown when "Use Pins For Ids" is enabled) |
| Value | Variable | The value to set for the global persistant memory variable (type depends on the memory type) |

### Output

| Name | Type | Description |
| --- | --- | --- |
| Execution Line Out | Execution | Execution Line Output |

## On-Node Properties

| Name | Description |
| --- | --- |
| Memory | Name | The ID of the global persistant memory variable to set (only shown when "Use Pins For Ids" is disabled) |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Use Pins For Ids | Boolean | If set to true, the Persistant Global Memory Id will be available as an input pin instead of a property |

## Script Reference
```
global.memory.persistant.set <global persistant memory id> <variable name>
```