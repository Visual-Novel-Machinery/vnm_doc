---
layout: single
title: Global Memory Set
permalink: /docs/nodes-references/global-memory-set
toc: true
sidebar:
  nav: "docs"
---


![Global Memory Set Node Visual]({{ site.baseurl }}/assets/images/NodeReference/global-memory-set.png)

## Pins

### Input

| Name | Type | Description |
| --- | --- | --- |
| Execution Line In | Execution | Execution Line Input |
| Global Memory Id | Name | The ID of the global memory variable to set (only shown when "Use Pins For Ids" is enabled) |
| Value | Variable | The value to set for the global memory variable (type depends on the memory type) |

### Output

| Name | Type | Description |
| --- | --- | --- |
| Execution Line Out | Execution | Execution Line Output |

## On-Node Properties

| Name | Description |
| --- | --- |
| Memory | Name | The ID of the global memory variable to set (only shown when "Use Pins For Ids" is disabled) |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Use Pins For Ids | Boolean | If set to true, the Global Memory Id will be available as an input pin instead of a property |

## Script Reference
```
global.memory.set <global memory id> <variable name>
```